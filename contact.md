---
layout: default
title: Contact
permalink: /contact/
---
<div class="container">
  <div class="page-hero">
    <h1 class="page-hero__title">Get in touch</h1>
    <p class="page-hero__sub">I'd love to hear from you.</p>
  </div>

  <div class="contact-grid">
    <form class="contact-form" action="https://formspree.io/f/your-form-id" method="POST">
      <div class="form-group">
        <label for="name">Name</label>
        <input type="text" id="name" name="name" required placeholder="Your name" />
      </div>
      <div class="form-group">
        <label for="email">Email</label>
        <input type="email" id="email" name="email" required placeholder="you@example.com" />
      </div>
      <div class="form-group">
        <label for="message">Message</label>
        <textarea id="message" name="message" rows="6" required placeholder="What's on your mind?"></textarea>
      </div>
      <button type="submit" class="btn">Send message</button>
    </form>

    <div class="contact-info">
      <p>I reply to most messages within a few days. If you've written something you'd like me to read, I'm open to that too.</p>
      <p>For time-sensitive matters, email is fastest.</p>

      <a href="mailto:you@example.com" class="contact-link">
        <span class="contact-link__label">Email</span>
        <span>you@example.com</span>
      </a>
      <a href="https://twitter.com/yourusername" class="contact-link">
        <span class="contact-link__label">Twitter</span>
        <span>@yourusername</span>
      </a>
      <a href="https://github.com/yourusername" class="contact-link">
        <span class="contact-link__label">GitHub</span>
        <span>github.com/yourusername</span>
      </a>
    </div>
  </div>
</div>
