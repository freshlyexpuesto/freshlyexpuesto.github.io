<!DOCTYPE html>
<html lang="{{ site.lang | default: "en-US" }}">
  <head>
    <meta charset="UTF-8">

{% seo title=false %}
    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link rel="preload" href="https://fonts.googleapis.com/css?family=Open+Sans:400,700&display=swap" as="style" type="text/css" crossorigin>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="theme-color" content="#157878">
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <meta name="description" content="{{ page.meta_description | default: page.description | default: site.description }}">
    <meta name="keywords" content="freshly,freshly cosmetics,cosmètica natural,cosmètica vegana,cosmètica cruelty-free, freshly ere, freshly ero">
    <title>{{ page.meta_title | default: page.title | default: site.title }}</title>
    <link rel="stylesheet" href="{{ '/assets/css/style.css?v=' | append: site.github.build_revision | relative_url }}">
    {% include head-custom.html %}
  </head>
  <body>
    <a id="skip-to-content" href="#content">Skip to the content.</a>

    <header class="page-header" role="banner">
      <h1 class="project-name">{{  page.title | default: site.title }}</h1>
      <h2 class="project-tagline">{{ page.description | default: site.description }}</h2>
      <a href="/testimonios-freshly" class="btn">🔥 Testimonios</a>
      <a href="/censura-en-comentarios-redes-sociales-freshly" class="btn">🤐 Censura</a>
      <a href="/" class="btn">català</a>
      <a href="/es" class="btn">Castellano</a>
    </header>

    <main id="content" class="main-content" role="main">
      {{ content }}

      <footer class="site-footer">
        {% if site.github.is_project_page %}
          <span class="site-footer-owner"><a href="{{ site.github.repository_url }}">{{ site.github.repository_name }}</a> is maintained by <a href="{{ site.github.owner_url }}">{{ site.github.owner_name }}</a>.</span>
        {% endif %}
      </footer>
    </main>
  </body>
</html>
