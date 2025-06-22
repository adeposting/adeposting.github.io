---
layout: page
permalink: /
description: i'm ade. i do things. make stuff. here's some. have fun.
---

<style>
    footer {
        margin-left: 5%;
    }

    header {
        display: none;
    }

    .container {
        display: flex;
        gap: 10px;
        align-items: center;

        .box {
            padding: 20px;
            text-align: left;
        }

        .icon {
            display: block;
        }

        ul {
            list-style: none;
            padding: 0;
            margin: 0;
        }

        .icon-container {
            display: flex;
            align-items: center;
            gap: 8px;
            margin-top: 5%;
        }

        img {
            width: 33vw;
            height: 33vw;
            min-height: 170px;
            min-width: 170px;
            max-height: 250px;
            max-width: 250px;
        }

        img.size-24px {
            margin: 0;
            padding: 0;
            width: 24px;
            height: 24px;
            min-height: 24px;
            min-width: 24px;
            max-height: 24px;
            max-width: 24px;
        }

    }

    @media (max-width: 346px) {
        .container {
            flex-direction: column;
        }
    }
</style>

<h1>{{ site.title }}</h1>

<p>
    {{ site.description }}
</p>

<div class="container">
    <div class="box">
        <img src="/assets/images/featured_image.jpg" alt="{{ site.title | escape }}">
    </div>
    <div class="box">
        <ul>
            <!--li class="icon-container">
                {%- include theme/icons/text.html text="B" class="size-24px" -%}
                <a href="https://blog.adeposting.com/">ade's blog</a>
            </li-->
            <li class="icon-container">
                {%- include theme/icons/text.html text="N" class="size-24px" -%}
                <a href="https://notes.adeposting.com/">ade's notes</a>
            </li>
            <li class="icon-container">
                {%- include theme/icons/github.html class="size-24px" -%}
                <a href="https://github.com/{{ site.github.username }}">@{{ site.github.username }}</a>
            </li>
            <li class="icon-container">
                {%- include theme/icons/twitter.html class="size-24px" -%}
                <a href="https://x.com/{{ site.twitter.username }}">@{{ site.twitter.username }}</a>
            </li>
        </ul>
    </div>
</div>