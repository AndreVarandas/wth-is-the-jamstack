---
theme: apple-basic
colorSchema: light
layout: intro-image
image: >-
  https://images.unsplash.com/photo-1657441411855-5ba346a6b044?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1710&q=80
fonts:
  sans: Roboto
  serif: Roboto Slab
  mono: Fira Code
css: unocss
class: text-coolgray-8 bg-coolgray-1
---

<div class="absolute rounded bottom-10 p-8 bg-coolgray-8">
  <h1>WTH is the Jamstack?</h1>
  <p>By André Varandas - <logos-twitter class="text-3xl mx-2" /> <a href="https://twitter.com/iamvarandas">@iamvarandas</a></p>
</div>


---
layout: image-right
image: https://s.w.org/style/images/about/WordPress-logotype-wmark.png
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

---
layout: image-right
image: ./assets/this-is-fine.jpg
---

# Let's look into...

### LAMP - (Linux, Apache, MySQL, PHP)

### WordPress development flow

- Configure the stack
- Developing and deploying
- Manage Wordpress, plugins and themes

<br />

### Maintaining the server

- Security patches
- Linux, PHP, MYSQL, Apache updates
- Backups, monitoring and logging


---
layout: image-right
image: https://roots.io/app/uploads/wp-routing-01.svg
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

<!--
- WordPress environment is loaded (core, plugins, theme)
- WordPress looks at URL and builds some query arguments based on it
- Obtained query arguments are used to run a \WP_Query (known as "main query")
- Based on the "type" of the query (eg. "single", "archive"…), WordPress chooses a template file among the ones available in theme
- Template file is loaded to display page
-->

---
layout: image-right
image: 'https://cdn.buttercms.com/ecJRnUxySgel12J15vJA'
---

# Jamstack

### What is it?

- It's not a framework.
- It started as a marketing term.
- It's a way of building websites and apps.

<br />

### Tools and services

- Static site generators
- Headless CMS
- Serverless functions

---
layout: image-right
image: https://miro.medium.com/max/1200/0*XhakmCEGBsQ-ai24.jpg
---

# Let's look into...

### Jamstack Development Flow

<br />

1. <logos-github class="text-3xl" /> Source code in a Git repository
2. <logos-nextjs class="text-3xl" /> Static site generator **(?)**
3. <logos-aws class="text-3xl" /> Serverless functions **(?)**
4. <logos-strapi class="text-3xl" /> Headless CMS to manage content **(?)**
5. <logos-netlify class="text-3xl" /> CDN or static site hosting

<br />

### Tools

Static site generators: **347**

Headless CMS: **96**

---
layout: statement
---

# How to Jamstack?

Typical workflow for building a Jamstack site

<br>

1. <twemoji-pencil /> Write content - Headless CMS, markdown files.
2. <twemoji-laptop /> Write code for the frontend.
3. <twemoji-cloud /> Build locally or in CI, fetch content and convert to static files.
4. <twemoji-rocket /> Deploy static files to a CDN/static site hosting.

<!--
Cache invalidation.
-->

---
layout: image-right
image: ./assets/jamstack-flow.png
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

---
layout: intro-image-right
image: ./assets/sutmm.jpeg
---

# Advantages?

- <twemoji-rocket class="text-xl text-orange-400" /> Faster 
- <twemoji-sparkles />  More secure
- <twemoji-money-mouth-face /> Cheaper, easier to scale and maintain
- <twemoji-robot /> Developer-friendly

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

---
layout: statement
---

# How to create a Jamstack site?

<br />

## Jamstack site with Markdown, Next.js and Neflify

### phplisbon.com

---
layout: intro-image-right
image: https://i.imgflip.com/2vta21.jpg
---

# Thank you!

<br />

<twemoji-clapping-hands class="text-4xl" /> <twemoji-clapping-hands class="text-4xl" /> <twemoji-clapping-hands class="text-4xl" />

<br />
<br />

### You can reach me at

1. <logos-twitter class="text-3xl mx-2" /> <a href="https://twitter.com/iamvarandas">@iamvarandas</a>
2. <logos-github class="text-3xl mx-2" /> <a href="https://github.com/andrevarandas">@andrevarandas</a>
