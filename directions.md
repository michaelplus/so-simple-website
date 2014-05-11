---
layout: page
permalink: /directions/
title: Directions
tags: [Directions]
modified: 2014-05-10
image:
  feature: smallmaps.png
  credit: Screenshot from Google Maps by Michael Murphy
  creditlink: http://maps.google.com?q=9300B Old Keene Mill Road, Buke Virginia
locations:
  9300B Old Keene Mill Road, Burke Virginia
---

{% if page.locations %}
# Address:
<a href="https://www.google.com/maps?q={% for location in page.locations %}{% if forloop.first %}{{location}}{% endif %}{% endfor %}">{% for location in page.locations %}{% if forloop.first %}{{location}}{% endif %}{% endfor %}
<img src="http://maps.googleapis.com/maps/api/staticmap?{% for location in page.locations %}{% if forloop.first %}center={{location}}&markers=color:blue%7C{{location}}{% else %}&markers=color:blue%7C{{location}}{% endif %}{% endfor %}&zoom={% if page.zoom %}{{page.zoom}}{% else %}13{% endif %}&size=400x300&scale=2&sensor=false&visual_refresh=true" alt=""></a>
{% endif %}

### GPS Users Warning:

Please note that there is no entrance on Shiplett Road to our office complex, Rolling Valley Office Park. The only entrance is at the light on Old Keene Mill Road just north of Sydenstricker Road. Also, if you are traveling north on Sydenstricker from the Fairfax County Parkway, do not turn off of Sydenstricker. Sydenstricker Road dead-ends into our office park.

### So Simple Theme is all about:

* Responsive templates. Looking good on mobile, tablet, and desktop.
* Gracefully degrading in older browsers. Compatible with Internet Explorer 9+ and all modern browsers.
* Minimal embellishments and subtle animations. 
* Readable typography to make your words shine.
* Support for large images to call out your favorite posts.
* Disqus comments if you choose to enable.
* Simple and clear permalink structure[^1].
* Tags for [Open Graph](https://developers.facebook.com/docs/opengraph/) and [Twitter Cards](https://dev.twitter.com/docs/cards) for a better social sharing experience.
* Vanilla [custom 404 page]({{ site.url }}/404.html) to get you started.
* Stylesheets for Pygments and Coderay [syntax highlighting](http://mmistakes.github.io/articles/so-simple-theme/code-highlighting-post/) to make your code examples look snazzy.
* Simple search that overlays results based on post title.
* [Grunt build script]({{ site.url }}/theme-setup/index.html#theme-development) for easier theme development.
* [Sitemap](https://github.com/mmistakes/so-simple-theme/blob/master/sitemap.xml) for search engines

<a markdown="0" href="{{ site.url }}/theme-setup" class="btn">Install Minimal Mistakes Theme</a>

[^1]: Example: *domain.com/category-name/post-title*