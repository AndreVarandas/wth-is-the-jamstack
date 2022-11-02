---
theme: apple-basic
colorSchema: light
layout: intro-image
image: /cover.avif
fonts:
  sans: Roboto
  serif: Roboto Slab
  mono: Fira Code
css: unocss
---

<div class="absolute rounded bottom-10 p-8 bg-coolgray-8">
  <h1>WTH is the Jamstack?</h1>
  <p>By André Varandas - <logos-twitter class="text-3xl mx-2" /> <a href="https://twitter.com/iamvarandas">@iamvarandas</a></p>
</div>


---
layout: intro-image-right
image: /wp-logo.png
---

# LAMP Stack

## Building a website with WordPress

### Linux, Apache, MySQL, PHP

- Use it to build dynamic websites.
- Used by WordPress, Drupal, Joomla, etc.

<br />

<logos-linux-tux class="text-3xl mx-2" /> 
<logos-apache class="text-3xl mx-2" /> 
<logos-mysql class="text-3xl mx-2" /> 
<logos-php class="text-3xl mx-2" />

<TheFooter />

<!--
LAMP Definition, what is it, how it works, how to use it, etc.
-->

---
layout: image-right
image: /this-is-fine.jpg
---

# Let's look into...

### LAMP - (Linux, Apache, MySQL, PHP)

### WordPress development flow

- Configure the stack
- Manage Wordpress, plugins and themes
- Developing and deploying

<br />

### Maintaining the server

- Security patches
- Linux, PHP, MYSQL, Apache updates
- Backups, monitoring and logging

<TheFooter />

<!--
How do we setup and maintain a WordPress website running on the LAMP stack
-->

---
layout: image-right
image: /wp-routing.svg
---

# Let's look into...

### LAMP Frontend Flow

https://andrevarandas.dev

Wordpress main() - entry point for every request.

```php
public function main($query_args = '') {
    $this->init();
    $this->parse_request($query_args);
    $this->send_headers();
    $this->query_posts();
    $this->handle_404();
    $this->register_globals();

    do_action_ref_array('wp', array(&$this));
}
```

<TheFooter />

<!--
- WordPress environment is loaded (core, plugins, theme)
- WordPress looks at URL and builds some query arguments based on it
- Obtained query arguments are used to run a \WP_Query (known as "main query")
- Based on the "type" of the query (eg. "single", "archive"…), WordPress chooses a template file among the ones available in theme
- Template file is loaded to display page
-->

---
layout: intro-image-right
image: /jam.png
---

# WTH is Jamstack?

### What is it?

- It's not a framework.
- It started as a marketing term.
- It's a way of building websites and apps.

<TheFooter />

<!--
JavaScript
Any framework or library you'd like

APIs
Server-side operations using APIs with JavaScript.

Markup
Generated from source files, Markdown, JSON, or a headless CMS.
-->

---

# Let's look into...

<div class="grid grid-cols-2">
<div>

### Must have

<br />

1. <logos-github class="text-2xl" /> Source code in a Git repository
2. <logos-netlify class="text-2xl" /> CDN or static site hosting

<br />

### Tools

<br />

1. Static site generators: **347**
2. Headless CMS: **96**
3. **Countless** amount of APIs.

<br />

</div>
<div>

### Optional

1. <logos-nextjs class="text-2xl" /> Static site generator 
2. <logos-aws class="text-2xl" /> Serverless functions or APIs 
3. <logos-strapi class="text-2xl" /> Headless CMS to manage content

</div>
</div>

<TheFooter />

<!--
2 Must use:

- Git and CDN or static site hosting.

Optional tools and how they work.
-->

---
layout: statement
---

# Typical workflow

### For developing a Jamstack site

<br>

1. <twemoji-pencil /> Write content - Headless CMS, markdown files.
2. <twemoji-laptop /> Write code for the frontend, microservices, use version control.
3. <twemoji-hammer /> Build! Fetch content and convert to static files.
4. <twemoji-rocket /> Deploy static files to a CDN/static site hosting.

<!--
Use your markup files to generate your pages.
Write your code to create dynamic elements.
Use your API to fetch content during build time.
Deploy your static files to a CDN.
-->

<TheFooter />

<!--
Typical workflow

- Write content
-  Dynamic behavior with JavaScript. Use GIT
- Push code changes, use version control
- Build should generate static files - prerender html in advance.
-->

---
layout: image-right
image: /jamstack-flow.png
---

# Let's look into...

### Jamstack Frontend Flow

https://andrevarandas.dev

<br />

1. <twemoji-man-technologist class="text-3xl" /> User requests a page
2. <logos-netlify class="text-3xl" /> The CDN delivers the static files
3. <twemoji-sparkles class="text-3xl" /> The page is loaded and rendered
4. <twemoji-cloud class="text-3xl" /> Client may request microservices

<!--
- Content Delivery Network
-Microservices such as firebase authentication
-->

<TheFooter />

---
layout: intro-image-right
image: /sutmm.jpeg
---

# Advantages?

- <twemoji-rocket class="text-xl text-orange-400" /> Faster 
- <twemoji-sparkles />  More secure
- <twemoji-money-mouth-face /> Cheaper, easier to scale and maintain
- <twemoji-robot /> Developer-friendly

<TheFooter />

<!--
- There is no server to maintain
- No Database or server-side code to maintain
- CDN is automatically scaled
- Focus on the frontend
-->

---
layout: statement
---

# When to use it?

<br />

## Use it when...

<br />

1. <twemoji-check-mark /> Marketing sites, blogs, eCommerce, documentation, etc.
2. <twemoji-check-mark /> When performance and SEO is a priority.

<br />

## But not for...

<br />

1. <twemoji-cross-mark /> Sites that need to be updated often or in real-time.
2. <twemoji-cross-mark /> Sites that need to perform complex operations. 

<TheFooter />

<!--
- Performance, SEO - static content
-->

---
layout: statement
---

# How to create a Jamstack site?

<br />

## With Markdown, Next.js and Neflify

### phplisbon.com

<TheFooter />

---
layout: intro-image-right
image: /thank-you.jpg
---

# Thank you!

<br />

<twemoji-red-heart class="text-4xl" /> <twemoji-red-heart class="text-4xl" /> <twemoji-red-heart class="text-4xl" />

<br />
<br />

### You can reach me at

1. <logos-twitter class="text-3xl mx-2" /> <a href="https://twitter.com/iamvarandas">@iamvarandas</a>
2. <logos-github class="text-3xl mx-2" /> <a href="https://github.com/andrevarandas">@andrevarandas</a>

<TheFooter />
