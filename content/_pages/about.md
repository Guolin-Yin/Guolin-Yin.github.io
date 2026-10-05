---
layout: about
title: Home
permalink: /
news: false
social: false
latest_posts: false
---

<section class="home-intro" aria-labelledby="home-title">
  <div class="home-intro-copy">
    <p class="home-role">Research Fellow · Centre for Wireless Innovation, Queen’s University Belfast</p>
    <h1 id="home-title">Guolin Yin</h1>
    <p class="home-lead">I work on wireless sensing, radio-frequency fingerprinting, and machine learning.</p>
    <p class="home-bio">My research explores how radio signals can help us understand connected devices and environments, and how to build methods that remain reliable across real-world conditions.</p>
    <nav class="home-links" aria-label="Profile links">
      <a href="{{ '/publications/' | relative_url }}">Publications</a>
      <a href="{{ '/cv/' | relative_url }}">CV</a>
      <a href="mailto:G.Yin@qub.ac.uk">Email</a>
    </nav>
  </div>
  <figure class="home-photo">
    <img src="{{ '/assets/img/prof_pic.JPG' | relative_url }}" alt="Guolin Yin in Belfast" loading="eager" />
    <figcaption>Belfast, Northern Ireland</figcaption>
  </figure>
</section>

<section class="home-section research-section" aria-labelledby="research-title">
  <div class="section-heading">
    <div>
      <p class="section-kicker">Research</p>
      <h2 id="research-title">Wireless signals in connected environments</h2>
    </div>
    <p class="section-intro">I develop sensing and learning methods for wireless systems, with a focus on reliability and security.</p>
  </div>
  <div class="research-list">
    <article class="research-item">
      <h3>Wireless sensing</h3>
      <p>Using Wi-Fi signals to study activity and context, including emerging sensing capabilities in IEEE 802.11bf.</p>
    </article>
    <article class="research-item">
      <h3>Radio-frequency identity</h3>
      <p>Identifying wireless devices from the physical characteristics of their transmissions and testing how well recognition generalises.</p>
    </article>
    <article class="research-item">
      <h3>Robust machine learning</h3>
      <p>Combining signal processing and machine learning to build methods that work across devices, locations, and radio conditions.</p>
    </article>
  </div>
</section>

<section class="home-section home-publications" aria-labelledby="home-publications-title">
  <div class="section-heading">
    <div>
      <p class="section-kicker">Selected work</p>
      <h2 id="home-publications-title">Recent publications</h2>
    </div>
    <a class="text-link" href="{{ '/publications/' | relative_url }}">All publications <span aria-hidden="true">↗</span></a>
  </div>
  <div class="publications home-publication-list">
    {% bibliography --group_by none --query @*[selected=true]* %}
  </div>
</section>

<section class="home-section field-note" aria-labelledby="field-note-title">
  <div class="field-note-copy">
    <p class="section-kicker">In the field · MWC Barcelona 2026</p>
    <h2 id="field-note-title">Testing Wi-Fi device identification in a new environment</h2>
    <p>At Mobile World Congress, our Wi-Fi RFFI system identified devices in an exhibition environment it had not seen before, processing more than 52,000 inference packets with 92% overall accuracy.</p>
    <p class="field-result">52,000+ packets &nbsp;·&nbsp; 92% accuracy &nbsp;·&nbsp; Barcelona</p>
    <a class="field-note-link" href="{{ '/blog/2026/presenting-rffi-at-mwc-2026-barcelona/' | relative_url }}">Read about the demonstration <span aria-hidden="true">↗</span></a>
  </div>
  <figure class="field-note-image">
    <img src="{{ '/assets/img/posts/mwc2026/IMG_8023.jpg' | relative_url }}" alt="Wi-Fi radio fingerprint identification demonstration at Mobile World Congress" loading="lazy" />
    <figcaption>Live Wi-Fi RFFI demonstration · HASC Hub, MWC 2026</figcaption>
  </figure>
</section>

<section class="home-section teaching-section" aria-labelledby="teaching-title">
  <div class="section-heading">
    <div>
      <p class="section-kicker">Teaching</p>
      <h2 id="teaching-title">Teaching and student support</h2>
    </div>
    <a class="text-link" href="{{ '/teaching/' | relative_url }}">More about my teaching <span aria-hidden="true">↗</span></a>
  </div>
  <div class="teaching-list">
    <article class="teaching-item">
      <h3>Queen’s University Belfast · 2025/26</h3>
      <p>Delivered teaching for <strong>ECS4002 Wireless Sensor Systems</strong> in both Semester 1 and Semester 2.</p>
    </article>
    <article class="teaching-item">
      <h3>University of Liverpool · PhD</h3>
      <p>Several years of teaching assistance in machine learning, statistics, electronic circuit design, and communication systems.</p>
    </article>
  </div>
</section>

<section class="home-section service-section" aria-labelledby="service-title">
  <div class="section-heading">
    <div>
      <p class="section-kicker">Academic service</p>
      <h2 id="service-title">Contributing to the research community</h2>
    </div>
  </div>
  <div class="service-details">
    <div>
      <span>Journal reviewer</span>
      <p>IEEE Transactions on Wireless Communications · IEEE Transactions on Mobile Computing</p>
    </div>
    <div>
      <span>TPC member · 2024–26</span>
      <p>GLOBECOM Workshop MLDLWS; ICNC AMCN; INFOCOM DeepWireless; ICC MLDLWiSec and MLDL Security; WCNCW WS13.</p>
    </div>
    <div>
      <span>TPC reviewer · 2025</span>
      <p>IEEE WF-IoT · AI/Machine Learning Technologies</p>
    </div>
    <div>
      <span>Upcoming TPC membership</span>
      <p>GC Workshops 2026 — MLDL WS · December 2026</p>
    </div>
  </div>
</section>

<section class="home-section writing-section" aria-labelledby="writing-title">
  <div class="section-heading writing-heading">
    <div>
      <p class="section-kicker">Notes</p>
      <h2 id="writing-title">Recent writing</h2>
    </div>
    <a class="text-link" href="{{ '/blog/' | relative_url }}">All notes <span aria-hidden="true">↗</span></a>
  </div>
  <div class="recent-posts">
    {% for post in site.posts limit:3 %}
      <a class="recent-post" href="{{ post.url | relative_url }}">
        <span class="recent-post-date">{{ post.date | date: '%b %Y' }}</span>
        <span class="recent-post-title">{{ post.title }}</span>
        <span class="recent-post-arrow" aria-hidden="true">↗</span>
      </a>
    {% endfor %}
  </div>
</section>

<section class="home-contact" aria-labelledby="contact-title">
  <h2 id="contact-title">Get in touch</h2>
  <div class="contact-actions">
    <a href="mailto:G.Yin@qub.ac.uk">Email</a>
    <a href="https://scholar.google.com/citations?user={{ site.scholar_userid }}" target="_blank" rel="noopener noreferrer">Google Scholar</a>
    <a href="https://github.com/{{ site.github_username }}" target="_blank" rel="noopener noreferrer">GitHub</a>
  </div>
</section>
