---
title: DocumentSizeAutoDetect element
description: The optional DocumentSizeAutoDetect element specifies whether the scan device automatically determines the size of the original scan media.
MS-HAID:
- 'wsdss\_doc\_b097765c-8c40-4aaf-8bb6-cf121230c15e.xml'
- 'image.documentsizeautodetect'
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 509e96d8-c99b-4d6e-9117-b9aed199da2c
keywords: ["DocumentSizeAutoDetect element Imaging Devices"]
topic_type:
- apiref
api_name:
- wscn DocumentSizeAutoDetect
api_type:
- Schema
---

# DocumentSizeAutoDetect element


The optional **DocumentSizeAutoDetect** element specifies whether the scan device automatically determines the size of the original scan media.

Usage
-----

``` syntax
<wscn:DocumentSizeAutoDetect>
  text
</wscn:DocumentSizeAutoDetect>
```

Attributes
----------

There are no attributes.

Text value
----------

Required. A Boolean value that must be 0, false, 1, or true.**falsetrue**

## Child elements


There are no child elements.

## Parent elements


<table>
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th>Element</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>[<strong>InputSize</strong>](inputsize.md)</p></td>
</tr>
</tbody>
</table>

Remarks
-------

If the specified text value is 1 or **true**, the scan device will automatically determine the size of the original scan media. If the **DocumentSizeAutoDetect** element is specified along with a [**ScanRegion**](scanregion.md) element, the scan region will be ignored if it falls outside of the media size that the device detected.

## <span id="see_also"></span>See also


[**ScanRegion**](scanregion.md)

[**InputSize**](inputsize.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bimage\image%5D:%20DocumentSizeAutoDetect%20element%20%20RELEASE:%20%2811/8/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




