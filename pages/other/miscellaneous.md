---
layout: default
title: Miscellaneous
permalink: /miscellaneous/
nav_order: 99
# has_children: true
has_toc: false
---

The content on this page is for testing purposes only.




<p class="note-title">
  This is a note
</p>

<p class="highlight">
  This is a note
</p>

<p>Code Example</p>

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
dateformat.i18n = require('./lang/' + l)
return true;
}
```

{% capture some_var %}
{% highlight some_language linenos %}
Some code
{% endhighlight %}
{% endcapture %}
{% include fix_linenos.html code=some_var %}

<p>Graph Example</p>

```mermaid
flowchart LR
A["Arr#91;0#93; "] --- B["Arr#91;1#93; "]
```
{: .bg-white }

site.url: {{ site.url }}

link: {% link /assets/images/data-structures/java-collection-graph.png %} 

page.url: {{ page.url }} <-- <code><i>specified by permalink</i></code>

page.path: {{ page.path }}

{% assign my_array = '' | split: '' %}
{% for page in site.pages %}

{% if page.parent == "Data Structures" %}

{% assign my_array = my_array | append: ', ' | append: page.title  %}

{% endif %}
{% endfor %}