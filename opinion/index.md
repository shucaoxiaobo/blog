---
layout: home
---

<div class="index-content opinion">
    <div class="section">
        <ul class="artical-cate">
            <li><a href="/Blog"><span>Blog</span></a></li>
            <li class="on" style="text-align:center"><a href="/Blog/opinion"><span>DevelopNote</span></a></li>
            <li style="text-align:right"><a href="/Blog/project"><span>Project</span></a></li>
        </ul>

        <div class="cate-bar"><span id="cateBar"></span></div>

        <ul class="artical-list">
        {% for post in site.categories.opinion %}
            <li>
                <div class="table-article">
                    <div class="col-title">
                        <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                    </div>
                    <div class="col-date">
                        <p class="entry-date">{{ post.date|date:"%Y-%m-%d" }}</p>
                    </div>
                </div>
                <div class="title-desc">{{ post.description }}</div>
            </li>
        {% endfor %}
        </ul>


    </div>
    <div class="aside">
    </div>
</div>
