<div class="row t60">
	{% if page.widget1_SV.image or page.widget1_SV.video or page.widget1_SV.title %}
		{% include _frontpage-widget.html widget=page.widget1_SV%}
	{% endif %}

	{% if page.widget2_SV.image or page.widget2_SV.video or page.widget2_SV.title %}
		{% include _frontpage-widget.html widget=page.widget2_SV %}
	{% endif %}

	{% if page.widget3_SV.image or page.widget3_SV.video or page.widget3._SVtitle %}
		{% include _frontpage-widget.html widget=page.widget3_SV %}
	{% endif %}
</div><!-- /.row -->

<div>

{% if page.callforaction_SV.url contains 'http' %}
{% assign url = '' %}
{% else %}
{% capture url %}{{ site.url }}{{ site.baseurl }}{% endcapture %}
{% endif %}
{% if page.callforaction_SV %}
    <div class="row t60 b60">
        <div class="small-12 text-center columns">
            <a class="button large radius {{ page.callforaction_SV.style }}" href="{{ url }}{{ page.callforaction_SV.url }}"{% if page.callforaction_SV.url contains 'http' %} target="_blank" {% endif %}>{{ page.callforaction_SV.text }}</a>
        </div><!-- /.small-12.columns -->
    </div><!-- /.row -->
{% endif %}
</div>


