## Análisis cualitativo para grandes volúmenes de texto con LLMs

## Keywords: NLP, Gemini, Ingeniería de Prompts, Análisis cualitativo, Noticias

## Resúmen

El desarrollo de la IA y los modelos generativos potencian el análisis cualitativo de textos para diversas disciplinas. Este tutorial aprovecha los créditos gratuitos de la API de Gemini de Google para enseñar a usar LLMs en R, un entorno amigable para el PLN. Se abordará un flujo de trabajo estructurado, desde el diseño y optimización de prompts y sus parámetros, hasta la iteración en dataframes para obtener salidas estructuradas, limpiar datos y finalmente, usar embeddings para visualizaciones.

En este marco, los objetivos planteados son:

-   El/la estudiante **comprenderá** los beneficios de usar LLMs para el análisis de texto.

-   El/la estudiante **diseñará** prompts para análisis cualitativo y **creará** criterios para evaluar los resultados del LLMs.

-   El/la estudiante **ajustará** los parámetros del modelo y los prompts para apuntar a resultados rigurosos y reproducibles.

-   El/la estudiante **automatizará** el análisis de texto en R con funciones e iteraciones para obtener un objeto estructurado.

-   El/la estudiante **analizará** la información resultante mediante visualizaciones y estadística descriptiva.

## ¿A quiénes está dirigido el tutorial?

Este tutorial está dirigido a investigadores, estudiantes y profesionales de cualquier disciplina (ciencias sociales, humanidades, ciencias de la salud, etc.) que trabajen con datos de texto y deseen potenciar sus análisis cualitativos mediante herramientas de IA.

Para aprovechar al máximo el taller, los participantes deben tener un conocimiento básico-intermedio de R. Específicamente, se espera que puedan:

1.  Entender y escribir funciones simples.

2.  Utilizar bucles for para iterar sobre elementos.

3.  Manejar datos tabulares con las funciones principales del paquete dplyr (como mutate, filter, select).

No se requiere experiencia previa con APIs, Procesamiento de Lenguaje Natural (PLN) o modelos de lenguaje.

A continuación, se presentan dos personas tipo ideales para este taller:

Persona 1:

-   David es un sociólogo que investiga el discurso público en redes sociales. Actualmente, está analizando el debate en torno a una nueva política medioambiental.

-   Se siente cómodo usando R para análisis estadístico y `dplyr` para limpiar y transformar datos. Ha usado for loops, aunque a veces le cuestan un poco. No tiene ninguna experiencia con IA o APIs.

-   David ha recolectado miles de comentarios de una plataforma online y necesita clasificarlos. Quiere ir más allá de un simple análisis de sentimiento y extraer los argumentos principales que usan las personas (ej. "impacto económico", "justicia climática", "desconfianza en el gobierno"). Hacer esto a mano para todo el volumen de datos es inviable.

-   Al no tener formación en programación, David necesita un flujo de trabajo muy claro y bien documentado que le permita aplicar los conceptos de análisis cualitativo que ya conoce, pero usando código de manera reproducible.

Persona 2:

-   Sofía es una investigadora en salud pública que trabaja con transcripciones de entrevistas semi-estructuradas a pacientes con enfermedades crónicas.

-   Tiene un nivel intermedio de R y del tidyverse. Ha creado sus propias funciones para automatizar tareas repetitivas de limpieza y se siente segura con las iteraciones.

-   Su objetivo es identificar y sistematizar las barreras de acceso al sistema de salud mencionadas por los pacientes en las entrevistas. Busca un método que le permita extraer esta información de manera estructurada (por ejemplo, en un dataframe con columnas para "tipo de barrera", "contexto", "cita textual") para luego analizarla cuantitativamente.

-   A Sofía le preocupa mucho la rigurosidad y la transparencia metodológica. Le interesa especialmente aprender a diseñar y optimizar "prompts" para asegurar que los resultados del modelo de IA sean consistentes, fiables y poder justificar su método en una publicación científica.

## Máximo de integrantes: 30

## Duración: 135 minutos

## Estructura del tutorial

El tutorial se compondrá de dos bloques y considera una pausa intermedia de aproximadamente 15 minutos. En la primera sección, se abordarán los antecedentes generales del taller, como la relevancia, contexto, funcionamiento de la tecnología, etc. Además, se configurará la sesión y llevarán a cabo los preparativos necesarios para que la parte práctica funcione bien. Luego, en una segunda sección, se realizará el núcleo del taller, ejecutando el flujo de trabajo con LLMs planteado y finalizando con un análisis breve de los resultados obtenidos. Ambas secciones serán de aproximadamente una hora.

## Requerimientos

Versión mínima de R 4.1, paquetes instalados 'gemini.R', 'datamedios', 'dplyr', 'purrr', 'ggplot2', 'jsonlite' (todos disponibles en CRAN), ojalá que tengan una API de google ya habilitada (se puede crear una API KEY en https://aistudio.google.com/apikey, si tienen problemas igualmente se abordará en el tutorial).

## Instructores

En el taller participarán dos personas como instructores, ambos integrantes de la organización Socialtec (https://socialtec.cl/quienes-somos/) y estudiantes de sociología de la Universidad de Chile. Ismael Aguayo (https://github.com/ismaelaguayob) es asistente de investigación en el núcleo milenio NUDOS y ayudante de estadística y métodos computacionales, con interes en la Ciencia de Datos y la inteligencia artificial. Exequiel Trujillo (https://github.com/exetrujillo) es desarrollador web y ayudante de métodos computacionales, y se encuentra estudiando ciberseguridad y sociología de la música a través de análisis computacional.

## Recursos

Link al repositorio del tutorial (trabajo en progreso, con la mayoría del código ya escrito): https://github.com/ismaelaguayob/taller-gemini-datamedios