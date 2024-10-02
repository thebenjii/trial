---
layout: internship
title: Software Engineering Intern
company: TechCorp
location: San Francisco, CA
description: Work on cutting-edge software projects.
permalink: /internships/software-engineering-intern/
---

# {{ page.title }}

**Company**: {{ page.company }}

**Location**: {{ page.location }}

**Description:**

{{ page.description }}

---

## Apply for This Position

<form action="https://formspree.io/f/xldrqyoq" method="POST">
  <!-- Internship title -->
  <input type="hidden" name="internship" value="{{ page.title }}">
  <!-- Redirect after submission -->
  <input type="hidden" name="_next" value="{{ '/thank-you/' | relative_url }}">

  <!-- Applicant's Name -->
  <label for="name">Name:</label><br>
  <input type="text" id="name" name="name" required><br><br>

  <!-- Applicant's Email -->
  <label for="email">Email:</label><br>
  <input type="email" id="email" name="_replyto" required><br><br>

  <!-- Applicant's Major -->
  <label for="major">Major:</label><br>
  <input type="text" id="major" name="major"><br><br>

  <!-- Applicant's Contact Information -->
  <label for="contact">Contact Information:</label><br>
  <textarea id="contact" name="contact" rows="4" cols="50"></textarea><br><br>

  <!-- Submit Button -->
  <input type="submit" value="Submit Application">
</form>
