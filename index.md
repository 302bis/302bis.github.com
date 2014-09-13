---
layout: page
title: 302bis
tagline: Freelance Web Designer. I like to create websites prioritizing usability and minimalism.
---
{% include JB/setup %}

<div class="posts">
  {% for post in site.posts %}

<div class="">
  <div class="">    
    <div class="row">
      <div class="col-lg-12 ">
                <h4><strong><a href="{{ post.url }}">{{ post.title }}</a></strong></h4>      
        <p>
          {{ post.summary }}
        </p>
                <p> {{ post.date | date: "%B %e, %Y" }}<a href="http://erjjones.github.com{{ post.url }}#disqus_thread" data-disqus-identifier="{{ post.url }}"></a>     
                  | Tags :{% for tag in post.tags %} <a href="/tags/{{ tag }}" rel="tooltip" title="View posts tagged with &quot;{{ tag }}&quot;"><span class="label label-info">{{ tag }}</span></a>  {% if forloop.last != true %} {% endif %} {% endfor %}                            
        </p>
    
      </div>
    </div>    
        <hr>
  </div>
</div>
  {% endfor %}
</div>
