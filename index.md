---
layout: default
---

<section class="hero">
  <h1>Jaewon Choi</h1>
  <p class="tagline">Ph.D. Candidate | Researcher in Agentic AI for Healthcare</p>
  <p class="text-light mb-4">Bridging Computer Systems Engineering and Medical Applications</p>
  
  <div class="cta-buttons">
    <a href="{{ '/projects/' | relative_url }}" class="btn btn-primary">View Projects</a>
    <a href="{{ '/publications/' | relative_url }}" class="btn btn-secondary">Publications</a>
  </div>
</section>

<section class="mb-4">
  <h2 class="text-center mb-3">News</h2>
  <div class="card">
    <ul>
      <li><strong>Nov 2026 (upcoming)</strong> — Invited talk "Agentic AI와 함께 연구하기" at the Inha University AI Convergence Seminar (Nov 3, online).</li>
      <li><strong>Oct 2026</strong> — Our paper on conditional resistance in synthetic microbiology profiles was accepted to the <a href="https://openreview.net/forum?id=HYtTXJuihA">NeurIPS 2026 GenAI4Health workshop</a> (co-first author).</li>
      <li><strong>Aug 2026</strong> — Our paper on predicting hemorrhage after brain biopsy was accepted to <em>Scientific Reports</em> (co-first author).</li>
      <li><strong>Aug 2026</strong> — PSCT-Net, on pediatric skull CT reconstruction, was accepted to the <a href="https://openreview.net/forum?id=31fG44sdm6">MICCAI 2026 PedAItrics workshop</a>.</li>
      <li><strong>Jun 2026</strong> — Our paper on transrectal ultrasound prostate video segmentation was accepted to MICCAI 2026.</li>
      <li><strong>Mar 2026</strong> — Presented HoloQRam at IEEE PerCom 2026 in Pisa (Best Paper Candidate).</li>
    </ul>
    <p class="text-center"><a href="{{ '/publications/' | relative_url }}">All publications →</a></p>
  </div>
</section>

<section class="mb-4">
  <h2 class="text-center mb-3">Research Areas</h2>
  <div class="grid grid-3">
    <div class="card">
      <h3>🤖 Agentic AI for Healthcare</h3>
      <p>Developing autonomous AI agents for clinical decision support and medical workflow automation at Seoul National University Hospital.</p>
    </div>
    <div class="card">
      <h3>📱 Mobile Systems & Graphics</h3>
      <p>Low-power graphics optimization for AR/VR devices, real-time rendering, and perceptual computing for mobile platforms.</p>
    </div>
    <div class="card">
      <h3>🏥 Medical Imaging & Diagnostics</h3>
      <p>AI-powered medical image analysis, automated pathology diagnostics, and VR-based diagnostic systems.</p>
    </div>
  </div>
</section>

<section class="mb-4">
  <h2 class="text-center mb-3">Recent Highlights</h2>
  <div class="grid grid-2">
    <div class="card">
      <h3>🏆 MD Winners Hackathon 2025</h3>
      <p class="card-meta">First Place Winner</p>
      <p>Developed an AI-powered medical diagnosis platform demonstrating innovative applications of agentic AI in healthcare.</p>
    </div>
    <div class="card">
      <h3>🏥 SCCM Datathon Chicago</h3>
      <p class="card-meta">K-MIMIC Data Provider & Mentor</p>
      <p>Attended SCCM Datathon at the Society of Critical Care Medicine HQ, providing K-MIMIC dataset access and mentoring teams on critical care data analytics.</p>
    </div>
  </div>
  <div class="text-center mt-3">
    <a href="{{ '/highlights/' | relative_url }}" class="btn btn-secondary">View All Highlights</a>
  </div>
</section>

<section>
  <h2 class="text-center mb-3">Latest Blog Posts</h2>
  <div class="grid grid-2">
    {% for post in site.posts limit:4 %}
    <article class="card">
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p class="card-meta">{{ post.date | date: "%B %d, %Y" }}</p>
      <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
      <a href="{{ post.url | relative_url }}" class="read-more">Read more →</a>
    </article>
    {% endfor %}
  </div>
  <div class="text-center mt-3">
    <a href="{{ '/blog/' | relative_url }}" class="btn btn-secondary">View All Posts</a>
  </div>
</section>