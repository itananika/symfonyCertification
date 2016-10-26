###1. Trait example
```php
<?php
    trait ezcReflectionReturnInfo {
        function getReturnType() { /*1*/ }
        function getReturnDescription() { /*2*/ }
    }
    
    class ezcReflectionMethod extends ReflectionMethod {
        use ezcReflectionReturnInfo;
        /* ... */
    }
    
    class ezcReflectionFunction extends ReflectionFunction {
        use ezcReflectionReturnInfo;
        /* ... */
    }
?>
```

###2. Precedence Order Example
An inherited member from a base class is overridden by a member inserted by a Trait. 
The precedence order is that members from the current class override Trait methods, which in turn override inherited methods
>
    parentObject > trait > childObject
>
```php
<?php
    class Base {
        public function sayHello() {
            echo 'Hello ';
        }
    }
    
    trait SayWorld {
        public function sayHello() {
            parent::sayHello();
            echo 'World!';
        }
    }
    
    class MyHelloWorld extends Base {
        use SayWorld;
    }
    
    $o = new MyHelloWorld();
    $o->sayHello();
?>
```
output
>   
    Hello World!
>

###3. Conflict Resolution 
If two Traits insert a method with the same name, a fatal error is produced, if the conflict is not explicitly resolved.
To resolve naming conflicts between Traits used in the same class, 
the insteadof operator needs to be used to choose exactly one of the conflicting methods.
```php
<?php
trait A {
    public function smallTalk() {
        echo 'a';
    }
    public function bigTalk() {
        echo 'A';
    }
}

trait B {
    public function smallTalk() {
        echo 'b';
    }
    public function bigTalk() {
        echo 'B';
    }
}

class Talker {
    use A, B {
        B::smallTalk insteadof A;
        A::bigTalk insteadof B;
    }
}

class Aliased_Talker {
    use A, B {
        B::smallTalk insteadof A;
        A::bigTalk insteadof B;
        B::bigTalk as talk;
    }
}
?>
```

**Using the as syntax, one can also adjust the visibility of the method in the exhibiting class.**
```php
<?php
trait HelloWorld {
    public function sayHello() {
        echo 'Hello World!';
    }
}

class MyClass1 {
    use HelloWorld { sayHello as protected; }
}
?>
```

###4. Traits Composed from Traits
```php
<?php
trait Hello {
    public function sayHello() {
        echo 'Hello ';
    }
}

trait World {
    public function sayWorld() {
        echo 'World!';
    }
}

trait HelloWorld {
    use Hello, World;
}
?>
```

###5. Abstract Trait Members
```php
<?php
trait Hello {
    public function sayHelloWorld() {
        echo 'Hello'.$this->getWorld();
    }
    abstract public function getWorld();
}

class MyHelloWorld {
    private $world;
    use Hello;
    public function getWorld() {
        return $this->world;
    }
    public function setWorld($val) {
        $this->world = $val;
    }
}
?>
```
###6. Static Trait Members
```php
<?php
trait StaticExample {
    public function inc() {
        static $c = 0;
        $c = $c + 1;
        echo "$c\n";
    }
    public static function doSomething() {
            echo 'Doing something';
        }
}

class Example {
    use StaticExample;
}

$o = new Example(); 
$o->inc(); // echo 1
Example::doSomething(); // echo 'Doing something'
?>
```
###7. Properties
If a trait defines a property then a class can not define a property with the same name, otherwise an error is issued. 
It is an E_STRICT if the class definition is compatible (same visibility and initial value) or fatal error otherwise.
```php
<?php
trait PropertiesTrait {
    public $same = true;
    public $different = false;
}

class PropertiesExample {
    use PropertiesTrait;
    public $same = true; // Strict Standards
    public $different = true; // Fatal error
}
?>
```