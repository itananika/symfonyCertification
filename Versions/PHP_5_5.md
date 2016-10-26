###New capability
1. Generators added;
2. try-catch blocks now support a finally block;
3. Added **`password_hash()`** (New password hashing)
4. `foreach` now supports **`list()`**: <blockquote> foreach ($array as list($a, $b)) {} <blockquote>
5. Passing an arbitrary expression instead of a variable to **`empty()`** is now supported;
6. array and string literal dereferencing: 
    ```php 
        <?php 
            echo [1, 2, 3][0] . 'PHP'[0]; 
        ?>
    ```
7. Class name resolution via `::class`;
8. OPcache extension added(like APC);
9. `foreach` now supports non-scalar keys;
10. The Apache 2.4 handler SAPI is now supported on Windows;

###Backward Incompatible
1. Support for Windows XP and 2003 has been dropped;
2. All case insensitive matching for function, class and constant names is now performed in a locale independent manner according to ASCII rules;
3. **`pack()`** and **`unpack()`** now supports the "Z" format code, which behaves identically to "a";
4. **`unpack()`** now keeps trailing NULL bytes and strips all trailing ASCII whitespace when the "a" format code is used;
5. `self`, `parent` and `static` are now always case insensitive;
6. PHP logo GUIDs removed. As result removed related functions: **`php_logo_guid()`**, **`php_egg_logo_guid()`**, 
    **`php_real_logo_guid()`**, **`zend_logo_guid()`**;
