---
layout: default
description: "Recomapp's Blog"
id: home
---

<div class="hero">
  <div class="hero-inner">
    <img class="hero-logo" src="/img/recomapp_256x256.png" alt="">
    <h1>{{ site.title }}</h1>
    <p>{{ site.description }}</p>
  </div>
</div>


<div class="articles">
	<div class="articles-inner">
		<h2>Articles</h2>
		<ul>
      {% for article in site.categories.articles %}
				<li>
					<a href="{{ article.url }}"> {{ article.title }}</a>
				</li>
			{% endfor %}
		</ul>
	</div>
</div>
