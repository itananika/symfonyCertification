###New capability
1. Traits supporting;
2. Short array syntax;
3. Function array dereferencing has been added;
4. Closures now support **`$this`**;
5. ***<?=*** is now always available;
6. Class member access on instantiation has been added, e.g. **`(new Foo)->bar()`**;
7. **`Class::{expr}()`** syntax is now supported;
8. Binary number format has been added;
9. Improved parse error messages and improved incompatible arguments warnings;
10. The session extension can now track the upload progress of files;
11. Built-in development web server in CLI mode;

###Backward Incompatible
1. Safe mode is no longer supported;
2. Magic quotes has been removed. **`get_magic_quotes_gpc()`** and **`get_magic_quotes_runtime()`** now always return _`FALSE`_. 
    **`set_magic_quotes_runtime()`** raises an _`E_CORE_ERROR`_ level error on trying to enable Magic quotes;
3. The **`register_globals`** and **`register_long_arrays`** php.ini directives have been removed;
4. Removed **`mbstring.script_encoding`**. Use **`zend.script_encoding`** instead;
5. Removed passing by Reference, so using it will raise a fatal error;
6. The **`break`** and **`continue`** statements don't accept variable arguments **`break 1 + foo() * $bar;`**. 
    Static arguments **`break 2;`** still work. Arguments **`break 0;`** and **`continue 0;`** are not allowed.
7. The timezone can't be sets using the TZ environment variable. Specify a timezone using the `date.timezone` php.ini option 
    or **`date_default_timezone_set()`** function. PHP won't attempt to guess the timezone, "UTC" -> as default and issue a *`E_WARNING`*;
8. Non-numeric string offsets(**`$a['foo']`**), where **`$a`** is a string. 
    **`(isset($a['foo']) === false && !empty($a['foo'])) === true`**, and produce a *`E_WARNING`* if you try to use them. 
    Offsets of types double, bool and null produce a *`E_NOTICE`*. Numeric strings(**`$a['2']`**) still work. 
    Note: Offsets like '12.3' && '5 foobar' are considered non-numeric and produce a *`E_WARNING`*. 
    Note: Following code returns different result. **`$str='abc';var_dump(isset($str['x']));`** // false for PHP 5.4+, true 5.3-;
9. **`(string)[1, 2, 3]`** will now generate an *`E_NOTICE`* level error. But the result **`Array`**;
10. Turning **`NULL`**, **`FALSE`**, or an **`empty`** string into an object by adding a property will now emit an *`E_WARNING`* level error, instead of *`E_STRICT`*;
11. **`foo($_GET, $_POST) {}`** calls fatal error. Parameter names that shadow super globals not allowed;
12. The `Salsa10` and `Salsa20` hash algorithms have been removed;
13. **`array_combine([], [])`** for <PHP5.4 issued _`E_WARNING`_ and returned _`FALSE`_. >PHP5.4 result === **`[]`**
14. If you use **`htmlentities()`** with asian character sets, it works like **`htmlspecialchars()`** - this has always been the case in previous versions of PHP,
    but now an _`E_STRICT`_ level error is emitted;
15. The third parameter of **`ob_start()`** has changed from boolean erase to integer flags;

###Reserved words
trait, callable, insteadof
