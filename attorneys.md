---
layout: default
title: About Jennifer
---

# About Jennifer
<div class="card-deck">
	{% for attorney in site.data.attorneys %}
		  <div class="card my-3" style="min-width: 30%;">
		    	<img src="assets/images/{{ attorney.picture }}" class="card-img" alt="..." style="min-width:30%;max-width:30%">
		  		<div class="card-body">
		  			<h5 class="card-title">{{ attorney.name }}</h5>
		  			<p class="card-text">{{ attorney.bio }}</p>
		  		</div>
				<ul class="list-group list-group-flush">
				    <li class="list-group-item">Email: <a href="mailto:{{ attorney.email }}">{{ attorney.email }}</a></li>
				    <li class="list-group-item">Call: {{ attorney.phone }}</li>
				</ul>
		  </div>
	{% endfor %}
</div>	
