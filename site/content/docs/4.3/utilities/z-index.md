---
layout: docs
title: Z-index (FloSports)
description: Control the z-index of elements with utility classes.
group: utilities
---

Set the `z-index` of elements with our z-index utilities. It is generally
recommended that these classes be used sparingly in applications as they create
new **[stacking contexts][1]** which can lead to difficult situations in complex
apps; restructuring html is usually prefered

Apply `.z-$value`


{{< highlight html >}}
<div class="z-hover">...</div>
<div class="z-focus">...</div>
<div class="z-active">...</div>
<div class="z-dropdown">...</div>
<div class="z-sticky">...</div>
<div class="z-fixed">...</div>
<div class="z-modal-backdrop">...</div>
<div class="z-modal">...</div>
<div class="z-popover">...</div>
<div class="z-tooltip">...</div>
{{< /highlight >}}

{{< highlight scss >}}

$zindecies: () !default;
// stylelint-disable-next-line scss/dollar-variable-default
$zindecies: map-merge(
  (
    "hover":   $zindex-hover,
    "focus":     $zindex-focus,
    "active":     $zindex-active,
    "dropdown":   $zindex-dropdown,
    "sticky":     $zindex-sticky,
    "fixed":     $zindex-fixed,
    "modal-backdrop":       $zindex-modal-backdrop,
    "modal":        $zindex-modal,
    "popover":     $zindex-popover,
    "tooltip":     $zindex-tooltip,
  ),
  $zindecies
);

@each $index, $value in $zindecies {
  .z-#{$index} {
    z-index: $value;
  }
}
{{< /highlight >}}


[1]:https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Positioning/Understanding_z_index/The_stacking_context
