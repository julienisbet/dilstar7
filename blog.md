---
title: dilstar7_blog
layout: default
---
 <div class="myposts">
  {% for post in site.posts %}     
    <div class="post">
      <img class="blogimage" src="images/{{post.image}}"/>
      <div class="blogcontent"> 
        <span class="title">{{ post.title}}</span>     
        <span class="postDate">{{ post.date | date: "%b %-d, %Y" }}
        </span> 
        <div class="copy">
        {{post.content}}   
        </div>
      </div>
    </div> 
  {% endfor %}
 </div>
