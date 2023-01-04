---
layout: default
title: Off-Topic / Curiosities (?)
permalink: /off-topic/
nav_order: 98
# has_children: true
has_toc: false
---

<p class="l-font">
    <i>03/01/23</i><br>
    I just discovered that I can use <code>html Emmet abreviations</code> on Markdown 
    documents changing the extension settings. It saves me <span class="fw-700">A LOT</span> of time 
    (Good luck formatting the <code>markdown</code> document tho 💀).

<br>
This is my <code>settings.json</code> of VSC and works pretty neat:
</p>

{% capture some_var %}
{% highlight json linenos %}
{
    "files.autoSave": "afterDelay",
    "explorer.confirmDelete": false,
    "editor.minimap.enabled": false,
    "emmet.excludeLanguages": [],
    "emmet.includeLanguages": { "markdown": "html" },
    "emmet.triggerExpansionOnTab": true,
    "[markdown]": {
        "editor.quickSuggestions": {
            "comments": "on",
            "strings": "on",
            "other": "on"
        }
    }
}
{% endhighlight %}
{% endcapture %}
{% include fix_linenos.html code=some_var %}

<div style="text-align:right;" class="l-font">
<a href="https://stackoverflow.com/questions/49956963/markdown-not-using-emmet" target="_blank">
🌠 Reference.
</a>
</div>

---



<!--  article template:

<p class="l-font">
    <i>day/month/year</i><br>
    ...
</p>
<div style="text-align:right;" class="l-font">
<a href="" target="_blank">
🌠 Reference.
</a>
</div>

---

 -->