---
title: Adventures
lede: Work is a big part of my life, but it isn't all of it. This is where the pedals, trails, and campfires live.
permalink: /adventures/
---
<div class="pillars">
  <div class="card photo">
    <img src="{{ '/assets/img/adventures/cycling.jpg' | relative_url }}" alt="Me and my road bike in front of a rushing waterfall" width="1000" height="753" loading="lazy">
    <div class="body">
      <h3>Cycling</h3>
      <p>Miles on two wheels are where I do my best thinking, and a good way to turn a free afternoon into an adventure.</p>
    </div>
  </div>
  <div class="card photo">
    <img src="{{ '/assets/img/adventures/mountain-biking.jpg' | relative_url }}" alt="Me and my mountain bike on a lookout deck above a forested valley" width="1000" height="753" loading="lazy">
    <div class="body">
      <h3>Mountain biking</h3>
      <p>Singletrack, roots, rocks, and the satisfaction of finally clearing a section that beat me last time.</p>
    </div>
  </div>
  <div class="card photo">
    <img src="{{ '/assets/img/adventures/camping.jpg' | relative_url }}" alt="A campsite in the woods with an awning off the van and a muddy mountain bike on the rack" width="1000" height="753" loading="lazy">
    <div class="body">
      <h3>Weekend camping</h3>
      <p>Pack the car on Friday, unplug, cook outside, and be back Sunday feeling like I took a week off.</p>
    </div>
  </div>
</div>

{%- if site.data.albums.size > 0 %}
<section class="section" aria-labelledby="photo-albums">
  <h2 id="photo-albums">Photo albums</h2>
  <p class="sub">The full, unedited camera roll. Albums open in Google Photos.</p>
  <div class="grid">
    {%- for album in site.data.albums %}
    <a class="card album" href="{{ album.url }}" target="_blank" rel="noopener">
      <span class="icon" aria-hidden="true">{{ album.icon | default: "📸" }}</span>
      <h3>{{ album.title }}</h3>
      {%- if album.dates %}<div class="meta">{{ album.dates }}</div>{% endif %}
      {%- if album.description %}<p>{{ album.description }}</p>{% endif %}
      <span class="more">Open album in Google Photos &nearr;</span>
    </a>
    {%- endfor %}
  </div>
</section>
{%- endif %}

{%- assign log = site.data.adventures | sort: 'date' | reverse %}
{%- if log.size > 0 %}
<section class="section" aria-labelledby="trail-log">
  <h2 id="trail-log">Trail log</h2>
  <div class="gallery">
    {%- for a in log %}
    <figure class="shot">
      {%- if a.image %}<img src="{{ a.image | relative_url }}" alt="{{ a.title }}" loading="lazy">{% endif %}
      <figcaption>
        <div class="title">{{ a.title }}</div>
        <div class="meta">{{ a.category }}{% if a.place %} &middot; {{ a.place }}{% endif %}{% if a.date %} &middot; {{ a.date | date: "%b %Y" }}{% endif %}</div>
        {%- if a.caption %}<p>{{ a.caption }}</p>{% endif %}
      </figcaption>
    </figure>
    {%- endfor %}
  </div>
</section>
{%- endif %}

<section class="section" aria-labelledby="bikes-and-data">
  <h2 id="bikes-and-data">Where the hobbies meet the day job</h2>
  <p>I've never been able to keep bikes out of my work. A few years ago I turned public bike share data into a hands-on lesson in data discovery with Kibana. And every Wednesday evening from May through July, I volunteer as a mountain bike coach with <a href="https://fullmoonvista.com/rootz/" target="_blank" rel="noopener">ROOTZ</a>, a youth and beginner-adult program.</p>
  <p>Coaching beginners to clear their first root turns out to be good practice for being a good teammate: small steps, a safe place to fall, and plenty of celebrating when it clicks. <a href="{{ '/projects/' | relative_url }}#community">More on coaching</a>.</p>
  <p class="btn-row">
    <a class="btn ghost" href="{{ '/Tutorials/BikeDataViz/' | relative_url }}">Visualizing bike share data with Kibana</a>
    <a class="btn ghost" href="https://fullmoonvista.com/rootz/" target="_blank" rel="noopener">About ROOTZ</a>
  </p>
</section>
