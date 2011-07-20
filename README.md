# Synopsis

### This is an experiment using node child processes to create a lightweight dynamic HTTP server

# Usage
Start up http-dynamic
```bash
		./lib/http-dynamic
```
Add scripts (any language) to the scripts directory
```php
<?php
  echo 'hello from php'."\n";
  echo 'arguments are '.$argv[1]."\n";
  exit();
?>
```

Make a HTTP request for that script
		curl localhost:8080/hello.php?foo=bar
		'hello from php
		arguments are foo=bar'
		
# Licence

(The MIT License)

Copyright (c) 2010 mkrecny <http://www.twitter.com/mkrecny>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
