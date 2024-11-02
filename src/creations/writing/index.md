---
layout: t2
title: Writing
ogd: Stuff I wrote like my poetry and short stories
propd: Stuff I wrote like my poetry and short stories
templateEngineOverride: njk, md
---

# my writing

---

## Short Stories And Concepts <i class="ph ph-notebook"></i>
My short stories, I mostly make them up on the fly. I put my concepts here as well.

<ul>
{%- for post in collections.story | reverse -%}
    <li style="margin-bottom:5px;"><a style="font-style: normal;" href="{{ post.url }}">{{ post.data.title }}</a> - <span style=" font-style: normal;">{{ post.date.toLocaleDateString('en-US', { month: 'short', day: 'numeric', year: 'numeric' }).replace('.', '') }}</span></li>
  {%- endfor -%}
</ul>

## Poetry <i class="ph ph-scroll"></i>
All of these are experimental and some of these are pretentious

<ul>
{%- for post in collections.poetry | reverse -%}
     <li style="margin-bottom:5px;"><a style="font-style: normal;" href="{{ post.url }}">{{ post.data.title }}</a> - <span style=" font-style: normal;">{{ post.date.toLocaleDateString('en-US', { month: 'short', day: 'numeric', year: 'numeric' }).replace('.', '') }}</span></li>
  {%- endfor -%}
</ul>

## Archives <i class="ph ph-archive"></i>
Old stuff from my original writing blog on Tumblr, might rewrite IOTD. SaH is under rewriting.

<ul>
{%- for post in collections.archive | reverse -%}
     <li style="margin-bottom:5px;"><a style="font-style: normal;" href="{{ post.url }}">{{ post.data.title }}</a> - <span style=" font-style: normal;">{{ post.date.toLocaleDateString('en-US', { month: 'short', day: 'numeric', year: 'numeric' }).replace('.', '') }}</span></li>
  {%- endfor -%}
</ul>

