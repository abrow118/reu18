---
layout: default
title: "CSAFE @ ISU REU"
css: "/css/index.css"
---

## Homework 

Date Assigned | What | Date Due | Solution (if applicable)  
:-------------|------|:-------- | ---:
6/5/18        | Ch. 1 problems 2, 4, 11, 14, 16, 20, 22, 26, 30, 32, 34, 40, 44, 52, 54, 66, 70a-c. Do all parts unless otherwise stated | 6/8/2018 @ 4:00pm | [Solution](static/homework/soln-assn-1.html)
6/14/18    | Ch. 2 problems 8a, 8c-f, 14, 16, 18, 22, 26, 34, 38. Do all parts unless otherwise stated. Use a .Rmd to write the homework. | 6/18/2018 @ 4:00pm | [Solution](static/homework/soln-assn-2.html)
6/19/18 | Ch. 3 problems 4, 6, 8, 16, 26, 28, 32, 44. Do all parts. Turn in a .pdf file that you compiled from a .Rmd | Due 6/22/18 @ 9:00am 





<div class="list-filters">
  <a href="/reu17" class="list-filter">All posts</a>
  <a href="/reu17/assignments" class="list-filter filter-selected">Assignments</a>
  <a href="/reu17/week1" class="list-filter">Week1</a>
  <a href="/reu17/week2" class="list-filter">Week2</a>
  <a href="/reu17/week3" class="list-filter">Week3</a>
  <a href="/reu17/week4" class="list-filter">Week4</a>
  <a href="/reu17/week5" class="list-filter">Week5</a>
  <a href="/reu17/week6" class="list-filter">Week6</a>
  <a href="/reu17/week7" class="list-filter">Week7</a>
</div>

<div class="posts-list">
  {% for post in site.tags.assignments %}
  <article>
    <a class="post-preview" href="{{ post.url | prepend: site.baseurl }}">
	    <h2 class="post-title">{{ post.title }}</h2>
	
	    {% if post.subtitle %}
	    <h3 class="post-subtitle">
	      {{ post.subtitle }}
	    </h3>
	    {% endif %}
      <p class="post-meta">
        Posted on {{ post.date | date: "%B %-d, %Y" }}
      </p>

      <div class="post-entry">
        {{ post.content | truncatewords: 50 | strip_html | xml_escape}}
        <span href="{{ post.url | prepend: site.baseurl }}" class="post-read-more">[Read&nbsp;More]</span>
      </div>
    </a>  
   </article>
  {% endfor %}
</div>