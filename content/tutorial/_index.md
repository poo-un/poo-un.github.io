---
linkTitle: "Tutorial"
title: Tutorial edición página
cascade:
  type: default
---

{{< callout emoji="⛰️" >}}
  En esta página se encuentra el tutorial para construir el sitio web de la asignatura de POO con todo tipo de contenidos.
{{< /callout >}}

## Organización de archivos
Dentro de cada carpeta existe un número de archivos y carpetas que se describen a continuación:

{{< filetree/container >}}
  {{< filetree/folder name="content" >}}
    {{< filetree/file name="_index.md" >}}
    {{< filetree/folder name="docs" state="closed" >}}
      {{< filetree/file name="_index.md" >}}
      {{< filetree/file name="El resto de archivos" >}}
      {{< filetree/folder name="POO-concepts" state="closed" >}}
      {{< filetree/file name="_index.md" >}}
      {{< filetree/file name="El resto de archivos donde estarán los conceptos de POO" >}}
    {{< /filetree/folder >}}
    {{< filetree/folder name="languages" state="closed" >}}
      {{< filetree/file name="_index.md" >}}
      {{< filetree/file name="El resto de archivos donde estarán los conceptos de POO para cada lenguaje de programación" >}}
    {{< /filetree/folder >}}
    {{< /filetree/folder >}}
    {{< filetree/folder name="about" state="closed" >}}
      {{< filetree/file name="_index.md" >}}
      {{< filetree/file name="El resto de archivos con información del curso" >}}
    {{< /filetree/folder >}}
    {{< filetree/folder name="practice" state="closed" >}}
      {{< filetree/file name="_index.md" >}}
      {{< filetree/file name="El resto de archivos donde estarán los ejercicios" >}}
      {{< filetree/folder name="Javascript-practice" state="closed" >}}
      {{< filetree/file name="_index.md" >}}
      {{< filetree/file name="El resto de archivos donde estarán los ejercicios de Javascript" >}}
    {{< /filetree/folder >}}
    {{< filetree/folder name="Python-practice" state="closed" >}}
      {{< filetree/file name="_index.md" >}}
      {{< filetree/file name="El resto de archivos donde estarán los ejercicios de Python" >}}
    {{< /filetree/folder >}}
    {{< /filetree/folder >}}
  {{< /filetree/folder >}}
  {{< filetree/file name="hugo.yaml → Donde está la configuración de la página" >}}
{{< /filetree/container >}}

## Títulos y textos
Para generar un título se utiliza el símbolo `#` seguido del título. El número de `#` indica el nivel de título. Por ejemplo, para generar un título de primer nivel se utiliza `# Título de primer nivel`. Para generar un título de segundo nivel se utiliza `## Título de segundo nivel`. Y así sucesivamente.

El texto se puede resaltar utilizando el símbolo `*`. Por ejemplo, para generar un texto en negrita se utiliza `**Texto en negrita**`. Para generar un texto en cursiva se utiliza `*Texto en cursiva*`. Y así sucesivamente.

## Listas
Para generar una lista se utiliza el símbolo `-` seguido del elemento de la lista. Por ejemplo, para generar una lista con los elementos `elemento1`, `elemento2` y `elemento3` se utiliza:

```markdown
- elemento1
- elemento2
- elemento3
```
Si se quiere hacer una lista ordenada secuencialmente, se utiliza el símbolo `1.` seguido del elemento de la lista. Por ejemplo, para generar una lista con los elementos `elemento1`, `elemento2` y `elemento3` se utiliza:

```markdown 
1. elemento1
2. elemento2
3. elemento3
```

Si se quiere hacer una lista anidada, se utiliza el símbolo `-` seguido del elemento de la lista. Por ejemplo, para generar una lista con los elementos `elemento1`, `elemento2` y `elemento3` se utiliza:

```markdown
- elemento1
  - elemento2
    - elemento3
```

## Imagenes
Para insertar una imagen se utiliza el siguiente código:

```markdown
![Texto alternativo](/ruta/a/la/imagen)
```
por ejemplo, si queremos poner la imagen de este link `https://source.unsplash.com/featured/800x600?landscape`, se utiliza:

```markdown 
![Texto alternativo](https://source.unsplash.com/featured/800x600?landscape)
```
y el resultado será así
![](https://source.unsplash.com/featured/800x600?landscape)

## Videos 
Para insertar un video se utiliza el siguiente código:

```markdown
{{</* youtube id_del_video */>}}
```
por ejemplo, si queremos poner el video de este link `https://www.youtube.com/watch?v=Da-2h2B4faU`, se utiliza:

```markdown 
{{</* youtube Da-2h2B4faU */>}}
```
y el resultado será así
{{< youtube Da-2h2B4faU >}}

## Bloques de código
Para insertar un bloque de código se utiliza la siguiente sintaxis usando backticks (`` ` ``):

````markdown
```el lenguaje en el que queremos poner el código
el código que queremos poner
```
````


por ejemplo, si queremos poner un bloque de código en Python, se utiliza:

````markdown
```python
def say_hello():
    print("Hello!")
```
````

y el resultado será así
```python
def say_hello():
    print("Hello!")
```

### Bloques de código con números de linea
Para insertar un bloque de código con números de linea se utiliza `linenos=table` y opcionalmente se pone `linenostart=(número de línea)` para definir en qué número de línea empieza el código. Todo esto usando la siguiente sintaxis y usando backticks (`` ` ``):

````markdown
```el lenguaje que queremos poner{linenos=table, linenostart=(número de línea)}
el código que queremos poner
```
````
por ejemplo, si queremos poner un bloque de código en Python, se utiliza:

````markdown
```python{linenos=table, linenostart=18}
def say_hello():
    print("Hello!")
```
````
y el resultado será así
```python{linenos=table, linenostart=18}
def say_hello():
    print("Hello!")
```

### Copiar código
El botón de copiado está activado por default para cada bloque de código.


## Enlaces
Para insertar un enlace se utiliza la siguiente sintaxis:

```markdown
[Texto del enlace](/ruta/al/enlace)
```

por ejemplo, si queremos poner un enlace a la página principal de la asignatura, se utiliza:

```markdown
[Enlace a la página principal](https://arojaspe.github.io/Hugo-POO-UN/)
```

y el resultado será así

[Enlace a la página principal](https://arojaspe.github.io/Hugo-POO-UN/) 



## Tablas
Para insertar una tabla se utiliza la siguiente sintaxis:

```markdown
| Columna 1 | Columna 2 | Columna 3 |
|-----------|-----------|-----------|
| Elemento 1 | Elemento 2 | Elemento 3 |
|------------|------------|------------|
| Elemento 4 | Elemento 5 | Elemento 6 |
```

y el resultado será así

| Columna 1 | Columna 2 | Columna 3 |
|-----------|-----------|-----------|
| Elemento 1 | Elemento 2 | Elemento 3 |


## Diagramas
Para insertar un diagrama se utiliza Mermaid.
Mermaid es una herramienta basada en Javascript que permite generar diagramas y diagramas de flujo a partir de texto. Para más información sobre Mermaid, se puede consultar la [documentación oficial](https://mermaid-js.github.io/mermaid/#/). Se pueden generar todo tipo de diagramas, como diagramas de flujo, diagramas de secuencia, diagramas de clases, diagramas de Gantt, etc. Para insertar un diagrama se utiliza la siguiente sintaxis:

````markdown
```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
````

y el resultado será así

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

Se recomienda el uso de un editor de Mermaid para facilitar la construcción del diagrama como [Mermaid.live](https://mermaid.live/edit/) 
## Elementos adicionales

### Callouts
Un callout es un elemento que permite resaltar un texto. Para insertar un callout se utiliza la siguiente sintaxis:

#### Callout default

```markdown
{{</* callout */>}}
  En esta página se encuentra el tutorial para construir el sitio web de la asignatura de POO.
{{</* /callout */>}}
```


y el resultado será así

{{< callout >}}
  En esta página se encuentra el tutorial para construir el sitio web de la asignatura de POO.
{{< /callout >}}


#### Callout de información

```markdown
{{</* callout type="info" */>}}
  En este callout se encuentra información importante.
{{</* /callout */>}}
```

y el resultado será así

{{< callout type="info" >}}
  En este callout se encuentra información importante.
{{< /callout >}}

#### Callout de advertencia

```markdown
{{</* callout type="warning" */>}}
  Este callout está pensado para atraer la atención de quien lo lee.
{{</* /callout */>}}
```

y el resultado será así

{{< callout type="warning" >}}
  Este callout está pensado para atraer la atención de quien lo lee.
{{< /callout >}}

#### Callout de error

```markdown
{{</* callout type="error" */>}}
  Este callout está pensado para indicar que algo ha salido mal.
{{</* /callout */>}}
```

y el resultado será así

{{< callout type="error" >}}
  Este callout está pensado para indicar que algo ha salido mal.
{{< /callout >}}

### Botones (cards)
Un botón es un elemento que permite resaltar un enlace. Para insertar un botón se utiliza la siguiente sintaxis:

```markdown
{{</* cards */>}}
  {{</* card link="la ruta del archivo al que se quiere dirigir" title="Nombre botón" icon="ícono" */>}}
  {{</* card link="/ruta" title="Siguiente botón" */>}}
{{</* /cards */>}}
```

{{< cards >}}
  {{< card link="./" title="Botón de ejemplo" icon="code" >}}
  {{< card link="./" title="Botón secundario" icon="document" >}}
{{< /cards >}}

Los nombres de los íconos pueden ser reemplazados por los disponibles en [Heroicons](https://v1.heroicons.com/) 


## Tutoriales adicionales
* [Markdown Guide](https://www.markdownguide.org/)
* [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* [Markdown Tutorial](https://www.markdowntutorial.com/)
* [Markdown Reference](https://commonmark.org/help/)
* [Hextra guide](https://imfing.github.io/hextra/docs/getting-started/)