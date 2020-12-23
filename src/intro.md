---
layout: page
title: Intro
---
<content-box>
  <turbo-frame id="intro" markdown="block">
## Second Intro Panel

Yay, I'm in a Turbo Frame!

Under the hood, this is just another Bridgetown page. Everything still "works" even with Javascript disabled! 😎

**[NEXT](/intro2)**


{% capture intro_nav %}
* [1](/){:data-turbo-frame="intro"}
* **[2](/intro){:data-turbo-frame="intro"}**
* [3](/intro2){:data-turbo-frame="intro"}
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