---
name: CV LaTeX ATS
description: "Use when creating or editing this LaTeX curriculum vitae, résumé, or CV. Follow the ATS-friendly layout and content rules."
applyTo: "**/*.tex"
---

# Instrucciones para el currículum en LaTeX

Usa `curriculum_es.tex` como versión de referencia en español. Las versiones traducidas son `curriculum_en.tex` (inglés) y `curriculum_pt.tex` (portugués de Portugal); mantenlas alineadas en datos, fechas, enlaces, habilidades y estructura, sin alterar los hechos al traducir.

## Estructura y diseño

- Usa un diseño de una sola columna con flujo de lectura de arriba abajo y de izquierda a derecha.
- No uses `multicol`, tablas (`tabular`, `tabularx`, `longtable`) para organizar contenido, ni paneles laterales.
- No incluyas foto, gráficos ni iconos; presenta los datos de contacto como texto legible.
- No uses líneas horizontales entre experiencias; sepáralas solo con una línea vacía de espaciado vertical, salvo que el usuario indique lo contrario.
- Da a cada experiencia un encabezado claro: cargo en una línea propia, en negrita y algo mayor; empresa, ubicación y fechas debajo, con una línea vacía de separación entre experiencias.
- En la experiencia freelance, describe el alcance y las competencias de forma general; no nombres páginas, productos o clientes específicos salvo que el usuario lo solicite.
- Mantén coherencia en las experiencias: cuando se indique el stack, incluye una última viñeta `Stack Tecnológico` con las tecnologías confirmadas, también en la experiencia freelance.
- Evita duplicar en la viñeta de stack las tecnologías ya enumeradas en los puntos de la experiencia; usa los puntos para describir responsabilidades y resultados, y el stack para nombrar herramientas.
- Usa una tipografía estándar sans-serif como Helvetica, Arial o equivalente; mantén el cuerpo entre 10 y 12 pt.
- Mantén una jerarquía tipográfica clara: encabezados de sección en negrita de 14 a 16 pt, títulos de puesto diferenciados y legibles, y cuerpo de 10 a 12 pt.
- Usa márgenes razonables y la clase `article` con `geometry` cuando sea apropiado.
- Conserva los encabezados de sección del currículum: Resumen Profesional, Experiencia Profesional, Educación, Publicaciones y Conferencias, y Habilidades Técnicas.
- Usa `itemize` para las viñetas.
- Para enlaces, usa `\href{url}{texto visible}` de `hyperref`. El texto visible debe ser breve, descriptivo y legible; nunca muestres URLs largas o kilométricas en el cuerpo del CV.
- Haz que los hipervínculos sean visualmente identificables, por ejemplo usando un color discreto, sin sacrificar la legibilidad al imprimir.
- Inserta los enlaces en palabras relevantes que ya formen parte del contenido, por ejemplo `\href{url}{App Store}`, `\href{url}{Google Play}`, el título de una publicación o el nombre de un proyecto.
- No uses iconos ni logotipos para enlaces, incluidos los de Android, Apple y GitHub. No cargues FontAwesome ni fuentes de iconos.
- No inventes URLs. Si el usuario comparte un enlace directo a una tienda, PWA, portafolio o publicación, incrústalo en el texto correspondiente con `\href`; si no lo comparte, deja el texto sin enlazar.
- Si alineas fechas, hazlo sin tablas, por ejemplo con espaciado horizontal (`\hfill`).

## Compatibilidad y validación

Prioriza texto seleccionable, orden de lectura natural y extracción clara del contenido. No prometas compatibilidad del 100 % con todos los ATS: los parsers varían. Cuando sea posible, compila el PDF y comprueba que el texto extraído conserva el orden y los caracteres correctamente.
