###New capability
1. Constant expressions. It is now possible to provide a scalar expression involving numeric and string literals and/or constants
```php
<?php
class C {
    const ONE = 1;
    const THREE = self::ONE + 1;
    const ONE_THIRD = self::ONE / self::THREE;
    const SENTENCE = 'The value of THREE is '.self::THREE;

    public function f($a = self::ONE + self::THREE) {
        return $a;
    }
}
?>
```
2. Variadic functions via ... . 
```php
<?php
    function f($req, $opt = null, ...$params) {}
?>
```
3. Argument unpacking via ...
```php
<?php
    function add($a, $b, $c) {
        return $a + $b + $c;
    }
    $operators = [2, 3];
    echo add(1, ...$operators);
?>
```
4. Exponentiation via `**`
```php
<?php
    printf("2 ** 3 == %d\n", 2 ** 3);//8
?>
```
5. Use function and use const
```php
<?php
    namespace Name\Space {
        const FOO = 42;
        function f() { echo __FUNCTION__."\n"; }
    }
    
    namespace {
        use const Name\Space\FOO;
        use function Name\Space\f;
    
        echo FOO."\n";
        f();
    }
?>
```
6. `default_charset` is now used as the default character set for the `htmlentities()`, `html_entity_decode()` and `htmlspecialchars()`.
7. php://input may now be reopened and read as many times as required;
8. Files larger than 2 gigabytes in size are now accepted;
9. The hash_equals() function has been added to compare two strings in constant time;
10. The __debugInfo() magic method has been added to allow objects to change the properties and values;
11. The gost-crypto hash algorithm has been added. This implements the GOST hash function using the CryptoPro S-box tables as specified by » RFC 4357, section 11.2.
12. pgsql async support;


###Backward Incompatible
1. Array keys won't be overwritten when defining an array as a property of a class via an array literal
```php
<?php
    class C {
        const ONE = 1;
        public $array = [
            self::ONE => 'foo',
            'bar',
            'quux',
        ];
    }
    var_dump((new C)->array);
        
?>
```
>    5.5:
> 
    array(2) {
        [0]=`>`
            string(3) "bar"
        [1]=`>`
            string(4) "quux"
    }
>    5.6:
> 
    array(2) {
       [1]=>
           string(3) "bar"
       [2]=>
           string(3) "bar"
       [3]=>
           string(4) "quux"
    }


2. **`json_decode()`** now rejects non-lowercase variants of the JSON literals `true`, `false` and `null`;
3. Stream wrappers now verify peer certificates and host names by default when using (SSL/TLS );
4. GMP resources are now objects(GNU Multiple Precision);
5. cURL file uploads. Uploads using the @file syntax now require CURLOPT_SAFE_UPLOAD to be set to FALSE. CURLFile should be used instead;
6. PHP logo GUIDs removed. As result removed related functions: **`php_logo_guid()`**, **`php_egg_logo_guid()`**, 
    **`php_real_logo_guid()`**, **`zend_logo_guid()`**;
