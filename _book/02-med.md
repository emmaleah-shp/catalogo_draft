--- 
title: "Medio Ambiente"
site: bookdown::bookdown_site
output: bookdown::bs4_book
---

# Ámbito Medio Ambiente
Descripción acá...

## Instituciones participantes {-}
*Grupo Biodiversidad y Ecosistemas*
Dirección General de Aguas – Ministerio de Obras Públicas 
División de Información y Economía Ambiental – Ministerio del Medio Ambiente 
Centro de Ciencia del Clima y la Resiliencia – Universidad de Chile 
Subsecretaría de Desarrollo Regional y Administrativo – Ministerio del Interior y Seguridad Pública 
Sistema Nacional de Información Ambiental – Ministerio del Medio Ambiente 

*Grupo Contaminación*
División de Información y Economía Ambiental – Ministerio de Medio Ambiente 
División de Políticas Públicas Saludables y Promoción - Ministerio de Salud 
Consejo Nacional de Desarrollo Urbano 

*Grupo Institucionalidad y Monitoreo Ambiental*
División de Calidad del Aire – Ministerio del Medio Ambiente 
Dirección General de Aguas – Ministerio de Obras Públicas 
División de Educación Ambiental y Participación Ciudadana – Ministerio del Medio Ambiente 
Servicio de Evaluación Ambiental – Ministerio del Medio Ambiente 
Subsecretaría de Desarrollo Regional y Administrativo – Ministerio del Interior y Seguridad Pública 
Superintendencia de Servicios Sanitarios  


## Chapters and sub-chapters {-}

There are two steps to cross-reference any heading:

1. Label the heading: `# Hello world {#nice-label}`. 
    - Leave the label off if you like the automated heading generated based on your heading title: for example, `# Hello world` = `# Hello world {#hello-world}`.
    - To label an un-numbered heading, use: `# Hello world {-#nice-label}` or `{# Hello world .unnumbered}`.

1. Next, reference the labeled heading anywhere in the text using `\@ref(nice-label)`; for example, please see Chapter

## Captioned figures and tables {-}

Figures and tables *with captions* can also be cross-referenced from elsewhere in your book using `\@ref(fig:chunk-label)` and `\@ref(tab:chunk-label)`, respectively.

See Figure \@ref(fig:nice-fig).


```r
par(mar = c(4, 4, .1, .1))
plot(pressure, type = 'b', pch = 19)
```

<div class="figure" style="text-align: center">
<img src="02-med_files/figure-html/nice-fig-1.png" alt="Plot with connected points showing that vapor pressure of mercury increases exponentially as temperature increases." width="80%" />
<p class="caption">(\#fig:nice-fig)Here is a nice figure!</p>
</div>

Don't miss Table \@ref(tab:nice-tab).


```r
knitr::kable(
  head(pressure, 10), caption = 'Here is a nice table!',
  booktabs = TRUE
)
```



Table: (\#tab:nice-tab)Here is a nice table!

| temperature| pressure|
|-----------:|--------:|
|           0|    0.000|
|          20|    0.001|
|          40|    0.006|
|          60|    0.030|
|          80|    0.090|
|         100|    0.270|
|         120|    0.750|
|         140|    1.850|
|         160|    4.200|
|         180|    8.800|


