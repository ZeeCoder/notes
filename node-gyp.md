###node-gyp errors and solutions.

##Python and OpenSSL issue

**Solution:** https://github.com/Homebrew/homebrew/issues/22816#issuecomment-25271211

**Error:**

```
ERROR:root:code for hash md5 was not found.
Traceback (most recent call last):
  File "/usr/local/Cellar/python/2.7.9/Frameworks/Python.framework/Versions/2.7/lib/python2.7/hashlib.py", line 147, in <module>
    globals()[__func_name] = __get_hash(__func_name)
  File "/usr/local/Cellar/python/2.7.9/Frameworks/Python.framework/Versions/2.7/lib/python2.7/hashlib.py", line 97, in __get_builtin_constructor
    raise ValueError('unsupported hash type ' + name)
ValueError: unsupported hash type md5
ERROR:root:code for hash sha1 was not found.
Traceback (most recent call last):
  File "/usr/local/Cellar/python/2.7.9/Frameworks/Python.framework/Versions/2.7/lib/python2.7/hashlib.py", line 147, in <module>
    globals()[__func_name] = __get_hash(__func_name)
  File "/usr/local/Cellar/python/2.7.9/Frameworks/Python.framework/Versions/2.7/lib/python2.7/hashlib.py", line 97, in __get_builtin_constructor
    raise ValueError('unsupported hash type ' + name)
ValueError: unsupported hash type sha1
ERROR:root:code for hash sha224 was not found.
Traceback (most recent call last):
  File "/usr/local/Cellar/python/2.7.9/Frameworks/Python.framework/Versions/2.7/lib/python2.7/hashlib.py", line 147, in <module>
    globals()[__func_name] = __get_hash(__func_name)
  File "/usr/local/Cellar/python/2.7.9/Frameworks/Python.framework/Versions/2.7/lib/python2.7/hashlib.py", line 97, in __get_builtin_constructor
    raise ValueError('unsupported hash type ' + name)
ValueError: unsupported hash type sha224
ERROR:root:code for hash sha256 was not found.
Traceback (most recent call last):
  File "/usr/local/Cellar/python/2.7.9/Frameworks/Python.framework/Versions/2.7/lib/python2.7/hashlib.py", line 147, in <module>
    globals()[__func_name] = __get_hash(__func_name)
  File "/usr/local/Cellar/python/2.7.9/Frameworks/Python.framework/Versions/2.7/lib/python2.7/hashlib.py", line 97, in __get_builtin_constructor
    raise ValueError('unsupported hash type ' + name)
ValueError: unsupported hash type sha256
ERROR:root:code for hash sha384 was not found.
Traceback (most recent call last):
  File "/usr/local/Cellar/python/2.7.9/Frameworks/Python.framework/Versions/2.7/lib/python2.7/hashlib.py", line 147, in <module>
    globals()[__func_name] = __get_hash(__func_name)
  File "/usr/local/Cellar/python/2.7.9/Frameworks/Python.framework/Versions/2.7/lib/python2.7/hashlib.py", line 97, in __get_builtin_constructor
    raise ValueError('unsupported hash type ' + name)
ValueError: unsupported hash type sha384
ERROR:root:code for hash sha512 was not found.
Traceback (most recent call last):
  File "/usr/local/Cellar/python/2.7.9/Frameworks/Python.framework/Versions/2.7/lib/python2.7/hashlib.py", line 147, in <module>
    globals()[__func_name] = __get_hash(__func_name)
  File "/usr/local/Cellar/python/2.7.9/Frameworks/Python.framework/Versions/2.7/lib/python2.7/hashlib.py", line 97, in __get_builtin_constructor
    raise ValueError('unsupported hash type ' + name)
ValueError: unsupported hash type sha512
Traceback (most recent call last):
  File "/usr/local/lib/node_modules/node-gyp/gyp/gyp_main.py", line 18, in <module>
    sys.exit(gyp.script_main())
  File "/usr/local/lib/node_modules/node-gyp/gyp/pylib/gyp/__init__.py", line 534, in script_main
    return main(sys.argv[1:])
  File "/usr/local/lib/node_modules/node-gyp/gyp/pylib/gyp/__init__.py", line 527, in main
    return gyp_main(args)
  File "/usr/local/lib/node_modules/node-gyp/gyp/pylib/gyp/__init__.py", line 503, in gyp_main
    options.circular_check)
  File "/usr/local/lib/node_modules/node-gyp/gyp/pylib/gyp/__init__.py", line 98, in Load
    generator.CalculateVariables(default_variables, params)
  File "/usr/local/lib/node_modules/node-gyp/gyp/pylib/gyp/generator/make.py", line 76, in CalculateVariables
    import gyp.generator.xcode as xcode_generator
  File "/usr/local/lib/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode.py", line 7, in <module>
    import gyp.xcodeproj_file
  File "/usr/local/lib/node_modules/node-gyp/gyp/pylib/gyp/xcodeproj_file.py", line 152, in <module>
    _new_sha1 = hashlib.sha1
AttributeError: 'module' object has no attribute 'sha1'
```
