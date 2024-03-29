# Usage

```typescript
import { printHRTime } from "print-hrtime";

const start = process.hrtime();
// do stuff
const end = process.hrtime(start);

const words = prettyHrtime(end);
console.log(words); // '1.2 ms'

words = prettyHrtime(end, { verbose: true });
console.log(words); // '1 millisecond 209 microseconds'

words = prettyHrtime(end, { precise: true });
console.log(words); // '1.20958 ms'
```

## Credits

This is an adaptation of the package [pretty-hrtime] (https://github.com/robrich/pretty-hrtime) rewritten in typescript.

## LICENSE

(MIT License)

Copyright (c) 2013 [Richardson & Sons, LLC](http://richardsonandsons.com/)

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
