# CanYouSee

## Description
How about some hide and seek?
Download this file [here](https://artifacts.picoctf.net/c_titan/5/unknown.zip).

## inspection 

* we hava a simple jpg in the zip file 

![alt text](ukn_reality.jpg)

* we just run exiif tools on linux 

``` bash
                                                                                                  
┌──(kali㉿kali)-[~/Desktop]
└─$ exiftool ./ukn_reality.jpg 
ExifTool Version Number         : 13.00
File Name                       : ukn_reality.jpg
Directory                       : .
File Size                       : 2.3 MB
File Modification Date/Time     : 2024:02:15 17:40:17-05:00
File Access Date/Time           : 2025:03:16 04:11:35-04:00
File Inode Change Date/Time     : 2025:03:16 04:11:35-04:00
File Permissions                : -rw-r--r--
File Type                       : JPEG
File Type Extension             : jpg
MIME Type                       : image/jpeg
JFIF Version                    : 1.01
Resolution Unit                 : inches
X Resolution                    : 72
Y Resolution                    : 72
XMP Toolkit                     : Image::ExifTool 11.88
Attribution URL                 : cGljb0NURntNRTc0RDQ3QV9ISUREM05fNGRhYmRkY2J9Cg==
Image Width                     : 4308
Image Height                    : 2875
Encoding Process                : Baseline DCT, Huffman coding
Bits Per Sample                 : 8
Color Components                : 3
Y Cb Cr Sub Sampling            : YCbCr4:2:0 (2 2)
Image Size                      : 4308x2875
Megapixels                      : 12.4

```

* we can see a base64 string (denoted by the == at the end)
* go to any online [base64 decoder](https://www.base64decode.org/) and convert it to get the flag

