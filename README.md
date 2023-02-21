---
title: "Descripcion de Proyecto"
author: "Daniel Behar/Cruz del Cid"
date: "13/11/2022"
---


# Shiny App

## Sección I: Descripcion de la Data.

El dataset `Animated TV Shows Around the World (1948 - 2022)`, extraido de Kaggle, fue el dataset utilizado para armar una aplicación de Shiny que refleje la data. El dataset en la página tiene dos archivos, uno de 1948 hasta 1987 y de 1987 hasta la fecha. Este proyecto solo abarcó el 2do dataset.
Dicho dataset contiene las siguientes variables:
  * `Title`: el nombre de la serie animada.
  * `Seasons`: las temporadas que dicha serie estuvo al aire.
  * `Episodes`: la cantidad de episodios que tuvo en total la serie.
  * `Country`: el o los paises en los que fue lanzado al aire. Solo incluye los paises o el pais donde fue lanzado inicialmente, no los lanzamientos locales que les siguieron.
  * `Premiere Year`: el año en que fue lanzada la serie.
  * `Final Year`: el año en que fue lanzado el último episodio de la serie.
  * `Original Channel`: el canal donde se lanzó al aire la serie por primera vez.
  * `Technique`: la técnica o técnicas que usaron para realizar la serie.

## Sección II: Descripción del proyecto.

El proyecto contiene cuatro páginas principales:
  * `Listado de Series`: la tabla de todas las series con opción de aplicarle filtros para buscar información puntual. Incluye un link que puede mandarse para ver la tabla con los filtros aplicados (esta función trabaja mejor al estar subida a un servidor).
  * `Métricas Generales`: algunas gráficas con información importante del dataset.
  * `Mi Lista`: está la opción de buscar series y seleccionarlas para un tipo de lista con "mis series por ver".
  * `Simulación`: con base en la lista seleccionada y un estimado de episodios que uno estima ver diarios, calcula cuando terminará de ver todas las series seleccionadas.

## Sección III: Dockerfile.

El dockerfile incluye lo necesario para subir el proyecto a un contenedor con Linux corriendo con docker ya instalado. La intención era subirlo a un EC2 de AWS y subirlo a la red.
