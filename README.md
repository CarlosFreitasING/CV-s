# Currículum de Carlos Alejandro Freitas Teixeira

Este repositorio reúne mi currículum en español, inglés y portugués de Portugal, tanto en versiones ATS como en versiones visuales para mostrar en una web.

## Versiones ATS

| Idioma | PDF | Fuente LaTeX |
|---|---|---|
| Español | [PDF](curriculum_es.pdf) | [LaTeX](curriculum_es.tex) |
| English | [PDF](curriculum_en.pdf) | [LaTeX](curriculum_en.tex) |
| Português | [PDF](curriculum_pt.pdf) | [LaTeX](curriculum_pt.tex) |

## Versiones visuales

| Idioma | PDF | Fuente LaTeX |
|---|---|---|
| Español | [PDF](curriculum_es_web.pdf) | [LaTeX](curriculum_es_web.tex) |
| English | [PDF](curriculum_en_web.pdf) | [LaTeX](curriculum_en_web.tex) |
| Português | [PDF](curriculum_pt_web.pdf) | [LaTeX](curriculum_pt_web.tex) |

Las versiones visuales incluyen una fotografía de perfil y están pensadas para presentación web, no para procesos ATS. La imagen utilizada está en [`assets/foto.jpeg`](assets/foto.jpeg).

## Compilación

Los documentos se compilan con pdfLaTeX. Ejecuta el comando dos veces para actualizar enlaces y referencias:

```powershell
pdflatex -interaction=nonstopmode -halt-on-error -jobname=curriculum_es_web curriculum_es_web.tex
```

Sustituye `curriculum_es_web` por el nombre del archivo que quieras compilar.
