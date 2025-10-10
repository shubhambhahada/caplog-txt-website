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
        <!-- <a href="#syntax-example" class="btn btn-primary">
          See it in Action
          <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
            <path d="M7 17l9.2-9.2M17 17V7H7"/>
          </svg>
        </a> -->
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


<section id="features" class="section section-features">
  <div class="container">
    <div class="features">
      <!-- <div class="features-header">
        <h2 class="features-title">Built for the Long Term</h2>
        <p class="features-subtitle">
          Every design decision prioritizes longevity, simplicity, and interoperability across tools and platforms.
        </p>
      </div> -->
      
      <div class="grid grid-3">
        <div class="card">
          <div class="card-icon">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
              <path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/>
              <polyline points="14,2 14,8 20,8"/>
              <line x1="16" y1="13" x2="8" y2="13"/>
              <line x1="16" y1="17" x2="8" y2="17"/>
              <polyline points="10,9 9,9 8,9"/>
            </svg>
          </div>
          <h3 class="card-title">Plain Text Forever</h3>
          <p class="card-description">
            No proprietary formats, no vendor lock-in. Your logs are stored as plain text files that will be readable for decades to come.
          </p>
        </div>
        
        <div class="card">
          <div class="card-icon">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
              <polyline points="16 18 22 12 16 6"/>
              <polyline points="8 6 2 12 8 18"/>
            </svg>
          </div>
          <h3 class="card-title">Human & Machine Readable</h3>
          <p class="card-description">
            Designed to be easily read by humans while maintaining a consistent structure that tools and scripts can parse reliably.
          </p>
        </div>
        
        <div class="card">
          <div class="card-icon">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
              <circle cx="12" cy="12" r="10"/>
              <polyline points="12,6 12,12 16,14"/>
            </svg>
          </div>
          <h3 class="card-title">Structured Timeline</h3>
          <p class="card-description">
            Each entry includes both event datetime and entry timestamp, providing clear chronological structure for your personal history.
          </p>
        </div>
        
        <div class="card">
          <div class="card-icon">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
              <path d="M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z"/>
              <polyline points="3.27,6.96 12,12.01 20.73,6.96"/>
              <line x1="12" y1="22.08" x2="12" y2="12"/>
            </svg>
          </div>
          <h3 class="card-title">Tool Interoperability</h3>
          <p class="card-description">
            A simple format specification enables multiple independent implementations, ensuring you're never locked into a single tool.
          </p>
        </div>
        
        <div class="card">
          <div class="card-icon">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
              <path d="M9 11H5a2 2 0 0 0-2 2v3a2 2 0 0 0 2 2h4"/>
              <path d="M15 11h4a2 2 0 0 1 2 2v3a2 2 0 0 1-2 2h-4"/>
              <path d="M12 5v14"/>
              <path d="M8 5h8"/>
              <path d="M8 19h8"/>
            </svg>
          </div>
          <h3 class="card-title">Version Control Friendly</h3>
          <p class="card-description">
            Plain text format works beautifully with Git and other version control systems, giving you a complete history of your logs.
          </p>
        </div>
        
        <div class="card">
          <div class="card-icon">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
              <path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/>
            </svg>
          </div>
          <h3 class="card-title">Simple Syntax</h3>
          <p class="card-description">
            Three lines per entry: event datetime, entry timestamp, and message. That's it. Easy to learn, impossible to forget.
          </p>
        </div>
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
    <div class="apps-header">
      <h2>Apps</h2>
      <p class="apps-subtitle">
        Tools and applications that work with the Caplog.txt format
      </p>
    </div>
    
    <div class="apps-grid">
      <div class="app-card">
        <div class="app-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
            <polyline points="4 17 10 11 4 5"/>
            <line x1="12" y1="19" x2="20" y2="19"/>
          </svg>
        </div>
        <div class="app-content">
          <h3 class="app-title">CLI Tool</h3>
          <p class="app-description">
            Python command-line interface for creating and managing caplog.txt files. 
            Interactive entry creation with automatic timestamps and validation.
          </p>
          <a href="{{ site.github.cli_repository_url }}" class="app-link" target="_blank" rel="noopener noreferrer">
            View on GitHub
            <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
              <path d="M7 17l9.2-9.2M17 17V7H7"/>
            </svg>
          </a>
        </div>
      </div>
      
      <!-- Placeholder for future apps -->
      <div class="app-card coming-soon">
        <div class="app-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
            <circle cx="12" cy="12" r="10"/>
            <path d="M12 6v6l4 2"/>
          </svg>
        </div>
        <div class="app-content">
          <h3 class="app-title">More Apps Coming Soon</h3>
          <p class="app-description">
            Additional tools and integrations are in development. 
            Stay tuned for web interfaces, mobile apps, and editor plugins.
          </p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- <section id="terminal-example" class="section">
  <div class="container">
    <div class="grid grid-2" style="align-items: center;">
      <div>
        <h2>Command Line Tool</h2>
        <p>
          Get started immediately with our Python CLI tool. It handles the format details 
          so you can focus on capturing your thoughts and experiences.
        </p>
        
        <div class="btn-group">
          <a href="{{ site.github.cli_repository_url }}" class="btn btn-primary" target="_blank" rel="noopener noreferrer">
            Download CLI Tool
          </a>
          <a href="{{ site.github.cli_repository_url }}#usage" class="btn btn-outline" target="_blank" rel="noopener noreferrer">
            View Documentation
          </a>
        </div>
      </div>
      
      <div>
        <div class="code-example">
          <div class="code-header">
            <h4 class="code-title">Terminal</h4>
          </div>
          <pre><code>$ python3 caplog.py ~/my-journal.txt
            Enter the entry date (Press enter to accept the default 2023-10-07):
            Enter the entry message (empty line to exit):
            Had a productive day working on the website.
            The new design is coming together nicely.
              Entry added successfully!</code></pre>
        </div>
      </div>
    </div>
  </div>
</section> -->

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