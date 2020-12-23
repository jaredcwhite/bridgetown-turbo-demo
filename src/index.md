---
# Feel free to add content and custom Front Matter to this file.

layout: home
---

A demo of Bridgetown combined with Turbo from the Hotwire project.
{:style="text-align: center"}

<br/>

<content-box>
  <turbo-frame id="intro" markdown="block">

## Turbo Frame Here

This part of the page will update independently of the rest of the page!

It will also use Turbo Streams to replace the below navigation on each step.

**[NEXT](/intro)**


{% capture intro_nav %}
* **[1](/){:data-turbo-frame="intro"}**
* [2](/intro){:data-turbo-frame="intro"}
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