###Datastructures
1. **`SplDoublyLinkedList`** — The SplDoublyLinkedList class. >= 5.3.0, PHP 7
2. **`SplStack`** — The SplStack class. >= 5.3.0, PHP 7
3. **`SplQueue`** — The SplQueue class. >= 5.3.0, PHP 7
4. **`SplHeap`** — The SplHeap class. >= 5.3.0, PHP 7
5. **`SplMaxHeap`** — The SplMaxHeap class. >= 5.3.0, PHP 7. keeping the maximum on the top.
6. **`SplMinHeap`** — The SplMinHeap class. >= 5.3.0, PHP 7. keeping the min on the top.
7. **`SplPriorityQueue`** — The SplPriorityQueue class. >= 5.3.0, PHP 7
8. **`SplFixedArray`** — The SplFixedArray class. >= 5.3.0, PHP 7. fixed length with int keys. Faster than single array
9. **`SplObjectStorage`** — The SplObjectStorage class. >= 5.3.0, PHP 7

###Iterators
1. **`AppendIterator`** — The AppendIterator class. >= 5.1.0, PHP 7. 
    An Iterator that iterates over several iterators one after the other. extends **`IteratorIterator`**
2. **`ArrayIterator`** — The ArrayIterator class. PHP 5, PHP 7
3. **`CachingIterator`** — The CachingIterator class. PHP 5, PHP 7
4. **`CallbackFilterIterator`** — The CallbackFilterIterator class>= 5.4.0, PHP 7
```php
<?php
$dir = new FilesystemIterator(__DIR__);

function is_large_file($current) {
    return $current->isFile() && $current->getSize() > 104857600;
}
$large_files = new CallbackFilterIterator($dir, 'is_large_file');
$files = new CallbackFilterIterator($dir, function ($current, $key, $iterator) {
    return $current->isDir() && ! $iterator->isDot();
});
?>
```
5. **`DirectoryIterator`** — The DirectoryIterator class
6. **`EmptyIterator`** — The EmptyIterator class
7. **`FilesystemIterator`** — The FilesystemIterator class. >= 5.3.0, PHP 7
8. **`FilterIterator`** — The FilterIterator class. >= 5.1.0, PHP 7
9. **`GlobIterator`** — The GlobIterator class. >= 5.3.0, PHP 7. similar fashion to glob().
10. **`InfiniteIterator`** — The InfiniteIterator class. >= 5.1.0, PHP 7
```php
<?php

$obj = new stdClass();
$obj->Mon = "Monday";
....
$obj->Sun = "Sunday";

$infinate = new InfiniteIterator(new ArrayIterator($obj));
foreach ( new LimitIterator($infinate, 0, 14) as $value ) {
    print($value . PHP_EOL);
}
?>
```
output will be infinity day list
11. **`IteratorIterator`** — The IteratorIterator class. >= 5.1.0, PHP 7
12. **`LimitIterator`** — The LimitIterator class. >= 5.1.0, PHP 7
```php
<?
$fruits = new ArrayIterator(array(
    'apple',
    'banana',
    'cherry',
    'damson',
    'elderberry'
));

//$count is not required
foreach (new LimitIterator($fruits, $startFrom, $count) as $fruit) {
    var_dump($fruit);
}
?>
```
13. **`MultipleIterator`** — The MultipleIterator class. >= 5.3.0, PHP 7. Iterator for all attached iterators
14. **`NoRewindIterator`** — The NoRewindIterator class. >= 5.1.0, PHP 7
15. **`ParentIterator`** — The ParentIterator class. >= 5.1.0, PHP 7 extends FilterIterator.
    allows a recursive iteration using RecursiveIteratorIterator that only shows those elements which have children
16. **`RecursiveArrayIterator`** — The RecursiveArrayIterator class. >= 5.1.0, PHP 7
    This iterator allows to unset and modify values and keys while iterating over Arrays and Objects in the same way as the ArrayIterator.
17. **`RecursiveCachingIterator`** — The RecursiveCachingIterator class. >= 5.1.0, PHP 7
18. **`RecursiveCallbackFilterIterator`** — The RecursiveCallbackFilterIterator class. >= 5.4.0, PHP 7
19. **`RecursiveDirectoryIterator`** — The RecursiveDirectoryIterator class. PHP 5, PHP 7
20. **`RecursiveFilterIterator`** — The RecursiveFilterIterator class. >= 5.1.0, PHP 7
21. **`RecursiveIteratorIterator`** — The RecursiveIteratorIterator class. PHP 5, PHP 7
22. **`RecursiveRegexIterator`** — The RecursiveRegexIterator class. >= 5.2.0, PHP 7. This recursive iterator can filter another recursive iterator via a regular expression.
23. **`RecursiveTreeIterator`** — The RecursiveTreeIterator class. >= 5.3.0, PHP 7
24. **`RegexIterator`** — The RegexIterator class. >= 5.2.0, PHP 7

###Interfaces
1. **`Countable`** — The Countable interface. >= 5.1.0, PHP 7
2. **`OuterIterator`** — The OuterIterator interface. >= 5.1.0, PHP 7. can be used to iterate over iterators.
3. **`RecursiveIterator`** — The RecursiveIterator interface. >= 5.1.0, PHP 7. can be used to Recursive iterate over iterators.
4. **`SeekableIterator`** — The SeekableIterator interface. >= 5.1.0, PHP 7

###Exceptions
1. **`BadFunctionCallException`** — The BadFunctionCallException class. >= 5.1.0, PHP 7. 
    callback refers to an undefined function or if some arguments are missing
2. **`BadMethodCallException`** — The BadMethodCallException class. >= 5.1.0, PHP 7
3. **`DomainException`** — The DomainException class. >= 5.1.0, PHP 7
4. **`InvalidArgumentException`** — The InvalidArgumentException class. >= 5.1.0, PHP 7
5. **`LengthException`** — The LengthException class. >= 5.1.0, PHP 7
6. **`LogicException`** — The LogicException class. >= 5.1.0, PHP 7
7. **`OutOfBoundsException`** — The OutOfBoundsException class. >= 5.1.0, PHP 7. Exception thrown if a value is not a valid key
8. **`OutOfRangeException`** — The OutOfRangeException class. >= 5.1.0, PHP 7. an illegal index was requested
9. **`OverflowException`** — The OverflowException class. >= 5.1.0, PHP 7. adding an element to a full container.
10. **`RangeException`** — The RangeException class. >= 5.1.0, PHP 7
11. **`RuntimeException`** — The RuntimeException class. >= 5.1.0, PHP 7
12. **`UnderflowException`** — The UnderflowException class. >= 5.1.0, PHP 7.
    performing an invalid operation on an empty container, such as removing an element.
13. **`UnexpectedValueException`** — The UnexpectedValueException class. >= 5.1.0, PHP 7

###SPL Functions
1. **`class_implements`** — Return the interfaces which are implemented by the given class or interface. >= 5.1.0, PHP 7
2. **`class_parents`** — Return the parent classes of the given class. >= 5.1.0, PHP 7
3. **`class_uses`** — Return the traits used by the given class. >= 5.4.0, PHP 7
4. **`iterator_apply`** — Call a function for every element in an iterator. >= 5.1.0, PHP 7
5. **`iterator_count`** — Count the elements in an iterator. >= 5.1.0, PHP 7
6. **`iterator_to_array`** — Copy the iterator into an array. >= 5.1.0, PHP 7
7. **`spl_autoload_call`** — Try all registered __autoload() function to load the requested class. >= 5.1.2, PHP 7
8. **`spl_autoload_extensions`** — Register and return default file extensions for spl_autoload. >= 5.1.2, PHP 7
9. **`spl_autoload_functions`** — Return all registered __autoload() functions. >= 5.1.2, PHP 7
10. **`spl_autoload_register`** — Register given function as __autoload() implementation. >= 5.1.2, PHP 7
11. **`spl_autoload_unregister`** — Unregister given function as __autoload() implementation. >= 5.1.2, PHP 7
12. **`spl_autoload`** — Default implementation for __autoload(). >= 5.1.2, PHP 7
13. **`spl_classes`** — Return available SPL classes. PHP 5, PHP 7
14. **`spl_object_hash`** — Return hash id for given object. >= 5.2.0, PHP 7

###File Handling
1. **`SplFileInfo`** — The SplFileInfo class. >= 5.1.2, PHP 7
2. **`SplFileObject`** — The SplFileObject class. >= 5.1.0, PHP 7
3. **`SplTempFileObject`** — The SplTempFileObject class. >= 5.1.2, PHP 7

###Miscellaneous Classes and Interfaces
1. **`ArrayObject`** — The ArrayObject class
2. **`SplObserver`** — The SplObserver interface
3. **`SplSubject`** — The SplSubject interface