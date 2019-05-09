---
layout: docs
title: Tint (FloSports)
description: Add tinted Overlays to content
group: utilities
---

## Example

Add tinted overlays using `*-tint` classes `.bg-tint`, `.btn-tint`, etc

{{< example >}}
  <div class="img-thumbnail position-relative w-50">
    <div class="bg-tint position-absolute top left h-100 w-100 text-white" > overlay </div>
    <img class="img-fluid" src="https://via.placeholder.com/2000"/>
  </div>
{{< /example >}}

## Partial Overlays

Add absolutely positioned partial overlays using `.top` `.right` `.bottom` and `.left`

{{< example >}}
<div class="img-thumbnail position-relative w-50">
  <button class="btn-tint position-absolute top left m-2">Click Me</button>
  <img class="img-fluid" src="https://via.placeholder.com/2000"/>
  <div class="position-absolute d-inline-flex flex-align-start bottom right">
    <i class="text-white bg-primary p-2">|></i>
    <time class="bg-tint text-white h-100 p-2" datetime="PT3H01M58S">3:01:58</time>
  </div>
</div>
{{< /example >}}
