---
layout: default
title: "Caplog.txt - Structured Personal Logging"
description: "An open, plain-text format for structured personal logging. Future-proof, human-readable, and machine-parseable."
---

<section id="hero" class="section section-hero">
  <div class="container">
    <div class="hero">
      <h1 class="hero-title">
        Simple. Structured. <span class="text-accent">Personal Logging.</span>
      </h1>
      <p class="hero-subtitle">
        Caplog.txt is an open, plain-text format for structuring your personal logs. 
        Future-proof, human-readable, and designed for longevity.
      </p>
      <div class="hero-actions">
        <a href="{{ site.github.repository_url }}" class="btn btn-primary" target="_blank" rel="noopener noreferrer">
          Read Specification
          <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
            <path d="M7 17l9.2-9.2M17 17V7H7"/>
          </svg>
        </a>
        <a href="{{ site.github.repository_url }}" class="btn btn-outline" target="_blank" rel="noopener noreferrer">
          <svg class="icon" viewBox="0 0 24 24" fill="currentColor">
            <path d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385.6.105.825-.255.825-.57 0-.285-.015-1.23-.015-2.235-3.015.555-3.795-.735-4.035-1.41-.135-.345-.72-1.41-1.23-1.695-.42-.225-1.02-.78-.015-.795.945-.015 1.62.87 1.845 1.23 1.08 1.815 2.805 1.305 3.495.99.105-.78.42-1.305.765-1.605-2.67-.3-5.46-1.335-5.46-5.925 0-1.305.465-2.385 1.23-3.225-.12-.3-.54-1.53.12-3.18 0 0 1.005-.315 3.3 1.23.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23.66 1.65.24 2.88.12 3.18.765.84 1.23 1.905 1.23 3.225 0 4.605-2.805 5.625-5.475 5.925.435.375.81 1.095.81 2.22 0 1.605-.015 2.895-.015 3.3 0 .315.225.69.825.57A12.02 12.02 0 0024 12c0-6.63-5.37-12-12-12z"/>
          </svg>
          View on GitHub
        </a>
      </div>
    </div>
  </div>
</section>





<section id="syntax-example" class="section">
  <div class="container">
    <div class="text-center" style="margin-bottom: 3rem;">
      <h2>See It In Action</h2>
      <p class="text-lg">
        Here's what a Caplog.txt file looks like. Clean, structured, and immediately understandable.
      </p>
    </div>
    
    <div class="code-example">
      <div class="code-header">
        <h4 class="code-title">sample.caplog.txt</h4>
        <button class="code-copy" onclick="copyCode()">Copy</button>
      </div>
      <pre><code>2023-10-06
2023-10-06T14:30:15
Started working on the new project proposal. 
Initial research phase complete, moving to draft outline.

2023-10-06
2023-10-06T18:45:22
Team meeting went well. Everyone aligned on project goals.
Sarah raised some good points about timeline constraints.

2023-10-07
2023-10-07T09:15:00
Morning run in the park. 5K in 28 minutes - personal best!
Weather was perfect, cool and crisp.</code></pre>
    </div>
    
    <div style="margin-top: 2rem; text-align: center;">
      <p class="text-secondary">
        Three simple parts: <strong>Event Date</strong>, <strong>Entry Timestamp</strong>, and <strong>Message</strong>.
        Separated by blank lines. That's the entire specification.
      </p>
    </div>
  </div>
</section>

<section id="apps" class="section section-apps">
  <div class="container">
    <div class="text-center" style="max-width: 800px; margin: 0 auto;">
      <h2>Apps</h2>
      <p>
        A Python CLI tool that handles the format details so you can focus on capturing your thoughts and experiences.
      </p>
      
      <div class="btn-group" style="margin-top: 2rem;">
        <a href="{{ site.github.cli_repository_url }}" class="btn btn-primary" target="_blank" rel="noopener noreferrer">
          CLI Tool on GitHub
        </a>
      </div>
    </div>
  </div>
</section>



<script>
function copyCode() {
  const code = document.querySelector('.code-example pre code').textContent;
  navigator.clipboard.writeText(code).then(function() {
    const button = document.querySelector('.code-copy');
    const originalText = button.textContent;
    button.textContent = 'Copied!';
    setTimeout(function() {
      button.textContent = originalText;
    }, 2000);
  });
}
</script>