minty-mocha
===========

This is a cheaper alternative module of mocha to get colored test results on mintty (or a git bash for Windows).
On the mintty, the `mocha` does work, but the text is not colored.

If `describe` and `it` functions are not exist in global,
this module creates alternatives.
If both of those are exist, this module do nothing.
So anyhow, this module does not export anything

This module might not work well on the other environment.

USAGE
-----

Simply, only require.

```
(function() {
    "use strict";
    require("minty-mocha");
    var chai = require('chai');
    var should = chai.should();
    var assert = chai.assert;

    describe("foo in bar", function() {
        describe("baz will boo", function() {
            it('should returns zero', function() {
                assert.equal(bar.foo.baz.boo(), 0);
            });
        });
        describe("there is no boo", function() {
            it('should ...
```

LICENSE
-------

[MIT](LICENSE)
