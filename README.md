## LibMDEC
This library is written for decoding PS1 MDEC images in C#. MDEC version 2 is currently supported.

## How to use
Use function ```MdecImageDecoder``` for decoding image
```
var test_96x96 = MDEC.MdecImageDecoder(File.ReadAllBytes("TEST_96x96.bs"), 96, 96);
var test_320x240 = MDEC.MdecImageDecoder(File.ReadAllBytes("TEST_320x240.bs"), 320, 240);
var test_640x480 = MDEC.MdecImageDecoder(File.ReadAllBytes("TEST_640x480.bs"), 640, 480);
```

Use function ```SaveAsJpg``` for save decoded data as .jpg image
```
MDEC.SaveAsJpg(test_96x96, "TEST_96x96");
MDEC.SaveAsJpg(test_320x240, "TEST_320x240");
MDEC.SaveAsJpg(test_640x480, "TEST_640x480");
```
![alt text](https://github.com/Dedok179/LibMDEC/blob/main/TEST_96x96.jpg?raw=true) ![alt text](https://github.com/Dedok179/LibMDEC/blob/main/TEST_320x240.jpg?raw=true)

Use function ```GetPreviewImage``` for get ```Bitmap``` data
```
MDEC.GetPreviewImage(test_96x96).Save("TEST_96x96.png", System.Drawing.Imaging.ImageFormat.Png);
MDEC.GetPreviewImage(test_320x240).Save("TEST_320x240.png", System.Drawing.Imaging.ImageFormat.Png);
MDEC.GetPreviewImage(test_640x480).Save("TEST_640x480.png", System.Drawing.Imaging.ImageFormat.Png);
```

## TODO
Implement encoding image data to MDEC image

## Author
Dedok179
