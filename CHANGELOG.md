## version 3.0.1: 2013-01-28

  * Fix #13: don't call the constructor when making the new prototype.

## version 3.0.0: 2013-01-18

  * Introduce `MyClass.Bare` as a way of allocating uninitialized
    instances
  * Created classes will now create instances in exactly the same way
    no matter what the calling context.  In particular this means
    `new` works as expected:

``` js
new MyClass(1, 2) // calls MyClass::init with arguments (1, 2)
```

## version 2.0.2: 2013-01-17

  * Started a CHANGELOG
  * Removed support for the `.fn` property which was buggy and unused
  * Down to 525 bytes minified
