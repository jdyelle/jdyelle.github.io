---
title: Curriculum Vitae
lede: "20+ years of architecture and engineering leadership, from Oracle and on-prem datacenters to serverless and GenAI on AWS."
permalink: /cv/
---
<p class="cv-actions btn-row">
  <a class="btn" href="https://www.linkedin.com/in/{{ site.author.linkedin }}/" rel="me noopener">View on LinkedIn</a>
  <a class="btn ghost" href="mailto:{{ site.author.email }}">Get in touch</a>
  <a class="btn ghost" href="javascript:window.print()">Print / Save as PDF</a>
</p>

<section class="cv-section" aria-labelledby="cv-highlights">
  <h2 id="cv-highlights">Highlights</h2>
  <ul class="highlights">
    {%- for h in site.data.cv.highlights %}
    <li>{{ h }}</li>
    {%- endfor %}
  </ul>
</section>

<section class="cv-section" aria-labelledby="cv-experience">
  <h2 id="cv-experience">Professional Experience</h2>
  {%- for job in site.data.cv.jobs %}
  <article class="job">
    <div class="job-head">
      <h3>{{ job.title }}</h3>
      <span class="dates">{{ job.dates }}</span>
    </div>
    <div class="org">{{ job.org }} &middot; {{ job.location }}</div>
    <p class="summary">{{ job.summary }}</p>
    <ul class="bullets">
      {%- for b in job.bullets %}
      <li>{{ b }}</li>
      {%- endfor %}
    </ul>
    {%- if job.tags %}
    <ul class="chips no-print" aria-label="Technologies">
      {%- for t in job.tags %}<li>{{ t }}</li>{% endfor %}
    </ul>
    {%- endif %}
  </article>
  {%- endfor %}
</section>

<section class="cv-section" aria-labelledby="cv-projects">
  <h2 id="cv-projects">Recent Projects</h2>
  <p><strong><a href="https://github.com/caylent-solutions/serverless-task-scheduler" rel="noopener">Serverless Task Scheduler</a></strong></p>
  <p>A dependency injection and telemetry framework for launching multitenant serverless tasks (Lambda, Step Functions, or Fargate). A React UI for management and user-to-tenant mapping, plus a Step Functions wrapper, lets business users manage tasks for their group without controlling pipelines or process-flow artifacts. EventBridge runs tasks on demand or on a schedule.</p>
</section>

<section class="cv-section" aria-labelledby="cv-education">
  <h2 id="cv-education">Education and Certifications</h2>
  <ul>
    {%- for e in site.data.cv.education %}<li>{{ e }}</li>{% endfor %}
    {%- for c in site.data.cv.certifications %}<li>{{ c }}</li>{% endfor %}
  </ul>
</section>
