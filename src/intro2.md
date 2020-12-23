---
layout: page
title: Intro2
---
<content-box>
  <turbo-frame id="intro" markdown="block">

## Final Bit of Intro'ing

And that's the end of the **intro** panel. 👀

Job well done! 🥳

**[START AGAIN](/)** or **[VISIT ANOTHER PAGE](/about/){:data-turbo-frame="_top"}**


{% capture intro_nav %}
* [1](/){:data-turbo-frame="intro"}
* [2](/intro){:data-turbo-frame="intro"}
* **[3](/intro2){:data-turbo-frame="intro"}**
{:#intro-nav}
{:style="font-size: 1.5em"}
{% endcapture %}

<turbo-stream action="replace" target="intro-nav">
  <template markdown="block">
{{ intro_nav }}
  </template>
</turbo-stream>
  </turbo-frame>
</content-box>

{{ intro_nav }}