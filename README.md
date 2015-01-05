# Apache Thrift BinaryPorotocol for JavaScript

An implementation of TBinaryProtocol for JavaScript Thrift library.

## Why not part of Thrift?

The reason is described here: https://github.com/apache/thrift/pull/345.

## Running tests

Tests require the `thrift.js` file to be placed in the the `test/deps` directory. The easiest way to obtain this file is to clone the [Thrift repository](https://github.com/apache/thrift) and copy the file from `lib/js/src/thrift.js` to deps folder. Then simply open the `test-binary.html` in the browser.

## Usage

`Thrift.BinaryProtocol` depends on `thrift` library being present.

    <script src="thrift.js"></script>
    <script src="thrift-binary-protocol.js"></script>
    <script>
      var transport = new Thrift.Transport("/dummy");
      var protocol  = new Thrift.BinaryProtocol(transport);
      ...
    </script>

All methods of the standard `TBinaryProtocol` are implemented.

## License

The MIT License (MIT)

Copyright (c) 2015 Radoslaw Gruchalski <radek@gruchalski.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
