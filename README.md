## Edit Google Spreadsheet

> A simple API for reading and writing Google Spreadsheets in Node.js based on https://github.com/jpillora/node-edit-google-spreadsheet.


#### List all worksheets
``` js
  Spreadsheet.list({
    debug: true,
    spreadsheetName: 'node-edit-spreadsheet',
    worksheetName: 'Sheet1',
    // Choose from 1 of the 3 authentication methods:
    //    1. Username and Password
    username: 'my-name@google.email.com',
    password: 'my-5uper-t0p-secret-password',
    // OR 2. OAuth
    oauth : {
      email: 'my-name@google.email.com',
      keyFile: 'my-private-key.pem'
    },
    // OR 3. Token
    accessToken : {
      type: 'Bearer',
      token: 'my-generated-token'
    }
  }, function sheetReady(err, worksheets) {
    // ...
  });
````

#### MIT License

Copyright © 2014 Jaime Pillora &lt;dev@jpillora.com&gt;

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
