# 🎨 Turbo Resumen de CSS Completo

## 📚 **1. SELECTORES BÁSICOS**
```css
/* 🔹 Selector de elemento */
p { color: blue; }

/* 🔹 Selector de clase */
.mi-clase { font-size: 16px; }

/* 🔹 Selector de ID */
#mi-id { background: yellow; }

/* 🔹 Selector universal */
* { margin: 0; padding: 0; }
```

## 🎯 **2. SELECTORES AVANZADOS**
```css
/* 🔹 Descendiente */
div p { color: red; }

/* 🔹 Hijo directo */
div > p { color: green; }

/* 🔹 Hermanos adyacentes */
h1 + p { margin-top: 0; }

/* 🔹 Atributo */
input[type="text"] { border: 1px solid #ccc; }

/* 🔹 Existencia de atributo */
p[class] { font-weight: bold; }

/* 🔹 Selector de clase aplicada a elemento */
p.mi-clase { color: blue }
```

## 🎨 **3. BOX MODEL**
```css
.caja {
    width: 200px;           /* 📏 Ancho */
    height: 100px;          /* 📐 Alto */
    padding: 20px;          /* 🛡️ Relleno interno */
    border: 2px solid black;/* 🖼️ Borde */
    margin: 10px;           /* 📦 Margen externo */
    box-sizing: border-box; /* 🎁 Incluye padding y border en el width */
}
```

## 🧩 **4. DISPLAY & POSITION**
```css
/* 🎭 Display */
.block { display: block; }      /* ⬇️ Ocupa toda la línea */
.inline { display: inline; }    /* ➡️ En línea */
.inline-block { display: inline-block; } /* 🎯 En línea pero con dimensiones */
.flex { display: flex; }        /* 📊 Contenedor flexible */
.grid { display: grid; }        /* 🏗️ Cuadrícula */

/* 📍 Position */
.static { position: static; }   /* 📄 Flujo normal */
.relative { position: relative; top: 10px; } /* 📍 Relativo a su posición */
.absolute { position: absolute; top: 0; left: 0; } /* 🎯 Relativo al contenedor */
.fixed { position: fixed; top: 0; } /* 📌 Fijo en viewport */
.sticky { position: sticky; top: 0; } /* 🧲 Se pega al scroll */
```

## 🎪 **5. FLEXBOX**
```css
.contenedor {
    display: flex;
    justify-content: center;    /* 🎯 Alineación horizontal */
    align-items: center;        /* 📏 Alineación vertical */
    flex-direction: row;        /* ➡️ Dirección (row/column) */
    flex-wrap: wrap;            /* 🔄 Salto de línea */
}

.item {
    flex: 1;                    /* 📊 Proporción del espacio */
    order: 2;                   /* 🔢 Orden visual */
}
```

## 🏗️ **6. CSS GRID**
```css
.contenedor {
    display: grid;
    grid-template-columns: 1fr 2fr 1fr; /* 🎯 3 columnas */
    grid-template-rows: 100px auto;     /* 📏 2 filas */
    gap: 10px;                          /* 📦 Espacio entre celdas */
}

.item {
    grid-column: 1 / 3;         /* 📍 Ocupa de col 1 a 3 */
    grid-row: 1;                /* 📍 Fila 1 */
}
```

## 🎨 **7. COLORES & FONDOS**
```css
.elemento {
    color: #ff0000;             /* 🔴 Color hexadecimal */
    color: rgb(255, 0, 0);      /* 🟥 RGB */
    color: rgba(255, 0, 0, 0.5);/* 🌈 RGB con transparencia */
    
    background-color: blue;      /* 🔵 Color de fondo */
    background-image: url('imagen.jpg'); /* 🖼️ Imagen de fondo */
    background-size: cover;      📏 Ajustar imagen */
    background-position: center; /* 🎯 Posición del fondo */
}
```

## ✨ **8. TIPOGRAFÍA**
```css
.texto {
    font-family: Arial, sans-serif; /* 🅰️ Familia tipográfica */
    font-size: 16px;                /* 📏 Tamaño */
    font-weight: bold;              /* 🏋️‍♂️ Grosor (normal, bold) */
    font-style: italic;             /* 🔤 Estilo (normal, italic) */
    text-align: center;             /* 🎯 Alineación */
    line-height: 1.5;               /* 📐 Altura de línea */
    text-decoration: underline;     /* ✏️ Decoración */
}
```

## 🎭 **9. TRANSICIONES & ANIMACIONES**
```css
/* 🔄 Transición suave */
.boton {
    transition: all 0.3s ease-in-out;
}
.boton:hover {
    transform: scale(1.1);      /* 🔍 Escalar al hover */
}

/* 🎬 Animación keyframes */
@keyframes mover {
    0% { transform: translateX(0); }
    100% { transform: translateX(100px); }
}

.animado {
    animation: mover 2s infinite alternate;
}
```

## 📱 **10. RESPONSIVE DESIGN**
```css
/* 📐 Media Queries */
@media (max-width: 768px) {
    .contenedor {
        flex-direction: column; /* 📱 Cambia a columna en móviles */
    }
}

/* 🖼️ Imágenes responsive */
img {
    max-width: 100%;           /* 📏 Nunca más ancha que su contenedor */
    height: auto;              /* 📐 Mantiene proporción */
}
```

## 🎯 **11. PSEUDOCLASES & PSEUDOELEMENTOS**
```css
/* 🎭 Pseudoclases */
a:hover { color: red; }        /* 🖱️ Al pasar mouse */
input:focus { border-color: blue; } /* ⌨️ Al enfocar */
li:nth-child(odd) { background: #f0f0f0; } /* 🔢 Elementos impares */

/* ✨ Pseudoelementos */
p::first-letter { font-size: 2em; } /* 🔠 Primera letra */
p::before { content: "👉 "; }       /* ➕ Contenido antes */
```

## 🎨 **12. TRANSFORMACIONES**
```css
.elemento {
    transform: rotate(45deg);       /* 🔄 Rotar */
    transform: scale(1.5);          /* 🔍 Escalar */
    transform: translate(50px, 20px); /* 🚀 Mover */
    transform: skew(10deg);         /* 📐 Inclinar */
}
```

## 🎪 **13. VARIABLES CSS**
```css
:root {
    --color-primario: #3498db;     /* 🎨 Definir variable */
    --espaciado: 20px;
}

.elemento {
    color: var(--color-primario);   /* 🎯 Usar variable */
    padding: var(--espaciado);
}
```

## 📦 **14. EJEMPLO PRÁCTICO COMPLETO**
```html
<!DOCTYPE html>
<html>
<head>
<style>
:root {
    --primary: #4CAF50;
    --secondary: #2196F3;
}

.card {
    width: 300px;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    background: white;
    transition: transform 0.3s ease;
}

.card:hover {
    transform: translateY(-5px);
}

.btn {
    background: var(--primary);
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background 0.3s;
}

.btn:hover {
    background: var(--secondary);
}

@media (max-width: 600px) {
    .card {
        width: 100%;
        margin: 10px 0;
    }
}
</style>
</head>
<body>
    <div class="card">
        <h2>🎨 Mi Tarjeta</h2>
        <p>¡CSS es increíble! ✨</p>
        <button class="btn">Haz clic 🚀</button>
    </div>
</body>
</html>
```

## 💡 **CONSEJOS RÁPIDOS**
- 🎯 **Especificidad**: `!important` > `inline` > `id` > `clase` > `elemento`
- 📱 **Mobile First**: Diseña primero para móviles
- 🎨 **Variables**: Usa CSS custom properties para mantener consistencia
- 🔍 **DevTools**: Aprende a usar las herramientas de desarrollador
- 📚 **BEM**: Considera metodologías como BEM para nombrar clases

¡Y eso es CSS en una cáscara de nuez! 🥜✨ ¿Necesitas profundizar en algún tema específico? 😊