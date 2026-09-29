# Tarea\_markdown Riccardo

## Markdown

#### ¿Qué es?

Markdown es un lenguaje de marcado ligero creado en 2004 por John Gruber y Aaron Swartz, diseñado para convertir texto plano formateado fácilmente en HTML u otros formatos. En programación, su principal función es permitir a los desarrolladores escribir documentación, descripciones de proyectos y contenido técnico con una sintaxis intuitiva, sin necesidad de lidiar con la complejidad de las etiquetas HTML.

#### ¿Para que sirve?

Su principal utilidad es simplificar la escritura estructurada, ya que el texto marcado se convierte automáticamente en HTML, PDF, Word u otros formatos, facilitando la publicación web y la documentación técnica sin necesidad de conocimientos complejos de programación.

### Etiquetas en Markdown 1

#### Elementos de bloque

**Encabezados:** Se usan símbolos de almohadilla (#) para definir niveles jerárquicos, desde # (H1) hasta ###### (H6).

## Encabezado 1 (#)

### Encabezado 2 (##)

#### Encabezado 3 (###)

**Encabezado 4 (####)**

**Encabezado 5 (#####)**

**Encabezado 6 (######)**

### Salto de línea

Primer párrafo.

Segundo párrafo.

#### Barra invertida al final

Andando con sus patitas mojadas,\
el gorrión\
por la terraza de madera

#### La etiqueta (br)

Andando con sus patitas mojadas,\
el gorrión\
por la terraza de madera

### Listas

#### Listas desordenadas

* Primer elemento
* Segundo elemento
* Tercer elemento

#### Listas ordenadas

1. Primer paso
2. Segundo paso
3. Tercer paso

#### Listas anidadas

1. Preparación
   * Reunir ingredientes
   * Precalentar el horno
2. Cocinado
   1. Mezclar
   2. Hornear 40 minutos

#### Listas de tareas

* [x] Escribir el borrador
* [ ] Revisar

### Citas

#### Sintaxis básica

> Un país, una civilización se puede juzgar por la forma en que trata a sus animales. — Mahatma Gandhi

#### Citas de varios párrafos

> Creo que los animales ven en el hombre un ser igual a ellos que ha perdido de forma peligrosa el sano intelecto animal.
>
> Es decir, que ven en él al animal irracional, al animal que ríe, al animal que llora. — Friedrich Nietzsche

#### Forma sencilla para un solo parrafo

> Es decir, que ven en él al animal irracional, al animal que ríe, al animal que llora. Friedrich Nietzsche

#### Citas anidadas

> Esto es una cita normal.
>
> > Y esto es una cita dentro de la cita.
>
> Volvemos al primer nivel.

### Bloques de código

#### Bloques con vallas (´´´)

```javascript
function saludar(nombre) {
  return `Hola, ${nombre}`;
}
```

#### También sirve la virgulilla (\~\~\~)

```
Esto también es un bloque de código
```

### Líneas horizontales

***

***

***

### Negrita y cursiva

_cursiva_ (`* cursiva *`)

_cursiva_ (`_ cursiva _`)

**negrita** (`** negrita **`)

**negrita** (`__ negrita __`)

_**ambas**_ (`*** ambas ***`)

_**ambas**_ (`___ ambas ___`)

Tachado ~~texto~~ (`~~tachado~~`)

### Subrayado

Esto va subrayado dentro del párrafo. `<u>subrayado</u>`

### Enlaces

#### Enlaces en línea

Aprende más en [Markdown.es](https://markdown.es/). `[Markdown.es](https://markdown.es).`

#### Con título emergente

[Markdown.es](https://markdown.es/)

```markdown
[Markdown.es](https://markdown.es "Guía de Markdown en español")
```

### Enlaces de referencia

Me llamo Javier y escribo sobre [viajes a Grecia](https://helenizarte.com/). `[viajes a Grecia][web].`

Ese [proyecto](https://helenizarte.com/) nació porque me encanta el país.

```markdown
[web]: https://helenizarte.com "Turismo en Grecia"
```

### Etiqueta implícita

Consulta la [documentación](https://markdown.es/sintaxis-markdown) para más detalles.

```markdown
[documentación]: https://markdown.es/sintaxis-markdown
```

### Imágenes

![Texto alternativo](../../.gitbook/assets/57fe3871c97dd888433799ebd60997c0.jpg)

! — indica que es una imagen y no un enlace.

\[Texto alternativo] — lo que se muestra si la imagen no carga, y lo que leen los lectores de pantalla.

(/ruta) — la ubicación del archivo, relativa o dirección de la imagen.

```markdown
![Texto alternativo](https://i.pinimg.com/736x/57/fe/38/57fe3871c97dd888433799ebd60997c0.jpg)
```

### Título emergente

![XD](../../.gitbook/assets/e9eb9ec1b0da71003807507b2368cd21.jpg)

### Rutas: relativas o absolutas

![Absoluta a otro dominio](https://ejemplo.com/imagen.jpg)

```markdown
![Absoluta a otro dominio](https://ejemplo.com/imagen.jpg)\
![Absoluta dentro del sitio](/imagenes/foto.jpg)\
![Relativa al documento](./foto.jpg)\
![Un nivel arriba](../assets/foto.jpg)
```

### Controlar el tamaño

Markdown no tiene sintaxis para el tamaño de una imagen. Es una de sus limitaciones más conocidas. Las opciones:

#### HTML en línea (universal)

```html
<img src="/foto.jpg" alt="Descripción" width="400">
```

### Código en línea

#### Sintaxis

Envuelve el texto entre acentos graves \`:

Ejecuta `npm install` antes de arrancar el proyecto.

#### Acentos graves dentro del código

¿Y si el propio código contiene un acento grave?\
Entonces usa dos acentos graves como delimitadores:

Usa `` la plantilla `${nombre}` `` para interpolar.

Usa \`\`la plantilla \`${nombre}\` \`\` para interpolar.

Además, si el contenido empieza o acaba con un acento grave, añade un espacio justo después de la apertura y antes del cierre. Markdown se lo come al procesar:

```markdown
`` `codigo` ``
```

\`\` \`codigo\` \`\`

### Escapar caracteres

#### Sintaxis

\*Esto no está en cursiva\*

2 \* 3 \* 4 = 24

Un guion bajo\_dentro\_de una palabra

#### La alternativa: código en línea

Escapando: \*\*negrita\*\*\
Con código: `**negrita**`

### Tablas

#### Sintaxis básica

Una tabla se construye con barras verticales | para separar columnas y una línea de guiones que separa la cabecera del cuerpo.

| Lenguaje | Año  | Creador         |
| -------- | ---- | --------------- |
| Markdown | 2004 | John Gruber     |
| HTML     | 1993 | Tim Berners-Lee |
| LaTeX    | 1984 | Leslie Lamport  |

#### Alineación de columnas

| Producto    | Cantidad |   Precio |
| ----------- | :------: | -------: |
| Teclado     |     2    |  89,00 € |
| Monitor     |     1    | 249,90 € |
| Cable USB-C |    12    |   7,50 € |

#### Formato dentro de las celdas

| Elemento | Ejemplo                             |
| -------- | ----------------------------------- |
| Negrita  | **importante**                      |
| Cursiva  | _matiz_                             |
| Código   | `npm install`                       |
| Enlace   | [Markdown.es](https://markdown.es/) |
| Tachado  | ~~obsoleto~~                        |

#### Saltos de línea dentro de una celda

| Campo     | Valor                                          |
| --------- | ---------------------------------------------- |
| Dirección | <p>Calle Mayor 1<br>28013 Madrid<br>España</p> |

### Casillas de verificación

#### Sintaxis

* [x] Escribir el borrador
* [x] Revisar la ortografía
* [ ] Publicar
* [ ] Compartir en redes

Tres detalles que hay que respetar:

El espacio dentro de los corchetes vacíos es obligatorio. \[ ] con espacio, no \[].

Hay un espacio entre el corchete de cierre y el texto. - \[ ] Tarea, no - \[ ]Tarea.

Solo funciona sobre listas desordenadas. Con 1. en lugar de -, la mayoría de procesadores no lo reconocen.

#### Anidar tareas

Se anidan igual que cualquier lista, con cuatro espacios por nivel:

* [ ] Preparar el lanzamiento
  * [x] Escribir la nota de prensa
  * [x] Preparar las capturas
  * [ ] Grabar el vídeo de demostración
* [ ] Publicar

#### Formato dentro de la tarea

Dentro del texto de cada tarea funciona el resto de sintaxis en línea:

* [ ] Revisar el archivo `config.yml`
* [ ] Leer la [documentación de la API](https://ejemplo.com/)
* [x] ~~Arreglar el error de login~~ resuelto en #142
* [ ] **Urgente:** desplegar antes del viernes
