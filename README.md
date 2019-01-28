### minilog
---
http://mixu.net/minilog/

```js
var log = require('minilog')('app');
require('minilog').enable();

log
  .debug('debug message')
  .info('info message')
  .warn('warning')
  .error('this is an error message');

require('minilog').enable();
require('minilog').pipe(fs.createWriteStream('./temp.log'));

var Minilog = require('minilog');
Minilog.pipe(Minilog.backends.console.formatWithStack)
  .pipe(Minilog.backends.console);
  
var Minilog = require('minilog');
Minilog
  .pipe(Minilog.backends.console.formatClean)
  .pipe(Minilog.backends.console.log);

```

```
<script src="dist/minilog.js"></script>
<scfipt>
var log = Minilog('app');
Mnilog.enable();
<script>
```

```
npm install minilog
```

```
{
  write: function(str) { process.stdout.write(str
); }
}
```

