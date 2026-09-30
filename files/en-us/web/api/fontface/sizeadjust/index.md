---
title: "FontFace: sizeAdjust property"
short-title: sizeAdjust
slug: Web/API/FontFace/sizeAdjust
page-type: web-api-instance-property
browser-compat: api.FontFace.sizeAdjust
---

{{APIRef("CSS Font Loading API")}}{{AvailableInWorkers}}

The **`sizeAdjust`** property of the {{domxref("FontFace")}} interface returns and sets a multiplier for the glyph outlines and metrics associated with the font.

This property is equivalent to the {{cssxref("@font-face/size-adjust")}} descriptor of {{cssxref("@font-face")}}.

## Value

A string containing a non-negative percentage. The default value is `100%`.

This property accepts the same values as the {{cssxref("@font-face/size-adjust")}} descriptor.

## Examples

### Setting the size adjustment of a font

This example creates a font face with a size adjustment of `90%`, then changes it to `95%`.

```js
const fontFace = new FontFace("my-font", 'url("my-font.woff")', {
  sizeAdjust: "90%",
});
console.log(fontFace.sizeAdjust); // "90%"

fontFace.sizeAdjust = "95%";
console.log(fontFace.sizeAdjust); // "95%"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- {{cssxref("@font-face/size-adjust")}}
