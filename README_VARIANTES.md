# Suite de Exámenes Interactivos (Iteración 5) — Algoritmos y Estructuras de Datos
## Modalidad Web: HTML5 + Tailwind CSS + JavaScript Vanilla

Este directorio contiene **4 variantes de examen completas e interactivas** desarrolladas conforme a la especificación [SDD.md](SDD.md).

Cada examen está encapsulado en una aplicación web interactiva local de una sola página (*SPA*), estilizada con **Tailwind CSS** y enriquecida con **simuladores dinámicos en JavaScript** para validar la lógica algorítmica en tiempo real y emitir hojas de examen impresas mediante `@media print`.

---

## 1. Acceso a los Exámenes

| Archivo | Variante | Dominio Narrativo | Color / Estilo | Acceso Directo |
| :--- | :--- | :--- | :--- | :--- |
| **`index.html`** | **Portal Hub** | Dashboard Central de la Suite | Indigo / Slate | [Abrir Portal](index.html) |
| **`tema1.html`** | **Tema 1 (Variante A)** | Criptoactivos & Finanzas Digitales | Cyan Eléctrico | [Abrir Tema 1](tema1.html) |
| **`tema2.html`** | **Tema 2 (Variante B)** | Smart Grid & Telemetría Energética | Esmeralda | [Abrir Tema 2](tema2.html) |
| **`tema3.html`** | **Tema 3 (Variante C)** | Telemetría Satelital & Órbitas GPS | Violeta / Púrpura | [Abrir Tema 3](tema3.html) |
| **`tema4.html`** | **Tema 4 (Variante D)** | Robótica Industrial & Brazos Ensambladores | Ámbar / Fuego | [Abrir Tema 4](tema4.html) |

---

## 2. Cuadro Comparativo Pedagógico de las 4 Variantes

| Bloque Evaluado | Tema 1 (Variante A) | Tema 2 (Variante B) | Tema 3 (Variante C) | Tema 4 (Variante D) |
| :--- | :--- | :--- | :--- | :--- |
| **1. Structs y Memoria (15%)** | `stCotizacion` (18 B) &rarr; `stOperacionCripto` (112 B). Arreglo de 40. | `stFaseElectrica` (22 B) &rarr; `stTransformador` (118 B). Arreglo de 30. | `stCoordenadaOrbital` (26 B) &rarr; `stModuloSatelite` (130 B). Arreglo de 25. | `stArticulacionRobot` (18 B) &rarr; `stBrazoIndustrial` (104 B). Arreglo de 35. |
| **2. Ordenamiento y Búsqueda (20%)** | **Quicksort (Pivote inicial):** Particiones recursivas. Búsqueda de **62** (éxito) y **30** (fracaso). | **Inserción Directa:** Pasadas e inserciones. Búsqueda de **43** (éxito) y **60** (fracaso). | **Burbujeo con Centinela:** Comparaciones y bandera. Búsqueda de **50** (éxito) y **35** (fracaso). | **Método Shell:** Saltos $k=4, 2, 1$. Búsqueda de **59** (éxito) y **40** (fracaso). |
| **3. Notaciones y Expresiones (15%)** | **Infija &rarr; Prefija:** `((m + n) * p^2) / (r - s * 4)` con resolución analítica. | **Evaluación Postfija con Pila:** `36 4 / 2 3 ^ * 14 + 8 -`. Rdo final: **78**. | **Árbol Sintáctico Binario:** `((a*b) - (c/3)^2) + (d+8)*h` con 3 recorridos. | **Postfija &rarr; Infija:** `x y + w z - * k 3 ^ / m n * +` con paréntesis mínimos. |
| **4. Función Misterio Recursiva (5%)** | **Conteo Condicional:** Cuenta impares estrictamente mayores a $k$. Traza con $V=[7,12,15,4,21], k=9$. | **Predicado Booleano:** Valida si el vector es estrictamente creciente. Traza con $V=[5,11,18,14,27]$. | **Búsqueda de Mínimo Par:** Halla el menor número par con centinela. Traza con $V=[33,14,28,9,6]$. | **Productorio de Positivos:** Multiplica elementos $>0$ con base neutra 1. Traza con $V=[4,-2,3,5,-1]$. |
| **5. Problema Integrador TDAs (45%)** | **Pila (Vocales) + Cola (Consonantes):** Inicia por Pila. Ejemplo: `criptografia` &rarr; `aiacrptoigrf`. | **Lista (['a'..'m']) + Pila (['n'..'z']):** Inicia por Lista. Ejemplo: `redesenergeticas` &rarr; `edeegstrneicasrr`. | **Cola (Pares) + Lista (Impares):** Inicia por Cola. Ejemplo: `satelital` &rarr; `stlaetlia`. | **Lista (Vocales) + Pila (Consonantes):** Inicia por Lista. Ejemplo: `automatizacion` &rarr; `auoancziaiotmt`. |

---

## 3. Características y Funcionalidades Web Implementadas

Cada variante interactiva (`temaN.html`) incorpora:
1. **Navegación por Pestañas:**
   - **📋 Consignas Oficiales:** Redacción completa con código C++ resaltado, tablas de memoria, fórmulas matemáticas y diagramas ASCII.
   - **🧪 Simulador en Vivo:** Herramientas interactivas programadas en JavaScript que permiten al docente o estudiante escribir cualquier palabra y presenciar la separación paso a paso en las estructuras dinámicas (Pila, Cola, Lista) con cálculo automático de mitades, o inspeccionar la traza recursiva en tiempo real.
   - **📊 Rúbrica y Calculadora Dinámica:** Controles deslizantes para calificar cada ítem (15%, 20%, 15%, 5%, 45%) con cálculo automático de puntaje acumulado y condición académica (*Insuficiente*, *Aprobado*, *Promocionado*).
   - **💻 Código Base / Starter C++:** Plantilla limpia con prototipos y `main()` modular con botón "Copiar al Portapapeles".
2. **Modo Impresión A4 Integrado:**
   - Al pulsar el botón **"Imprimir / Guardar PDF"** o presionar `Ctrl + P`, el motor de estilos activa las reglas `@media print`:
     - Oculta controles interactivos, tabs, simuladores y botones.
     - Adapta el fondo a blanco y tipografía a negro de alto contraste.
     - Formatea el examen en hojas A4 con espacio superior para Nombre, DNI y Calificación, listo para toma presencial en papel.

---

## 4. Control de Calidad y Validación

- [x] **Puntaje Global:** Cada tema totaliza exactamente **100%**.
- [x] **Diversificación Total:** No hay algoritmos de ordenamiento ni esquemas de notación repetidos entre variantes.
- [x] **Ejemplos Resueltos:** Cada Ejercicio 5 está demostrado paso a paso con diagramas y resultado validado en el código fuente.
- [x] **Compatibilidad Offline:** Cero dependencias de Node.js o servidores backend; ejecutable haciendo doble clic en el archivo HTML.
