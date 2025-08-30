## LibMDEC
This library is written for decoding PS1 MDEC images in C#. MDEC version 2 is currently supported.

## How to use
Use function ```MdecImageDecoder``` for decoding image
```
var test_96x96 = MDEC.MdecImageDecoder(File.ReadAllBytes("TEST_96x96.bs"), 96, 96);
var test_320x240 = MDEC.MdecImageDecoder(File.ReadAllBytes("TEST_320x240.bs"), 320, 240);
var test_640x480 = MDEC.MdecImageDecoder(File.ReadAllBytes("TEST_640x480.bs"), 640, 480);
```

## Author
Dedok179
