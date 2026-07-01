---
layout: archive
author_profile: true
classes: wide
header:
  overlay_image: /imagenes/clubes-juveniles.jpg
  overlay_filter: 0.6
  actions:
    - label: "Unirme al Club de Lectura"
      url: /club-de-lectura/
    - label: "Sobre el Proyecto"
      url: /sobre-el-proyecto/
excerpt: "Un espacio dedicado a la divulgación y el diálogo sobre teología, religión, espiritualidad y fe, desde una aproximación académica y científica."
title: "Haciendo teología en el continente digital"
---

<h3 class="archive__subtitle">Lo más reciente</h3>

<div style="position:relative;overflow:hidden;margin-bottom:3rem;">
  <div id="carrusel" style="display:flex;transition:transform 0.5s ease;will-change:transform;">
    {% assign todo = site.posts | concat: site.noticias | sort: 'date' | reverse %}
    {% for post in todo %}
    <div style="min-width:100%;box-sizing:border-box;padding:0 0.5rem;">
      <div class="article-list-item" style="display:flex;gap:1.5rem;align-items:flex-start;padding:1.5rem;background:#ffffff;border:1px solid #e5e5e0;border-radius:8px;">
        {% if post.header.teaser %}
        <a href="{{ post.url }}" style="flex-shrink:0;">
          <img src="{{ post.header.teaser }}" alt="{{ post.title }}" style="width:200px;height:140px;object-fit:cover;display:block;">
        </a>
        {% endif %}
        <div style="flex:1;">
          <h3 style="font-family:Georgia,serif;font-size:1.1rem;font-weight:normal;margin:0 0 0.4rem 0;line-height:1.4;">
            <a href="{{ post.url }}" style="color:#1a1a1a;text-decoration:none;">{{ post.title }}</a>
          </h3>
          <p style="font-size:0.78rem;color:#aaa;margin:0 0 0.6rem 0;">{{ post.date | date: "%B %d, %Y" }}</p>
          <p style="font-size:0.9rem;color:#444;margin:0 0 1rem 0;line-height:1.6;">{{ post.excerpt | strip_html | truncate: 200 }}</p>
          <a href="{{ post.url }}" style="display:inline-block;padding:0.4rem 1rem;background:#1a1a1a;color:#fff!important;text-decoration:none;font-size:0.78rem;letter-spacing:0.05em;text-transform:uppercase;">Leer más</a>
        </div>
      </div>
    </div>
    {% endfor %}
  </div>
  <button onclick="moverCarrusel(-1)" style="position:absolute;left:0;top:50%;transform:translateY(-50%);background:#f5c842;border:none;padding:0.5rem 1rem;cursor:pointer;font-size:1.2rem;z-index:10;color:#1a1a1a!important;">‹</button>
  <button onclick="moverCarrusel(1)" style="position:absolute;right:0;top:50%;transform:translateY(-50%);background:#f5c842;border:none;padding:0.5rem 1rem;cursor:pointer;font-size:1.2rem;z-index:10;color:#1a1a1a!important;">›</button>
</div>

<script>
  var actual = 0;
  var total = {{ site.posts.size | plus: site.noticias.size }};

  function moverCarrusel(dir) {
    actual = (actual + dir + total) % total;
    document.getElementById('carrusel').style.transform = 'translateX(-' + (actual * 100) + '%)';
  }

  setInterval(function() {
    moverCarrusel(1);
  }, 5000);
</script>

<div style="background:#f5f5f0;border:1px solid #e5e5e0;padding:1.5rem;margin-bottom:2rem;">
  <div style="font-size:0.7rem;letter-spacing:0.1em;text-transform:uppercase;background:#f5c842;color:#1a1a1a;display:inline-block;padding:0.15rem 0.5rem;margin-bottom:1rem;">Eventos</div>
  <div style="display:flex;gap:1.5rem;flex-wrap:wrap;">

    <!-- EVENTO: Coloquio Internacional de Teología (TeoRed), octubre 2026 -->
    <div style="flex:1;min-width:200px;border-left:3px solid #f5c842;padding-left:1rem;">
      <div style="display:flex;align-items:center;gap:0.4rem;margin-bottom:0.4rem;">
        <svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="#f5c842" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="4" width="18" height="18" rx="2" ry="2"></rect><line x1="16" y1="2" x2="16" y2="6"></line><line x1="8" y1="2" x2="8" y2="6"></line><line x1="3" y1="10" x2="21" y2="10"></line></svg>
        <span style="font-size:0.78rem;color:#6b6b6b;">Octubre 21 y 22 de 2026</span>
      </div>
      <h3 style="font-family:Georgia,serif;font-weight:normal;margin:0 0 0.3rem 0;font-size:1rem;">Coloquio Internacional de Teología (TeoRed)</h3>
      <p style="font-size:0.82rem;color:#6b6b6b;margin:0 0 0.8rem 0;">Presencial y virtual · Fundación Universitaria Católica del Norte</p>
      <a href="/noticias/coloquio-internacional-teologia/" style="display:inline-block;padding:0.4rem 1rem;background:#1a1a1a;color:#fff!important;text-decoration:none;font-size:0.78rem;border-radius:4px;">Más información</a>
    </div>
    
  </div>
</div>

<div style="background:#f5f5f0;border:1px solid #e5e5e0;padding:1.5rem;margin-bottom:2rem;display:flex;gap:1.5rem;align-items:center;flex-wrap:nowrap;"><img src="/imagenes/libro-jesus-aproximacion-historica.jpg" alt="Jesús: Aproximación histórica" style="width:80px;box-shadow:0 4px 12px rgba(0,0,0,0.2);flex-shrink:0;"><div style="flex:1;"><div style="font-size:0.7rem;letter-spacing:0.1em;text-transform:uppercase;background:#f5c842;color:#1a1a1a;display:inline-block;padding:0.15rem 0.5rem;margin-bottom:0.5rem;">Club de Lectura</div><h3 style="font-family:Georgia,serif;font-weight:normal;margin:0 0 0.2rem 0;font-size:1.1rem;">Jesús: Aproximación histórica</h3><p style="color:#6b6b6b;margin:0 0 0.5rem 0;font-size:0.85rem;">José Antonio Pagola</p><p style="margin:0 0 1rem 0;font-size:0.9rem;">Estamos leyendo juntos una de las obras más rigurosas sobre el Jesús histórico.</p><a href="/club-de-lectura/" style="display:inline-block;padding:0.5rem 1.2rem;background:#1a1a1a;color:#fff!important;text-decoration:none;font-size:0.85rem;border-radius:4px;">Ver más</a></div></div>
