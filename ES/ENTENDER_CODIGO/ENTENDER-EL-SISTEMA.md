# Prompt para analizar y comprender un proyecto existente mediante ingeniería inversa

Quiero que actúes como mi mentor de programación mientras analizo y comprendo mediante ingeniería inversa un proyecto de software existente.

NO intentes explicarme todo el código del proyecto de una sola vez.

Mi objetivo es construir un modelo mental del proyecto que me permita, con el tiempo, orientarme y comprenderlo de forma autónoma.

## MI NIVEL

Llevo aproximadamente un año aprendiendo Python por mi cuenta.

Conozco los fundamentos de Python y he desarrollado proyectos, pero tengo dificultades cuando los proyectos se vuelven grandes e incluyen múltiples componentes, bibliotecas, abstracciones y patrones arquitectónicos.

No des por hecho que comprendo una biblioteca, un framework, un patrón arquitectónico o una abstracción simplemente porque conozco Python.

## MI OBJETIVO

Ayúdame a comprender:

* Qué hace el proyecto.
* Cómo está organizado.
* Dónde comienza la ejecución.
* Cómo fluyen los datos a través del sistema.
* Cuáles son los componentes principales.
* Qué responsabilidad tiene cada componente.
* Por qué se utilizan determinadas bibliotecas.
* Cómo se comunican los componentes.
* Dónde se encuentra la lógica de negocio.
* Cómo se almacenan y recuperan los datos.
* Cómo se gestionan los errores.
* Cómo se prueba el proyecto.
* Qué partes son importantes y cuáles corresponden a la infraestructura.

## FASE 1 — VISIÓN GENERAL DE ALTO NIVEL

Antes de examinar en profundidad los archivos individuales, explícame:

1. ¿Qué problema resuelve este proyecto?
2. ¿Cuáles son sus principales entradas?
3. ¿Cuáles son sus principales salidas?
4. ¿Cuáles son sus componentes principales?
5. ¿Qué tecnologías y bibliotecas utiliza?
6. ¿Cómo se comunican los componentes principales?
7. ¿Cómo es, a grandes rasgos, la arquitectura general?

Proporcióname un modelo mental sencillo o un diagrama si resulta útil.

Todavía NO expliques las funciones individuales.

## FASE 2 — ESTRUCTURA DEL PROYECTO

Ayúdame a comprender la estructura de carpetas y archivos.

Para cada directorio importante, explícame:

* ¿Qué responsabilidad tiene?
* ¿Qué tipo de código debe contener?
* ¿Qué tipo de código NO debería contener?
* ¿Cómo interactúa con los demás directorios?

No expliques cada archivo individualmente.

Céntrate en la estructura y las responsabilidades.

## FASE 3 — SEGUIR UNA FUNCIONALIDAD DE PRINCIPIO A FIN

Elige una funcionalidad sencilla y representativa, y síguela a través de toda la aplicación.

Por ejemplo:

```text
Solicitud
   ↓
Router / Controlador
   ↓
Servicio
   ↓
Repositorio
   ↓
Base de datos
   ↓
Respuesta
```

Explícame qué sucede en cada etapa.

Para cada etapa, dime:

* ¿Cuál es su responsabilidad?
* ¿Qué datos recibe?
* ¿Qué devuelve?
* ¿Quién la llama?
* ¿Qué componente llama al siguiente?
* ¿Por qué este componente está separado de los demás?

Esto es extremadamente importante, porque quiero comprender cómo encajan todas las piezas entre sí.

## FASE 4 — COMPRENDER LOS COMPONENTES IMPORTANTES

Cuando examinemos una clase, función o módulo importante, explícamelo siguiendo este orden:

1. ¿Qué problema resuelve?
2. ¿Por qué existe?
3. ¿Quién lo utiliza?
4. ¿Qué recibe?
5. ¿Qué produce?
6. ¿De qué depende?
7. ¿Qué elementos dependen de él?
8. ¿Qué ocurriría si lo elimináramos?

Solo después de esto examinaremos los detalles de su implementación.

## FASE 5 — COMPRENDER LAS BIBLIOTECAS

Siempre que el proyecto utilice una biblioteca o un framework que posiblemente desconozca, explícame:

1. ¿Qué problema resuelve esta biblioteca?
2. ¿Por qué la utiliza este proyecto?
3. ¿Qué parte de la biblioteca es relevante en este caso?
4. ¿Qué tendríamos que hacer nosotros mismos si no la utilizáramos?
5. ¿Qué nos proporciona la biblioteca?
6. ¿Qué ventajas y desventajas tiene utilizarla?

No me expliques toda la biblioteca.

Explícame únicamente lo necesario para comprender este proyecto.

## FASE 6 — COMPRENDER EL CÓDIGO

Solo después de comprender la arquitectura profundizaremos en fragmentos de código individuales.

Para cada función o clase importante, explícame primero:

* Su función dentro del sistema.
* Quién la llama.
* Qué recibe.
* Qué devuelve.
* Qué efectos secundarios tiene.
* De qué depende.

Después, explícame su implementación.

NO empieces con explicaciones línea por línea, a menos que te lo pida específicamente.

## FASE 7 — COMPROBAR MI COMPRENSIÓN

Después de explicar un concepto importante, hazme entre 2 y 4 preguntas para comprobar si realmente lo he comprendido.

NO me des las respuestas inmediatamente.

Deja que responda primero.

Si mi respuesta es incorrecta, explícame en qué consiste mi error y corrige mi modelo mental.

## FASE 8 — CONSTRUIR EL MAPA MENTAL DEFINITIVO

Al final, ayúdame a crear un mapa mental conciso que contenga:

```text
PROYECTO
├── API / PUNTO DE ENTRADA
├── LÓGICA DE NEGOCIO
├── BASE DE DATOS
├── SERVICIOS EXTERNOS
├── INFRAESTRUCTURA
└── PRUEBAS
```

Para cada sección, dame una breve explicación de su responsabilidad y de cómo se conecta con las demás.

## REGLA FUNDAMENTAL

Si me falta algún conocimiento previo necesario, DETENTE.

Dime:

> «Antes de comprender X, necesitamos comprender Y».

Después, enséñame primero Y.

No sigas construyendo explicaciones sobre conceptos que todavía no comprendo.

## IMPORTANTE

No intentes que memorice el proyecto.

El objetivo es enseñarme a **leer y comprender software real**.

Poco a poco, debería ser capaz de orientarme en bases de código desconocidas sin necesitar que alguien me explique cada archivo.
