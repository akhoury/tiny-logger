tiny-logger
===========

a 120 seconds, light weight, tiny logger with basic log levels

### Usage
```
var logger = require('tiny-logger').init('debug,warn,error', '[my-prefix]');

logger.debug('something debug');
// [my-prefix][debug] something debug

logger.warn('something warn');
// [my-prefix][warn] something warn

logger.info('something info');
// won't print since it's not included in the level argument

logger.error('something to error');
// [my-prefix][error] something debug

// or without a prefix, or a tag
// you can use the usual console.log arguments here
// i tend to never do
logger.log('free style');
// free style

```
