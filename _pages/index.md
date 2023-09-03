---
layout: page
title: Home
id: home
permalink: /
---

# Welcome! 🙏

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Only a Hindu Can Teach about Hinduism. - Garuda
</p>

This is the Website of Garuda. I writes about Religion and Science. I am a Hindu and My goal is to make people understand Hinduism , to eliminate the disinformation they may have attained from some Sources.

You can find all of my articles  <a class="internal-link" href="/articles">Here</a>.

<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
