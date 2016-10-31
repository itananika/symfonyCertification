###Core Extensions
1. Arrays;
2. Classes/Objects
3. Date/Time
4. Directories
5. Error Handling
6. Program execution
7. Filesystem
8. Filter
9. Function Handling
10. Hash
11. PHP Options/Info
12. Mail. PHP must have access to the sendmail binary on your system during compile time. If you use another mail program,
    be sure to use the appropriate sendmail wrappers that come with them
13. Math
14. Misc.
15. Network
16. Output Control
17. Password Hashing
18. Phar
19. Reflection. 
20. POSIX Regex. This feature was DEPRECATED in PHP 5.3.0, and REMOVED in PHP 7.0.0
21. Sessions
22. SPL. The Standard PHP Library (SPL) is a collection of interfaces and classes that are meant to solve common problems
    it is available and compiled by default in PHP 5.0.0.
23. Streams
24. Strings
25. Tokenizer. The tokenizer functions provide an interface to the PHP tokenizer embedded in the Zend Engine. 
    Using these functions you may write your own PHP source analyzing or modification tools without having to deal with the language specification at the lexical level.
26. URLs
27. Variable handling

###Bundled Extensions
1. Apache. These functions are only available when running PHP as an Apache module.
2. BC Math. BCMath Arbitrary Precision Mathematics
3. Calendar
4. COM. Starting with PHP 5, this extension (and this documentation) was rewritten from scratch
5. Ctype. Character type checking
6. DBA. Database (dbm-style) Abstraction Layer
7. Exif. Exchangeable image information
8. Fileinfo
9. FTP
10. iconv
11. GD. Image Processing and GD. We can output image content instead of html
12. intl. Internationalization Functions
13. JSON
14. Multibyte String
15. NSAPI
16. PCNTL. Process Control
17. PCRE. The PCRE library is a set of functions that implement regular expression pattern matching using the same syntax and semantics as Perl 
18. PDO. DO ships with PHP 5.1, and is available as a PECL extension for PHP 5.0
19. POSIX
20. Semaphore
21. Shared Memory
22. Sockets
23. SQLite3
24. XML-RPC
25. Zlib

###External Extensions
1. Bzip2. The bzip2 functions are used to transparently read and write bzip2 (.bz2) compressed files.
2. cURL
3. dBase
4. DOM
5. Enchant
6. FrontBase. This extension has been moved to the » PECL repository and is no longer bundled with PHP as of PHP 5.3.0.
7. Gettext. The gettext functions implement an NLS (Native Language Support) API which can be used to internationalize your PHP applications.
8. GMP. These functions allow for arbitrary-length integers to be worked with using the GNU MP library.
    However, note that PHP 5.5 and earlier represented GMP numbers as resources
9. Firebird/InterBase
10. Informix. This extension has been moved to the » PECL repository and is no longer bundled with PHP as of PHP 5.2.1. 
11. IMAP
12. LDAP. Lightweight Directory Access Protocol 
13. libxml. These functions/constants are available as of PHP 5.1.0, and the following core extensions rely on this 
    libxml extension: DOM, libxml, SimpleXML, SOAP, WDDX, XSL, XML, XMLReader, XMLRPC and XMLWriter.
14. Mcrypt
15. Mhash. This extension is obsoleted by Hash.
16. mSQL
17. Mssql. This feature was REMOVED in PHP 7.0.0.
18. MySQL (Original). This extension is deprecated as of PHP 5.5.0, and has been removed as of PHP 7.0.0. Instead, either the mysqli or PDO_MySQL extension 
19. MySQLi
20. Mysqlnd
21. OCI8
22. OpenSSL
23. MS SQL Server (PDO)
24. Firebird (PDO)
25. MySQL (PDO)
26. Oracle (PDO)
27. ODBC and DB2 (PDO)
28. PostgreSQL (PDO)
29. SQLite (PDO)
30. PostgreSQL
31. Pspell. These functions allow you to check the spelling of a word and offer suggestions.
32. Readline
33. Recode
34. SimpleXML
35. SNMP. The SNMP extension provides a very simple and easily usable toolset for managing remote devices via the Simple Network Management Protocol.
36. SOAP
37. Sybase. As of PHP 7.0.0, the sybase_ct extension has been removed.
38. Tidy. Tidy is a binding for the Tidy HTML clean and repair utility which allows you to not only clean and otherwise manipulate HTML documents, 
    but also traverse the document tree.
39. ODBC
40. WDDX
41. XML Parser
42. XMLReader
43. XMLWriter
44. XSL
45. Zip

###PECL Extensions
1. APC. This extension is considered unmaintained and dead
2. APD. Advanced PHP debugger. APD is a Zend Extension, modifying the way the internals of PHP handle function calls, and thus may or may not be compatible with other Zend Extensions
3. BBCode. This extension aims to help parse BBCode text in order to convert it to HTML or another markup language
4. bcompiler. PHP bytecode Compiler. This extension is EXPERIMENTAL
5. Cairo. Cairo is a native PHP extension to create and modify graphics using the Cairo Graphics Library.
6. chdb.  is a fast key-value database for constant data. Fast loading
7. Classkit. These functions allow the dynamic manipulation of PHP classes, at runtime.
    This extension has been replaced by runkit, which is not limited to class manipulation but has function manipulation
8. Crack. These functions allow you to use the CrackLib library to test the 'strength' of a password.
    This extension has been moved to the » PECL repository and is no longer bundled with PHP as of PHP 5.0.0.
9. CUBRID. These functions allow you to access CUBRID database servers.
10. Cyrus. Cyrus IMAP administration. This extension has been moved to the » PECL repository and is no longer bundled with PHP as of PHP 5.0.0.
11. DB++. db++, made by the German company » Concept asa, is a relational database system with high performance and low memory and disk usage in mind.
    This extension is EXPERIMENTAL
12. dbx. The dbx module is a database abstraction layer. This extension has been moved to the » PECL repository and is no longer bundled with PHP as of PHP 5.1.0.
13. Direct IO. HP supports the direct io functions as described in the Posix Standard.
    This extension has been moved to the » PECL repository and is no longer bundled with PHP as of PHP 5.0.0.
14. Eio. This extension provides asyncronous POSIX I/O by means. each request is executed in a thread
15. Ev. Libev is an event loop: one registers interest in certain events (such as a file descriptor being readable or a timeout occurring), 
    and it will manage these event sources and provide the program with events.
16. Event. PHP event service works at PHP 5.4+
17. Expect. FAM monitors files and directories, notifying interested applications of changes
18. FAM
19. FDF. Forms Data Format (FDF) is a format for handling forms within PDF documents
20. filePro
21. FriBiDi
22. Gearman
23. Gender
24. GeoIP
25. Gmagick
26. GnuPG
27. Gupnp
28. haru
29. htscanner
30. Hyperwave API
31. IBM DB2
32. ID3
33. IIS
34. ImageMagick
35. inclued
36. Ingres
37. Inotify
38. Judy
39. KADM5
40. KTaglib
41. Lapack
42. Libevent
43. Lua
44. LZF
45. Mailparse
46. MaxDB
47. MCVE
48. Memcache
49. Memcached
50. Memtrack
51. Mimetype
52. Ming
53. mnoGoSearch
54. Mongo
55. mqseries
56. Msession
57. mysqlnd_memcache
58. mysqlnd_ms
59. mysqlnd_mux
60. mysqlnd_qc
61. mysqlnd_uh
62. Ncurses
63. Gopher
64. Newt
65. YP/NIS
66. OAuth
67. oggvorbis
68. OpenAL
69. Paradox
70. Parsekit
71. PDF
72. 4D (PDO)
73. CUBRID (PDO)
74. IBM (PDO)
75. Informix (PDO)
76. MS SQL Server (PDO)
77. Proctitle
78. PS
79. pthreads
80. Quickhash
81. Radius
82. Rar
83. RPM Reader
84. RRD
85. runkit
86. SAM
87. SCA
88. scream
89. SDO
90. SDO DAS XML
91. SDO-DAS-Relational
92. Session PgSQL
93. Solr
93. Sphinx
94. SPL Types
95. SPPLUS
96. SQLite
97. SQLSRV
98. ssdeep
99. SSH2
100. Statistics
101. Stomp
102. SVM
103. SVN
104. Swish
105. Taint
106. TCP
107. tokyo_tyrant
108. Trader
109. V8js
110. Varnish
111. vpopmail
112. Weakref
113. win32ps
114. win32service
115. WinCache
116. xattr
117. xdiff
118. Xhprof
119. Yaf
120. Yaml
121. YAZ