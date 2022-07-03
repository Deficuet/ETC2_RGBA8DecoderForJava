# ETC2_RGBA8DecoderForJava
Decode the image data of Unity Texture2D with texture compression uncrunched ETC2_RGBA8

The code is rewrited from [AssetStudio/Texture2DDecoderNative/etc.cpp](https://github.com/Perfare/AssetStudio/blob/master/Texture2DDecoderNative/etc.cpp)
## How to use
The function `decodeETC2A8` in class `ETCDecoder`
```java
public static void decodeETC2A8(byte[] data, final int width, final int height, byte[] out)
```
`data` - image data of Texture2D object read from assetbundle

`width` `height` - `m_width` and `m_height` property of Texture2D object

`out` - output byte array. Its size should always be width * height * 4

**The color channel of the output data is BGRA**
