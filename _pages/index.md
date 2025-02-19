---
layout: page
title: Home
id: home
permalink: /
---

<div class="home-welcome">
  <div class="welcome-img"></div>

  <div>
    <h1>howdy! welcome to my [[digital garden]]! ✧🦋(◕‿◕✿)</h1>

    <p>here you'll find resources i've collected and thoughts i have on a wide variety of topics that inspire me, reflect my values, and feed my insatiable appetite for learning cool shizz! think of it less like a traditional blog and more of a free-form personal notebook, where there's no need for polish or performance.</p>

    <p>in an increasingly unstable digital world, this is my effort to carve out a corner of the internet where i can reliably preserve the things that feel important; for myself, and whoever else may be interested in the same things!</p>

    <p>for a visual representation of everything i have here thus far, check out my [[node map]].</p>

  </div>
</div>

<hr>

<div class="home-links">
  <div>
    <h2>themesᯓ★</h2>
    <p>here are some starting points if you're not sure where to jump in!</p>
    <p>[[tech]] [[anti-capitalism]] [[occult]] [[books]] [[mental health]] [[writing]]</p>
  </div>

  <div>
    <h2>recently updated notes 𖤣.𖥧.𖡼.⚘</h2>
    <ul>
      {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
      {% for note in recent_notes limit: 5 %}
        <li>
          {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
        </li>
      {% endfor %}
    </ul>
  </div>

  <div>
    <h2>thanks for visiting 𓆩♡𓆪</h2>
    <p>feel free to drop a lil note in my guestbook, or check out my <a href="https://www.haleytibbitts.com">website</a> to see what else i've got goin' on.</p>
  </div>

  <div class="links-img"></div>
</div>
