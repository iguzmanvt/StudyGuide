# StudyGuide: guía de crecimiento económico

Este repositorio conserva un fork de [dvollrath/StudyGuide](https://github.com/dvollrath/StudyGuide), la guía de Dietrich Vollrath para un curso basado en Jones y Vollrath. Los materiales originales están en inglés. Se mantiene la [licencia MIT original](LICENSE), con copyright de 2020; esta copia no atribuye la autoría del curso a su propietario del fork.

## Ruta de lectura

El [índice original](index.md) explica el enfoque y su relación con el libro. Para recorrer los materiales en GitHub, sigue este orden:

| Orden | Tema | Entrada |
| ---: | --- | --- |
| 1 | Introducción | [Introduction](intro/introduction.md) |
| 2 | Herramientas matemáticas | [Preliminaries](preliminaries/preliminaries.md) |
| 3 | Medición del PIB | [Measuring GDP](gdp/gdp.md) |
| 4 | Hechos estilizados | [Growth facts](facts/facts.md) |
| 5 | Solow y crecimiento equilibrado | [Solow and Balanced Growth](solow/solow.md) |
| 6 | Ideas y productividad | [Ideas and Productivity](ideas/ideas.md) |
| 7 | Desarrollo comparado | [Comparative Development](develop/develop.md) |
| 8 | Población y recursos | [Population and Resources](population/population.md) |
| 9 | Evaluaciones del curso original | [Test material](tests/tests.md) |

`tests/` contiene materiales docentes de evaluación, según su página de entrada. No representa una suite de pruebas de software.

## Código, datos y salidas

Los [datos](data/) incluyen CSV utilizados por el material original. [plotly/](plotly/) y otras carpetas conservan HTML y bibliotecas asociadas: al descargar una salida para consulta local, conserva su estructura de recursos. La [fuente Quarto de Solow](solow/quarto-solow.qmd) se mantiene junto a sus materiales.

La inspección de los cuatro `app.R` identifica estos prototipos Shiny y sus dependencias declaradas `shiny`, `rsconnect` y `ggplot2`:

| Aplicación | Código |
| --- | --- |
| Modelo dinámico simple | [BabyBasic](code/BabyBasic/app.R) |
| Cálculo del PIB real | [GDPBasic](code/GDPBasic/app.R) |
| Modelo malthusiano | [PopBasic](code/PopBasic/app.R) |
| Modelo de productividad | [ProdBasic](code/ProdBasic/app.R) |

Esta revisión comprobó su presencia y leyó sus declaraciones de dependencias; no ejecutó las aplicaciones ni revalidó sus cálculos. Los datos y gráficos conservan sus ediciones históricas.

## Configuración y mantenimiento

La [configuración Jekyll](_config.yml) conserva el tema remoto `just-the-docs/just-the-docs`, la base `/StudyGuide` y el dominio original `https://growthecon.com`. Una publicación en otro dominio requiere revisar esa configuración y los vínculos del contenido. Este README guía la lectura del repositorio; no acredita una compilación completa del sitio.

El mantenimiento del 11 de noviembre de 2026 sustituyó el README provisional por este índice y corrigió el enlace de licencia del pie de página, conservando el crédito del autor. Se retiraron 13 archivos de metadatos de Finder y un historial R vacío. Los cuatro historiales R con contenido permanecen versionados; `.gitignore` evita añadir nuevos historiales de consola y metadatos de Finder.

La limpieza conserva las páginas docentes, los datos, las aplicaciones, los HTML, sus bibliotecas y la licencia. No se eliminaron bibliotecas repetidas que puedan formar parte de las dependencias de cada salida. La revisión cubre organización, procedencia y enlaces de esta entrada; la ejecución de aplicaciones, la compilación del sitio y la validación económica requieren comprobaciones propias.
