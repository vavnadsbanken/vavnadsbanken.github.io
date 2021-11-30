<div class="row t60">
	{% if page.widget1_EN.image or page.widget1_EN.video or page.widget1_EN.title %}
		{% include _frontpage-widget.html widget=page.widget1_EN%}
	{% endif %}

	{% if page.widget2_EN.image or page.widget2_EN.video or page.widget2_EN.title %}
		{% include _frontpage-widget.html widget=page.widget2_EN %}
	{% endif %}

	{% if page.widget3_EN.image or page.widget3_EN.video or page.widget3._ENtitle %}
		{% include _frontpage-widget.html widget=page.widget3_EN %}
	{% endif %}
</div><!-- /.row -->


<div>

{% if page.callforaction_EN.url contains 'http' %}
{% assign url = '' %}
{% else %}
{% capture url %}{{ site.url }}{{ site.baseurl }}{% endcapture %}
{% endif %}
{% if page.callforaction_EN %}
    <div class="row t60 b60">
        <div class="small-12 text-center columns">
            <a class="button large radius {{ page.callforaction_EN.style }}" href="{{ url }}{{ page.callforaction_EN.url }}"{% if page.callforaction_EN.url contains 'http' %} target="_blank" {% endif %}>{{ page.callforaction_EN.text }}</a>
        </div><!-- /.small-12.columns -->
    </div><!-- /.row -->
{% endif %}
</div>
