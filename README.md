title: "Examen Final"
description: "Sitio web de examen final creado por GENESIS SALINAS"
baseurl: "" # Si usas un repositorio tipo tu-usuario.github.io
url: "https://tu-usuario.github.io" # Reemplaza con tu nombre de usuario real

author:
  name: "GENESIS SALINAS"

theme: minima

collections:
  examen_final_genesis:
    output: true
    permalink: /examen_final_genesis/:title/
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <title>{{ page.title }} - Examen Final</title>
</head>
<body>
  <header>
    <h1>Examen Final - GENESIS SALINAS</h1>
    <nav>
      <a href="{{ '/' | relative_url }}">Inicio</a> |
      <a href="{{ '/about.html' | relative_url }}">Acerca de</a> |
      <a href="{{ '/contact.html' | relative_url }}">Contacto</a> |
      <a href="{{ '/examen_final_genesis.html' | relative_url }}">Examen Final Genesis</a>
    </nav>
  </header>

  <main>
    {{ content }}
  </main>

  <footer>
    <p>© 2025 GENESIS SALINAS</p>
  </footer>
</body>
</html>
---
title: "Elemento Uno"
date: 2025-06-07
description: "Primer elemento de la colección Examen Final Genesis."
---

Contenido del **Elemento Uno** para la colección Examen Final Genesis.
---
title: "Elemento Dos"
date: 2025-06-08
description: "Segundo elemento de la colección Examen Final Genesis."
---

Contenido del **Elemento Dos** con más información para mostrar.
---
layout: default
title: Inicio
---

Bienvenido al sitio creado por **GENESIS SALINAS** para el examen final.
---
layout: default
title: Acerca de
---

Este sitio fue creado por **GENESIS SALINAS** como parte del examen final.

En esta página podrás conocer más sobre el propósito del sitio y el autor.
---
layout: default
title: Contacto
---

Si deseas contactarme, puedes enviarme un correo a: [genesis.salinas@email.com](mailto:genesis.salinas@email.com)
---
layout: default
title: Examen Final Genesis
---

# Lista de Elementos - Examen Final Genesis

<ul>
  {% for item in site.examen_final_genesis %}
    <li>
      <a href="{{ item.url }}">{{ item.title }}</a> — {{ item.description }}
    </li>
  {% endfor %}
</ul>

