---
layout: docs
title: Tooltips (FloSports)
description: Documentation and examples for adding custom FloSports tooltips with CSS
group: components
toc: true
---

Style tooltips with `.tooltip.tooltip-top`, `.tooltip.tooltip-right`, andy `.tooltip.tooltip-bottom`. Left tooltips are currently unsupported.

## Example

`.tooltip.tooltip-top`
{{< example >}}
<button type="button" class="btn btn-primary">Click Me</button>
<div class="tooltip tooltip-top">Tooltip</div>
{{< /example >}}

`.tooltip.tooltip-right`
{{< example >}}
<button type="button" class="btn btn-primary">Click Me</button>
<div class="tooltip tooltip-right">Tooltip</div>
{{< /example >}}

`.tooltip.tooltip-bottom`
{{< example >}}
<button type="button" class="btn btn-primary">Click Me</button>
<div class="tooltip tooltip-bottom">Tooltip</div>
{{< /example >}}



## Hover and click

Combine tooltips with `.hover-*` or `.click-*` classes to control display. Note the use of `*-inline` for left side tooltips

Hover

{{< example >}}
<button type="button" class="btn btn-primary hover-target">Hover Me</button>
<div class="tooltip tooltip-top hover-toggle-block">Tooltip</div>
{{< /example >}}

{{< example >}}
<button type="button" class="btn btn-primary hover-target">Hover Me</button>
<div class="tooltip tooltip-right hover-toggle-inline">Tooltip</div>
{{< /example >}}

{{< example >}}
<button type="button" class="btn btn-primary hover-target">Hover Me</button>
<div class="tooltip tooltip-bottom hover-toggle-block w-50">Tooltip with image
  <img class="img-fluid" src="https://via.placeholder.com/1000"/>
</div>
{{< /example >}}

Click

{{< example >}}
<label for="click-toggle-input-top" type="button" class="btn btn-primary">Click Me</label>
<input class="click-toggle-input d-none" type="checkbox" id="click-toggle-input-top">
<div class="tooltip tooltip-top click-toggle-block">Tooltip</div>
{{< /example >}}

{{< example >}}
<label for="click-toggle-input-right" type="button" class="btn btn-primary">Click Me</label>
<input class="click-toggle-input d-none" type="checkbox" id="click-toggle-input-right">
<div class="tooltip tooltip-right click-toggle-inline">Tooltip</div>
{{< /example >}}

{{< example >}}
<label for="click-toggle-input-bottom" type="button" class="btn btn-primary">Click Me</label>
<input class="click-toggle-input d-none" type="checkbox" id="click-toggle-input-bottom">
<div class="tooltip tooltip-bottom click-toggle-block">Tooltip</div>
{{< /example >}}
