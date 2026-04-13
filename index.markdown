---
layout: archive
author_profile: true
classes: wide
header:
  overlay_image: /imagenes/imagen-principal.jpg
  overlay_filter: 0.6
  actions:
    - label: "Explorar artículos"
      url: /articulos/
    - label: "Sobre el Proyecto"
      url: /sobre-el-proyecto/
excerpt: "Un espacio dedicado a la divulgación teológica a partir de la reflexión académica."
title: "Haciendo teología en el continente digital"
---

<div style="background:#f5f5f0;border:1px solid #e5e5e0;padding:1.5rem;margin-bottom:3rem;display:flex;gap:1.5rem;align-items:center;flex-wrap:nowrap;">
  <img src="/imagenes/libro-jesus-aproximacion-historica.jpg" alt="Jesús: Aproximación histórica" style="width:80px;box-shadow:0 4px 12px rgba(0,0,0,0.2);flex-shrink:0;">
  <div style="flex:1;">
    <div style="font-size:0.7rem;letter-spacing:0.1em;text-transform:uppercase;background:#f5c842;color:#1a1a1a;display:inline-block;padding:0.15rem 0.5rem;margin-bottom:0.5rem;">Club de Lectura</div>
    <h3 style="font-family:Georgia,serif;font-weight:normal;margin:0 0 0.2rem 0;font-size:1.1rem;">Jesús: Aproximación histórica</h3>
    <p style="color:#6b6b6b;margin:0 0 0.5rem 0;font-size:0.85rem;">José Antonio Pagola</p>
    <p style="margin:0 0 1rem 0;font-size:0.9rem;">Estamos leyendo juntos una de las obras más rigurosas sobre el Jesús histórico.</p>
    <a href="/club-de-lectura/" style="display:inline-block;padding:0.5rem 1.2rem;background:#1a1a1a;color:#fff!important;text-decoration:none;font-size:0.85rem;border-radius:4px;">Ver más</a>
  </div>
</div>

<div style="background:#f5f5f0;border:1px solid #e5e5e0;padding:1.5rem;margin-bottom:3rem;display:flex;gap:1.5rem;align-items:center;flex-wrap:nowrap;">
  <div style="flex-shrink:0;width:80px;height:80px;background:linear-gradient(45deg,#f09433,#e6683c,#dc2743,#cc2366,#bc1888);border-radius:16px;display:flex;align-items:center;justify-content:center;">
    <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 24 24" fill="white"><path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zM12 0C8.741 0 8.333.014 7.053.072 2.695.272.273 2.69.073 7.052.014 8.333 0 8.741 0 12c0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98C8.333 23.986 8.741 24 12 24c3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98C15.668.014 15.259 0 12 0zm0 5.838a6.162 6.162 0 1 0 0 12.324 6.162 6.162 0 0 0 0-12.324zM12 16a4 4 0 1 1 0-8 4 4 0 0 1 0 8zm6.406-11.845a1.44 1.44 0 1 0 0 2.881 1.44 1.44 0 0 0 0-2.881z"/></svg>
  </div>
  <div style="flex:1;">
    <div style="font-size:0.7rem;letter-spacing:0.1em;text-transform:uppercase;background:#f5c842;color:#1a1a1a;display:inline-block;padding:0.15rem 0.5rem;margin-bottom:0.5rem;">Instagram</div>
    <h3 style="font-family:Georgia,serif;font-weight:normal;margin:0 0 0.2rem 0;font-size:1.1rem;">Síguenos en Instagram</h3>
    <p style="margin:0 0 1rem 0;font-size:0.9rem;">Contenido teológico, reflexiones y novedades del proyecto.</p>
    <a href="https://www.instagram.com/teandrico_blog/" target="_blank" style="display:inline-block;padding:0.5rem 1.2rem;background:linear-gradient(45deg,#f09433,#dc2743,#bc1888);color:#fff!important;text-decoration:none;font-size:0.85rem;border-radius:4px;">Seguir en Instagram</a>
  </div>
</div>

<h3 class="archive__subtitle">Artículos recientes</h3>

<div style="position:relative;overflow:hidden;margin-bottom:3rem;">
  <div id="carrusel" style="display:flex;transition:transform 0.5s ease;will-change:transform;">
    {% for post in site.posts %}
    <div style="min-width:100%;box-sizing:border-box;padding:0 0.5rem;">
      <div style="display:flex;gap:1.5rem;align-items:flex-start;background:#fff;border:1px solid #e5e5e0;padding:1.5rem;">
        {% if post.header.teaser %}
        <a href="{{ post.url }}" style="flex-shrink:0;">
          <img src="{{ post.header.teaser }}" alt="{{ post.title }}" style="width:180px;height:130px;object-fit:cover;">
        </a>
        {% endif %}
        <div>
          <h3 style="font-family:Georgia,serif;font-size:1.2rem;font-weight:normal;margin:0 0 0.5rem 0;">
            <a href="{{ post.url }}" style="color:#1a1a1a;text-decoration:none;">{{ post.title }}</a>
          </h3>
          <p style="font-size:0.8rem;color:#aaa;margin:0 0 0.5rem 0;">{{ post.date | date: "%B %d, %Y" }}</p>
          <p style="font-size:0.9rem;color:#444;margin:0;">{{ post.excerpt | strip_html | truncate: 200 }}</p>
          <a href="{{ post.url }}" style="display:inline-block;margin-top:0.8rem;font-size:0.8rem;color:#1a1a1a;text-decoration:underline;">Leer más →</a>
        </div>
      </div>
    </div>
    {% endfor %}
  </div>

  <button onclick="moverCarrusel(-1)" style="position:absolute;left:0;top:50%;transform:translateY(-50%);background:#f5c842;border:none;padding:0.5rem 1rem;cursor:pointer;font-size:1.2rem;z-index:10;">‹</button>
  <button onclick="moverCarrusel(1)" style="position:absolute;right:0;top:50%;transform:translateY(-50%);background:#f5c842;border:none;padding:0.5rem 1rem;cursor:pointer;font-size:1.2rem;z-index:10;">›</button>
</div>

<script>
  var actual = 0;
  var total = {{ site.posts.size }};

  function moverCarrusel(dir) {
    actual = (actual + dir + total) % total;
    document.getElementById('carrusel').style.transform = 'translateX(-' + (actual * 100) + '%)';
  }

  setInterval(function() {
    moverCarrusel(1);
  }, 5000);
</script>
