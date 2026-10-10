---
title: Projects
lede: Things I've built, open sourced, written up, and given back to.
permalink: /projects/
---
<section class="section" style="padding-top:0" aria-labelledby="community">
  <h2 id="community">Community</h2>
  <a class="card album" href="https://fullmoonvista.com/rootz/" target="_blank" rel="noopener">
    <span class="icon" aria-hidden="true">🚵</span>
    <h3>ROOTZ youth mountain bike program: volunteer coach</h3>
    <div class="meta">USA Cycling club &middot; Victor, NY</div>
    <p>I volunteer as a mountain bike coach with ROOTZ, a club that helps youth riders (6+) and beginner adults build confidence and skills on the trail. We ride Wednesday evenings from May through July, with a simple rule: always ride together, never alone.</p>
    <p>Coaching new riders has sharpened how I develop less senior engineers. Break a big skill into small, repeatable pieces, make it safe to try something hard and fall down, and celebrate the first time someone clears the root that stopped them last week.</p>
    <span class="more">Learn more about ROOTZ &nearr;</span>
  </a>
</section>

<section class="section" style="padding-top:0" aria-labelledby="work-projects">
<h2 id="work-projects">Code and writing</h2>
<div class="grid">
  <div class="card">
    <h3><a href="https://github.com/caylent-solutions/serverless-task-scheduler" rel="noopener">Serverless Task Scheduler</a></h3>
    <p>A dependency injection and telemetry framework for launching multitenant serverless tasks on Lambda, Step Functions, or Fargate. Includes a React management UI, user-to-tenant mapping, and EventBridge scheduling so business users can run their own tasks without touching pipelines.</p>
    <ul class="chips"><li>AWS</li><li>Step Functions</li><li>EventBridge</li><li>React</li></ul>
    <a class="more" href="https://github.com/caylent-solutions/serverless-task-scheduler" rel="noopener">View on GitHub &rarr;</a>
  </div>
  <div class="card">
    <h3><a href="https://github.com/jdyelle/RocDevESLoader/" rel="noopener">RocDevESLoader</a></h3>
    <p>A C# tool that bulk loads public bike share trip data into Elasticsearch. Built for a RocDev talk in December 2019 and used throughout the Bike Share Kibana tutorial.</p>
    <ul class="chips"><li>C#</li><li>Elasticsearch</li><li>Bulk API</li></ul>
    <a class="more" href="https://github.com/jdyelle/RocDevESLoader/" rel="noopener">View on GitHub &rarr;</a>
  </div>
  <div class="card">
    <h3><a href="{{ '/Tutorials/' | relative_url }}">Tutorials</a></h3>
    <p>Hands-on walkthroughs for building an Elasticsearch cluster in VirtualBox, securing it with Nginx, and exploring data in Kibana.</p>
    <ul class="chips"><li>Elasticsearch</li><li>Kibana</li><li>Nginx</li><li>VirtualBox</li></ul>
    <a class="more" href="{{ '/Tutorials/' | relative_url }}">Read the tutorials &rarr;</a>
  </div>
  <div class="card">
    <h3>Field notes</h3>
    <p>Short, practical notes from my own setups.</p>
    <ul>
      <li><a href="{{ '/Notes/centos_stream_9_kubernetes.txt' | relative_url }}">Kubernetes on CentOS Stream 9 with cri-o</a></li>
      <li><a href="{{ '/Notes/docker_compose_autostart.txt' | relative_url }}">Docker Compose autostart</a></li>
    </ul>
  </div>
</div>
</section>

<section class="section" style="padding-top:0" aria-labelledby="side-projects">
<h2 id="side-projects">Side projects</h2>
<div class="grid">
  <div class="card">
    <h3>Home Dock USA</h3>
    <div class="meta">2025</div>
    <p>Managed the DevOps environment for protected branches and release stability, using VMs, GitHub self-hosted runners, PostgreSQL utilities, and Docker (Supabase images), and provided general LLM assistance to the development team.</p>
    <ul class="chips"><li>DevOps</li><li>GitHub Runners</li><li>PostgreSQL</li><li>Docker</li><li>Supabase</li></ul>
  </div>
  <div class="card">
    <h3><a href="https://rocdev.org/" rel="noopener">RocDev talk: Geospatial analytics with Elasticsearch</a></h3>
    <div class="meta">December 2019</div>
    <p>Used NYC Citi Bike data to show off Elasticsearch's geospatial analytics, with walkthroughs of Kibana as a visualization and data science tool, presented to the RocDev community. The talk became my <a href="{{ '/Tutorials/BikeDataViz/' | relative_url }}">bike share tutorial</a>.</p>
    <ul class="chips"><li>Public speaking</li><li>Elasticsearch</li><li>Kibana</li></ul>
  </div>
</div>
</section>
