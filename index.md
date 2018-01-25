---
layout: page
----title: portfolio
----[permalink: /portfolio/
---

{% for project in site.portfolio %}
{% assign mod = forloop.index | modulo: 3 %}
    
{% if mod  == 1 %}
<div class="section group">
{% endif %}

        <div class="col span_1_of_3">
	  <div class="container">
            <a class="img__img" href="{{ site.baseurl }}{{ project.url }}">
	    <center>
	      <img class="image" src="{{ project.img }}">
	      {% if  project.title != "TIENDA"  %}
	      <div class="text_underline">
		{% else %}
              <div class="text_underline_tienda">
		{% endif %}
	    	{{ project.title }}
 	      </div>
	      </center>
	      {% if  project.title != "TIENDA"  %}
	      <div class="overlay">
		<div class="text">
		  {{ project.title }}
		  <br/>
		  <div class="text_smaller">
		    {{ project.description }}
		  </div>
		</div>
	      </div>
	      {% endif %}
	    </a>
	  </div>
	</div>
{% if mod == 0 %}
</div>
{% endif %}

{% endfor %}
