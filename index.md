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
              
        <p>
          {{ post.summary }}
        </p>
                
    <h4><strong><a href="{{ post.url }}">View more...</a></strong></h4> 
      </div>
    </div>    
        <hr>
  </div>
</div>
  {% endfor %}
</div>
