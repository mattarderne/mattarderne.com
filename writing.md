---
layout: single
title: Writing
excerpt: "Collection of Writing."
exclude: true
---

<!-- <img name="absurd.design" src="/assets/images/ad_blog.png" alt=""/> -->

> I aspire to improve my ability to communicate through writing. This is the workshop. 

## [group by 1](https://groupby1.substack.com/)
My thoughts on modern data analytics systems.  Describe your day-job stuff.

Topics cover the intersection of Data Engineering and Data Analytics. 



## [Matt's World View](https://rdrn.substack.com)

General writing, expanding my understanding of the world. This is very experimental. 

---


# Selected posts 

{% for post in site.posts %}
  {% unless post.exclude %} 
    

## <a href="{{ post.url | relative_url }}" rel="permalink">{{ post.title }}</a>  
<i><time datetime="{{ page.date | date_to_xmlschema }}">{{ post.date | date: "%e %B %Y" }}</time> - {{ post.blog }}  </i>


> <p class="archive-item-excerpt" itemprop="description">{{ post.excerpt | markdownify |  truncate: 250 }}

--- 
  {% endunless %}
{% endfor %}

**All posts will be copied [here](/writing_archive) from Substack in due course.**