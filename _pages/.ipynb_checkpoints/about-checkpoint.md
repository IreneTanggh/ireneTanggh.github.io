---
layout: page
permalink: /
title: about
nav: about
---

<div class="col p-0 pt-4 pb-4">
  <h1 class="pb-3 title text-left font-weight-bold">Xuxin Tang</h1>
  <h6 class="m-0 mb-2" style="font-size: 0.83em;">{{ page.description }}</h6>
  {% if page.address %}
      <h6 class="m-0 mb-2" style="font-size: 0.83em;">{{ page.address }}</h6>
  {% endif %}
</div>

<!-- Introduction -->

<div style="display: flex; flex-wrap: wrap;">
    <div class="text-justify p-0">
        <div class="col-xs-12 col-sm-6 p-0 pt-2 pb-sm-2 pb-4 pl-sm-4 text-center" style="float: right;">
          <img class="profile-img img-responsive" src="{{ 'prof_pic.jpg' | prepend: '/assets/img/' | prepend: site.baseurl | prepend: site.url }}">
        </div>

        <p>
            I received my master and bachelor degree at <a href="https://www.whu.edu.cn/" target="_blank">Wuhan University</a> co-advised by Prof. Zhijiang Li and <a href="http://www.mit.edu/~f_zhang/" target="_blank">Prof. Fan Zhang</a>. 
        </p>
        
        <p>
            I have a great passion for studying on big data concerning fields, including data analytics, data visualization, artificial intelligence and human AI/data interaction. <br />
        </p>
        <p>
            I have nearly 3-year industry experience. At most time I worked as a recommendation algorithm engineer for YY Live, Chinese top 1 live broadcasting company. The job duty is deciding which real-time contents are delivered to customers, composed of building models, daily data analytics and data visualization.
            </p>
        <p>
            My master research mainly focused on cloud computing, auto-scaling container and image processing. The thesis of container has some cites. Additionally, because of my personal interests, I also participated in and got good rankings in some AI competitions.<br/>
        </p>
    </div>
</div>

<!-- Selected publications -->
<div class="news mt-3 p-0">
  <h1 class="title mb-4 p-0">selected publications</h1>
  {% bibliography -f papers -q @*[selected=true]* %}
</div>

