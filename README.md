carta-renuncia-tex
==================

Esta es una plantilla para LaTeX para generar una carta de renuncia voluntaria basada en el modelo disponible en la [Dirección del Trabajo](http://www.dt.gob.cl/1601/w3-article-94513.html) de Chile.

Uso
---

Configurar los campos de la plantilla en `settings.tex`. Para las fechas se usa el comando `\DTMdisplaydate`, por ejemplo, si la fecha donde se hace efectiva la renuncia es el 18 de septiembre de 2018 debería ir:

```latex
\newcommand*{\ultimoDia}{\DTMdisplaydate{2018}{9}{18}{-1}}
```

Generación del documento
------------------------

Dependerá del sistema, pero en general `pdflatex` es suficiente:

```
pdflatex letter.tex
```

Y generará `letter.pdf`.