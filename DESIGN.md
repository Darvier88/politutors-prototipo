# PoliTutors · Sistema de diseño

Guía de identidad visual del prototipo. Cualquier pantalla nueva, la haga una persona o una IA, debe seguir estas reglas. El objetivo es que PoliTutors se vea **hecho a propósito**, no como una plantilla genérica.

---

## 1. Concepto: «Cuaderno politécnico»

El cuaderno cuadriculado de un buen compañero de la ESPOL: ordenado, con la cuadrícula celeste de siempre, fórmulas reales y anotaciones en rojo que te salvan el examen.

- **Para los padres** se lee como un **boletín**: sobrio, con tablas, cifras y garantías claras.
- **Para los estudiantes** se siente como el **cuaderno de un pana**: notas a mano, sellos y lenguaje cercano.
- **La sesión en vivo** cambia a **modo pizarra**: fondo azul noche y trazos de tiza.

Se divide el *registro* (boletín, cuaderno o pizarra), no la marca: la tipografía y la paleta son las mismas en todo el producto.

---

## 2. Relación con la identidad de la ESPOL

PoliTutors es un emprendimiento de estudiantes de la ESPOL y sus tutores son estudiantes de la ESPOL. Por eso su colorimetría **parte de la de la institución** y evita parecer un sitio oficial.

Tomado del *Manual de Identidad Corporativa ESPOL (2019)* y del logotipo institucional:

| Elemento ESPOL | Cómo lo usa PoliTutors |
|---|---|
| Azul institucional del logotipo | Color primario de acción (`--azul`) |
| Celeste de la textura de curvas y del logo | Cuadrícula del cuaderno y gráficos (`--celeste`), nunca como texto |
| Celeste pálido | Fondos de apoyo (`--celeste-p`) |
| Pantone plata y tramas de negro al 80 % y 50 % | Grises de texto secundario y filetes |
| Textura corporativa: cruce diagonal de la «e» y la «s» a **133°** | Tramado diagonal sutil a 133° en el hero, el pie y las zonas destacadas |
| Tipografía sans (Neue Hans Kendrick; Roboto como alternativa) | PoliTutors también es *sans-first*, con **Archivo** (libre, de Omnibus-Type, Argentina) |
| Logotipo en minúsculas | Wordmark `politutors` en minúsculas |

**Uso de la marca ESPOL.** El prototipo **no usa el logotipo, el sello ni la tortuga de la ESPOL**. Solo menciona “ESPOL” como dato descriptivo (por ejemplo, “Tutor verificado · matrícula ESPOL”). Para usar cualquier elemento gráfico oficial hay que solicitarlo a la Gerencia de Comunicación y Asuntos Públicos (comunicacion@espol.edu.ec), como indica la página de recursos de marca de la ESPOL.

> **Pendiente de validar:** los códigos exactos del manual (Pantone, CMYK, HEX) están en imágenes que no se pudieron extraer. Los valores de abajo se tomaron del logotipo y de la textura institucional. Si el equipo tiene el manual, reemplazar `--azul`, `--celeste` y `--celeste-p` por los oficiales. Todo lo demás se ajusta solo, porque el CSS usa variables.

---

## 3. Color

| Token | HEX | Uso | Contraste |
|---|---|---|---|
| `--paper` | `#F7F5F0` | Fondo general (papel cálido) | — |
| `--sheet` | `#FFFFFF` | Hojas (contenedores) | — |
| `--ink` | `#0E1F3D` | Texto y titulares (azul tinta, nunca negro puro) | 15,0:1 sobre papel |
| `--muted` | `#56627A` | Texto secundario (gris plata) | 5,6:1 sobre papel |
| `--azul` | `#1D4EA2` | **Único color de acción**: botones primarios, enlaces y progreso | 7,2:1 sobre papel; texto blanco encima 7,9:1 |
| `--azul-d` | `#163C7E` | Hover y estado presionado | Blanco encima 10,6:1 |
| `--celeste` | `#00B2E9` | Cuadrícula, gráficos y detalles. **Nunca texto** | 2,3:1 (no apto para texto) |
| `--celeste-d` | `#0077A8` | Celeste legible para etiquetas y cifras | 4,6:1 sobre papel |
| `--celeste-p` | `#DDF1FB` | Fondos informativos | Tinta encima 14,1:1 |
| `--amber` | `#F2C14E` | Resaltador, **solo como fondo** bajo texto tinta. Guiño al amarillo histórico de la ESPOL | Tinta encima 9,8:1 |
| `--red` | `#B8360A` | Rojo corrector: anotaciones, vacíos del diagnóstico, errores (siempre con texto o icono, nunca solo color) | 5,4:1 sobre papel |
| `--ok` | `#1E6B47` | Estados correctos (verificado, liberado) | 6,5:1 sobre papel |

**Colores por materia** (solo como filete o gráfico): Matemáticas `#1D4EA2`, Física `#0077A8`, Química `#2E7D5B`.

**Modo pizarra (sesión en vivo):** fondo `#0F1E33`, tiza `#EAF2F8` (14,8:1), celeste tiza `#5CCDF0` (9,1:1), amarillo tiza `#F5D45C` (11,5:1), rojo tiza `#FF7A59` (6,5:1).

**Regla:** en cada pantalla hay **un solo** color de acción (azul). El rojo corrige y el ámbar resalta. No se agregan más colores.

---

## 4. Tipografía

Las tres fuentes son libres y están en Google Fonts.

| Rol | Fuente | Detalles |
|---|---|---|
| Titulares y UI | **Archivo** (Omnibus-Type) | Titulares en 800 con ancho expandido (`font-stretch: 112–118 %`) e interletra −0,02 em. UI en 400/500/600 |
| Cifras, tiempos, precios, fórmulas y etiquetas | **Chivo Mono** (Omnibus-Type) | Etiquetas en mayúsculas de 11–12 px con interletra +0,06 em |
| Notas del tutor y citas | **Alegreya** itálica (Huerta Tipográfica) | Solo frases cortas: la nota del tutor en el reporte y los testimonios |

**Escala (px):** 12 · 14 · 16 · 18 · 22 · 28 · 38 · 52. El hero va en 52 px en escritorio y 34 px en celular, con interlineado 1,02.

**Nunca:** Inter, Plus Jakarta Sans, Poppins ni Space Grotesk.

---

## 5. Retícula y espacio

- Ancho máximo de 1180 px, márgenes de 20 px y retícula de 12 columnas en escritorio y 4 en celular.
- Espaciado en escala de 4: **4 · 8 · 12 · 16 · 24 · 32 · 48 · 72**.
- Alineación a la izquierda por defecto. Solo se centran números grandes y estados vacíos.
- **Cuadrícula de cuaderno:** líneas celestes cada 24 px (`--celeste` al 16 %). Solo en el hero, el diagnóstico, la búsqueda de tutor y la pizarra.
- **Tramado 133°:** líneas diagonales azules al 6 % cada 9 px. Solo como fondo de bandas destacadas (pie, llamado final).

---

## 6. Componentes

| Componente | Especificación |
|---|---|
| **Botón primario** | Fondo `--azul`, texto blanco Archivo 600 de 15 px, alto 46 px, radio 4 px. Sin sombra ni degradado. Hover `--azul-d`; al presionar baja 1 px. Foco: contorno de 2 px en `--celeste-d` con 2 px de separación |
| **Botón secundario** | Borde de 1,5 px en tinta, fondo transparente |
| **Hoja** (en lugar de tarjeta) | Fondo blanco, borde de 1 px en tinta al 14 %, radio 4 px y **sin sombra** |
| **Etiqueta** (en lugar de píldora) | Chivo Mono en mayúsculas de 11,5 px, color `--celeste-d`, precedida por un cuadrito de 6 px. Sin fondo |
| **Estado** | Punto de 7 px + texto. Sin píldora de color |
| **Sello** (insignias, verificado) | Contorno de 1,5 px, Chivo Mono en mayúsculas y rotación de −3°. Máximo uno destacado por bloque |
| **Vacío del diagnóstico** | Texto rodeado “a mano” con un óvalo rojo corrector |
| **Campo de texto** | Solo una línea inferior de 1,5 px, como renglón de cuaderno. Al enfocar se vuelve azul de 2 px. Los errores van con texto, no solo con color |
| **Área de texto** | Hoja con renglones celestes cada 28 px |
| **Selección** (chips) | Rectángulo de radio 4 px con borde de 1 px. Seleccionado: fondo azul |
| **Tabla** | Filetes de 1 px, cifras en Chivo Mono alineadas a la derecha |

---

## 7. Iconos y motivos

- **Iconos propios en SVG:** trazo de 1,6 px sobre retícula de 24 px, extremos redondeados y sin relleno. Se definen una sola vez en la función `ic()`.
- **Cero emojis en la interfaz.** Solo se permiten dentro de mensajes escritos por usuarios.
- **Materias con notación real** en lugar de iconos de matraz o átomo: `∑` Matemáticas, `Δv` Física, `H₂O` Química.
- **Anotaciones a mano:** óvalos, subrayados y flechas en rojo corrector, hechos en SVG.
- **Resaltador ámbar** bajo una o dos palabras clave por pantalla, nunca más.
- **Fotografía** (versión final): tutores reales en el campus Gustavo Galindo, con luz natural y sin fotos de banco.

---

## 8. Movimiento

- 150–250 ms con `ease-out`, todo en CSS y sin librerías.
- Solo tres usos: (1) feedback de botones, (2) la búsqueda de tutor (pulso sobre la cuadrícula), (3) las anotaciones que se dibujan al aparecer.
- Respeta `prefers-reduced-motion`: sin animaciones.

---

## 9. Tono de los textos

- Español de Ecuador. Tuteo a estudiantes y a padres, con frases cortas y concretas.
- **Estudiante:** «¿Te trabaste con un ejercicio? Sube la foto y en menos de 3 minutos te ayuda alguien de la ESPOL.»
- **Padre:** «Ves cada sesión: tema, duración, avances y lo que falta reforzar.»
- Mostrar pruebas en lugar de adjetivos: cifras, garantías y procesos. Si todavía no hay cifras reales, no se inventan: se muestra el proceso.

---

## 10. Nunca

- Degradados (en especial azul→morado) y glassmorphism.
- Sombras difusas en tarjetas.
- Píldoras de colores para todo.
- Hero centrado con píldora arriba y dos botones.
- Tres tarjetas iguales en fila como única estructura.
- Emojis como iconos.
- Inter, Plus Jakarta Sans y Poppins.
- El celeste como color de texto.
- El logotipo, el sello o la tortuga de la ESPOL sin autorización.

---

## 11. Accesibilidad y rendimiento

- Contraste mínimo de 4,5:1 en texto normal (ver la tabla de color).
- Áreas táctiles de 44 px o más y foco siempre visible.
- Ningún estado depende solo del color.
- Solo 3 familias tipográficas con `display=swap`.
- La identidad vive en CSS y SVG, sin imágenes pesadas, porque buena parte del público usa Android de gama baja.
