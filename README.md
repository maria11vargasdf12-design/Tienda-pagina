# Velour — Tienda de Ropa 

Tienda de ropa y accesorios desarrollada con HTML, CSS y JavaScript vanilla. Incluye carrito de compras funcional, diseño responsive y validación W3C.

---

## Estructura del proyecto

```
pagina tienda/
├── index.html
├── style.css
├── script.js
└── images/
    ├── bolso1.png
    ├── bolso2.png
    ├── car.svg
    ├── menu.png
    ├── modelo.png
    ├── ii1.svg
    ├── ii2-.svg
    ├── ii3.svg
    ├── ofert1.png
    ├── ofert2.png
    ├── ofert3.png
    ├── producto1.png → producto8.png
    ├── 1.png
    ├── 2.png
    └── 3.png
```

---

## Cómo correr el proyecto

1. Instala la extensión **Live Server** en VS Code
2. Click derecho en `index.html` → **Open with Live Server**
3. Se abre en `http://127.0.0.1:5500`
4. Cuando se guarden los cambios se recarga la página y permite ver los cambios.

---

## Secciones de la página

|    Sección      |                     Descripción                  |
|-----------------|--------------------------------------------------|
| **Header**      | Hero con imagen, texto y botón de acción         |
| **Navbar**      | Menú de navegación con carrito desplegable       |
| **Information** | Envío gratis, pago con tarjeta, envío nacional   |
| **Ofertas**     | 3 productos en oferta destacados                 |
| **Productos**   | Grid de 8 productos con botón agregar al carrito |
| **Servicios**   | 3 imágenes de tienda en layout asimétrico        |
| **Contacto**    | Formulario de suscripción por email              |
| **Footer**      | Enlaces de navegación en 4 columnas              |

---
## Carrito de compras

- Al hacer clic en **Agregar** el producto se añade al carrito
- El carrito se despliega al pasar el mouse sobre el ícono 🛒
- Cada producto se puede eliminar con la **X**
- El botón **Vaciar Carrito** elimina todos los productos
- Muestra imagen, nombre y precio de cada producto agregado

---

## Colores

| Nombre         |   Hex     |
|----------------|-----------|
| Azul principal | `#869dbb` |
| Azul oscuro    | `#7190b8` |
| Azul hover     | `#5a7a9e` |
| Crema          | `#f7f5e4` |
| Texto oscuro   | `#1e1e1d` |
| Texto gris     | `#272725` |

---

## Fuentes (Google Fonts)

- **Inter** — fuente principal del cuerpo
- **Lexend** — títulos y headings
- **Dosis** — textos secundarios
- **Public Sans** — textos generales
- **Roboto Mono** — detalles
---

## Diseño Responsive

| Breakpoint|                    Comportamiento                    |
|-----------|------------------------------------------------------|
| `> 991px` | Layout completo escritorio                           |
| `≤ 991px` | Menú hamburguesa, columnas apiladas, grid 2 columnas |
---

## Logo

El logo **VELOUR** está en texto en el navbar para poder modificarlo en `index.html`:

```html
<a href="#" class="logo">VELOUR</a>
```

Estilos en `style.css`:

```css
.logo {
    font-size: 25px;
    font-weight: 800;
    color: #f7f5e4;
    text-transform: uppercase;
    letter-spacing: 6px;
}
```

---

##  JavaScript — script.js

|            Función            |               Descripción             |
|-------------------------------|---------------------------------------|
| `cargarEventListeners()`      | Inicializa todos los eventos          |
| `comprarElemento(e)`          | Detecta clic en botón Agregar         |
| `leerDatosElemento(elemento)` | Extrae imagen, título, precio e id    |
| `insertarCarrito(elemento)`   | Crea la fila en la tabla del carrito  |
| `eliminarElemento(e)`         | Elimina un producto del carrito       |
| `vaciarCarrito(e)`            | Vacía todos los productos del carrito |

---

## Validación

HTML validado con **W3C Markup Validation Service** — sin errores, solo 2 warnings menores en secciones sin heading.

---

## Tecnologías

- HTML5
- CSS3 (Flexbox + Grid + Media Queries)
- JavaScript vanilla
- Google Fonts
- Live Server (desarrollo local)
- Git + GitHub (control de versiones)

---

