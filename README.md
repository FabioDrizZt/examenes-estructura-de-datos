# Suite de Exámenes Interactivos — Algoritmos y Estructuras de Datos

Plataforma interactiva de evaluaciones académicas desarrollada en **HTML5, Tailwind CSS y JavaScript Vanilla**. Incluye 4 variantes de exámenes parciales temáticos con simuladores de ejecución en tiempo real, trazadores algorítmicos, calculadora de rúbrica dinámica y soporte de impresión directa en formato A4 para toma presencial (`@media print`).

Desarrollado bajo la metodología **Spec-Driven Development (SDD)**.

---

## 🚀 Acceso a las Variantes y Portal

| Archivo | Variante | Dominio Narrativo | Color / Estilo | Acceso |
| :--- | :--- | :--- | :--- | :--- |
| **[`index.html`](index.html)** | **Portal Hub** | Dashboard Central & Selector | Indigo / Slate | [Abrir Portal](index.html) |
| **[`tema1.html`](tema1.html)** | **Tema 1 (Variante A)** | Criptoactivos & Finanzas Digitales | Cyan Eléctrico | [Abrir Tema 1](tema1.html) |
| **[`tema2.html`](tema2.html)** | **Tema 2 (Variante B)** | Smart Grid & Telemetría Energética | Esmeralda | [Abrir Tema 2](tema2.html) |
| **[`tema3.html`](tema3.html)** | **Tema 3 (Variante C)** | Telemetría Satelital & Órbitas GPS | Violeta / Púrpura | [Abrir Tema 3](tema3.html) |
| **[`tema4.html`](tema4.html)** | **Tema 4 (Variante D)** | Robótica Industrial & Brazos Ensambladores | Ámbar / Fuego | [Abrir Tema 4](tema4.html) |

---

## 📊 Matriz Comparativa Pedagógica

| Bloque Evaluado | Tema 1 (Variante A) | Tema 2 (Variante B) | Tema 3 (Variante C) | Tema 4 (Variante D) |
| :--- | :--- | :--- | :--- | :--- |
| **1. Structs y Memoria (15%)** | `stCotizacion` (18 B) &rarr; `stOperacionCripto` (112 B). Arreglo de 40. | `stFaseElectrica` (22 B) &rarr; `stTransformador` (118 B). Arreglo de 30. | `stCoordenadaOrbital` (26 B) &rarr; `stModuloSatelite` (130 B). Arreglo de 25. | `stArticulacionRobot` (18 B) &rarr; `stBrazoIndustrial` (104 B). Arreglo de 35. |
| **2. Ordenamiento y Búsqueda (20%)** | **Quicksort (Pivote inicial):** Particiones recursivas. Búsqueda de **62** (éxito) y **30** (fracaso). | **Inserción Directa:** Pasadas e inserciones. Búsqueda de **43** (éxito) y **60** (fracaso). | **Burbujeo con Centinela:** Comparaciones y bandera. Búsqueda de **50** (éxito) y **35** (fracaso). | **Método Shell:** Saltos $k=4, 2, 1$. Búsqueda de **59** (éxito) y **40** (fracaso). |
| **3. Notaciones y Expresiones (15%)** | **Infija &rarr; Prefija:** `((m + n) * p^2) / (r - s * 4)` con resolución analítica. | **Evaluación Postfija con Pila:** `36 4 / 2 3 ^ * 14 + 8 -`. Rdo final: **78**. | **Árbol Sintáctico Binario:** `((a*b) - (c/3)^2) + (d+8)*h` con 3 recorridos. | **Postfija &rarr; Infija:** `x y + w z - * k 3 ^ / m n * +` con paréntesis mínimos. |
| **4. Función Misterio Recursiva (5%)** | **Conteo Condicional:** Cuenta impares estrictamente mayores a $k$. Traza con $V=[7,12,15,4,21], k=9$. | **Predicado Booleano:** Valida si el vector es estrictamente creciente. Traza con $V=[5,11,18,14,27]$. | **Búsqueda de Mínimo Par:** Halla el menor número par con centinela. Traza con $V=[33,14,28,9,6]$. | **Productorio de Positivos:** Multiplica elementos $>0$ con base neutra 1. Traza con $V=[4,-2,3,5,-1]$. |
| **5. Problema Integrador TDAs (45%)** | **Pila (Vocales) + Cola (Consonantes):** Inicia por Pila. Ejemplo: `criptografia` &rarr; `aiacrptoigrf`. | **Lista (['a'..'m']) + Pila (['n'..'z']):** Inicia por Lista. Ejemplo: `redesenergeticas` &rarr; `edeegstrneicasrr`. | **Cola (Pares) + Lista (Impares):** Inicia por Cola. Ejemplo: `satelital` &rarr; `stlaetlia`. | **Lista (Vocales) + Pila (Consonantes):** Inicia por Lista. Ejemplo: `automatizacion` &rarr; `auoancziaiotmt`. |

---

## 🛠️ Características Principales

1. **Navegación por Pestañas:** Consignas oficiales, simuladores en vivo, calculadora de rúbrica y código base C++ con opción de copiado directo.
2. **Simuladores Interactivos en JavaScript:** Permiten a estudiantes y docentes ensayar cadenas y observar el procesamiento en las estructuras de datos (Pilas, Colas, Listas) y seguir la traza recursiva.
3. **Modo Impresión Presencial (`Ctrl + P`):** Reglas `@media print` automáticas que transforman cada variante en un examen A4 blanco y negro con campos para datos del alumno.
4. **Cero Dependencias de Servidor:** Funciona 100% offline y en cualquier navegador moderno abriendo los archivos HTML directamente o a través de GitHub Pages.

---

## 📑 Documentación Adicional

- [Especificación Técnica y Pedagógica Completa (SDD.md)](SDD.md)
- [Resumen Detallado de Variantes (README_VARIANTES.md)](README_VARIANTES.md)
