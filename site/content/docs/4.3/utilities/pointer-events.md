---
layout: docs
title: Pointer events
description: Control pointer-events
group: utilities
---

Set the `pointer-events` of elements with utilities. Useful in combination with `.visible` and `.invisible` for controlling clickability when creating transions and animations

Apply `.pointer-events-all` or `.pointer-events-none` as needed.

{{< highlight html >}}
<div class="pointer-events-all">...</div>
<div class="pointer-events-none">...</div>
{{< /highlight >}}

{{< highlight scss >}}
// Class
.pointer-events-all {
  pointer-events: all;
}
.pointer-events-none {
  pointer-events: none;
}
{{< /highlight >}}
