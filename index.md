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