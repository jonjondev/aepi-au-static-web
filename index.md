---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
relativity: .
title: AEPi Sydney Metro
subtitle: Welcome to the official website of the ΩZA Chapter of Alpha Epsilon Pi, the international Jewish fraternity.
---
<div class="home-container">
    <div class="home-posts">
        {%- if site.posts.size > 0 -%}
            {%- for post in site.posts limit:2 -%}
                <div class="blog-card-full">
                    {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
                    <h3>{{ post.date | date: date_format }}</h3>
                    <div class="blog-image" style="background-image: url({{ post.image }})"></div>
                    <div class="blog-text">
                        <h1>{{ post.title }}</h1>
                        <p>{{ post.body }}</p>
                    </div>
                    {%- if site.show_excerpts -%}
                        {{ post.excerpt }}
                    {%- endif -%}
                </div>
            {%- endfor -%}
        {%- endif -%}
    </div>
    <div class="home-social">
        <iframe allowtransparency="true" frameborder="1" height="900" scrolling="no" src="https://www.facebook.com/plugins/page.php?href=https%3A%2F%2Fwww.facebook.com%2Faepisydney%2F&amp;tabs=timeline&amp;width=340&amp;height=500&amp;small_header=false&amp;adapt_container_width=true&amp;hide_cover=false&amp;show_facepile=true&amp;appId=303155660018639" style="border:none;overflow:hidden" width="340"></iframe>
    </div>
</div>