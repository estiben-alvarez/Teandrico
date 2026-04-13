---
title: "Artículos"
layout: archive
permalink: /articulos/
author_profile: false
classes: wide
---

<input type="text" id="buscador" placeholder="Buscar artículos..." onkeyup="filtrar()" style="width:100%;padding:0.8rem 1rem;border:1px solid #e5e5e0;font-size:1rem;margin-bottom:2rem;font-family:'Helvetica Neue',Arial,sans-serif;outline:none;">

<div id="lista-articulos">
{% include archive-list-custom.html %}
</div>

<script>
function filtrar() {
  var texto = document.getElementById('buscador').value.toLowerCase();
  var articulos = document.querySelectorAll('.article-list-item');
  articulos.forEach(function(articulo) {
    var contenido = articulo.innerText.toLowerCase();
    if (contenido.includes(texto)) {
      articulo.style.display = 'flex';
    } else {
      articulo.style.display = 'none';
    }
  });
}
</script>
