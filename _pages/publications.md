---
title: "Publications"
permalink: /publications/
layout: single
author_profile: true
---
You can also find my publications on [Google Scholar](https://scholar.google.com/citations?user=Cb6W6tgAAAAJ&hl=en).

<h4 style="margin-bottom:0px;padding-top:10px;">Preprints</h4>
<ul class="preprint_list">

{% assign number_printed = 0 %}
{% for publi in site.data.publication_list %}
{% if publi.type == "preprint" %}

<li ><p>
<b>{{ publi.title }}</b> ({{ publi.year }})
<br>{{ publi.authors }}<br>
<a href="javascript:toggleBibtex('{{ publi.label }}')">[BibTeX]</a>
<a href="{{ publi.link_pre.url }}" target="_blank">[PDF]</a> 
</p>
<div id="bib_{{ publi.label }}" class="bibtex noshow">
<pre>
{{ publi.bibtex }}
</pre>
</div>
</li>

{% endif %}
{% endfor %}

</ul>

<h4 style="margin-bottom:0px;padding-top:10px;">Journal and Conference Publications</h4>
<!-- Generated from JabRef by PubList by Truong Nghiem at 11:44 on 2015.09.10. -->
<ul class="biblist">

{% assign number_printed = 0 %}
{% for publi in site.data.publication_list %}
{% if publi.type == "journal" %}

<li ><p>
<b>{{ publi.title }}</b> ({{ publi.year }})
<br>{{ publi.authors }}<br>
<i>{{ publi.link_main.display }}, <a href="{{ publi.link_main.url }}" target="_blank">[Link]</a></i>
<br>
<a href="javascript:toggleBibtex('{{ publi.label }}')">[BibTeX]</a>
<a href="{{ publi.link_pre.url }}" target="_blank">[PDF]</a> 
</p>
<div id="bib_{{ publi.label }}" class="bibtex noshow">
<pre>
{{ publi.bibtex }}
</pre>
</div>
</li>

{% endif %}
{% endfor %}

</ul>

<h4 style="margin-bottom:0px;padding-top:10px;">Books and Edited Volumes</h4>
<!-- Generated from JabRef by PubList by Truong Nghiem at 11:44 on 2015.09.10. -->
<ul class="biblist">

{% assign number_printed = 0 %}
{% for publi in site.data.publication_list %}
{% if publi.type == "book" %}

<li ><p>
<b>{{ publi.title }}</b> ({{ publi.year }})
<br>{{ publi.authors }}<br>
<i>{{ publi.link_main.display }}, <a href="{{ publi.link_main.url }}" target="_blank">[Link]</a></i>
<br>
<a href="javascript:toggleBibtex('{{ publi.label }}')">[BibTeX]</a>
<a href="{{ publi.link_pre.url }}" target="_blank">[PDF]</a> 
</p>
<div id="bib_{{ publi.label }}" class="bibtex noshow">
<pre>
{{ publi.bibtex }}
</pre>
</div>
</li>

{% endif %}
{% endfor %}

</ul>