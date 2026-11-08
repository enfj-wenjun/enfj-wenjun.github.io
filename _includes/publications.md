<h2 id="publications" style="margin: 2px 0 12px;">Working Papers</h2>

<div class="publications" style="margin-top: 0;">
<ol class="bibliography" style="margin: 0; padding: 0; list-style: none;">

{% for link in site.data.publications.main %}

<li style="min-height: 0; margin: 0 0 24px; padding: 0;">

  <div class="title">
    <a href="{{ link.pdf | relative_url }}">{{ link.title }}</a>
  </div>

  <div class="author">{{ link.authors }}</div>

  {% if link.conference %}
  <div class="periodical">
    <em>{{ link.conference }}</em>
  </div>
  {% endif %}

  <div class="links">
    {% if link.code %}
    <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
    {% endif %}
    {% if link.page %}
    <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
    {% endif %}
    {% if link.bibtex %}
    <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
    {% endif %}
    {% if link.notes %}
    <strong><i style="color:#e74d3c">{{ link.notes }}</i></strong>
    {% endif %}
    {% if link.others %}
    {{ link.others }}
    {% endif %}
  </div>

</li>

{% endfor %}

</ol>
</div>
