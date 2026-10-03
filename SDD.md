# SDD — Spec-Driven Development: Exámenes Interactivos de Programación y Estructuras de Datos
## Iteración 5 — Generación de 4 Nuevas Variantes en Versión Web (HTML + Tailwind CSS + JavaScript)

**Cátedra:** Algoritmos y Estructuras de Datos / Programación Avanzada (C++)  
**Instancia:** Examen Parcial / Regularidad y Promoción (Ciclo Lectivo 2026)  
**Documento:** Especificación Formal de Diseño y Arquitectura de Software de Exámenes (SDD)  
**Ubicación:** Repositorio de Exámenes de Estructuras de Datos  
**Hereda de:** Especificación pedagógica de generación de variantes de examen  
**Estado:** **ESPECIFICACIÓN COMPLETA APROBADA PARA IMPLEMENTACIÓN**  

---

## 1. Visión General, Alcance y Objetivos de la Iteración 5

La **Iteración 5** representa la evolución digital de la batería de exámenes de la cátedra. Integra las directrices pedagógicas de evaluación con una **plataforma web interactiva local de vanguardia (HTML5 + Tailwind CSS + JavaScript Vanilla)**.

### 1.1 Metas Clave
1. **Paridad y Rigor Pedagógico:** Formular cuatro (4) variantes de examen (Tema 1, Tema 2, Tema 3 y Tema 4) con idéntica distribución porcentual (totalizando exactamente **100%**) y niveles de exigencia cognitiva equivalentes.
2. **Diversificación Radical (Anti-Repetición):** Cada variante implementa dominios de estructuras disímiles, algoritmos de ordenamiento distintos, modalidades de notaciones aritméticas variadas, funciones recursivas incógnitas exclusivas y combinaciones singulares de Tipos de Datos Abstractos (TDAs) dinámicos en C++.
3. **Experiencia Web Interactiva (HTML + Tailwind + JS):** Proveer cada examen en un formato web auto-contenido (*Single-File Components* o bundles ligeros sin dependencias de Node.js) que los estudiantes y docentes puedan abrir directamente en cualquier navegador (Chrome, Edge, Firefox), con:
   - Navegación fluida por pestañas (*Consignas*, *Simulador de Ejecución*, *Calculadora de Rúbrica*, *Código de Partida*).
   - Micro-simuladores interactivos en JavaScript que permiten visualizar el comportamiento de las estructuras del Ejercicio 5 y la traza del Ejercicio 2 y 4.
   - Modo de impresión optimizado para papel o PDF (`@media print`) que oculta los controles interactivos y formatea el examen listo para evaluación presencial tradicional.
   - Hub de acceso central (`index.html`) para alternar y comparar los 4 temas en un clic.

---

## 2. Pila Tecnológica, Estándares Web e Invariantes

### 2.1 Pila de Entrega Web (Frontend)
- **Estructura:** HTML5 semántico (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`).
- **Estilos:** Tailwind CSS CDN (v3.4+) con paletas oscuras (*Dark Mode* Slate/Zinc/Neutral), tipografías web de Google Fonts ([Inter](https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap) y [Fira Code / JetBrains Mono](https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;600&display=swap)) y efectos de *Glassmorphism* (`backdrop-blur-md`, bordes sutiles con opacidad `white/10`).
- **Comportamiento e Interactividad:** JavaScript Vanilla (ES6+) moderno y seguro, sin librerías externas pesadas ni compiladores (NPM/Vite innecesarios para portabilidad directa mediante doble clic).
- **Formatos Matemáticos y Diagramas:** Fórmulas matemáticas formateadas con entidades HTML/LaTeX nítidas y diagramas de memoria renderizados en bloques monospace con paleta de terminal ANSI accesible.
- **Portabilidad:** Cero dependencias de servidor. Ejecutable en protocolo local `file://` o mediante Live Server.

### 2.2 Invariantes de Evaluación y Rúbrica (100% Total)
Cada uno de los 4 exámenes respetará estrictamente la siguiente distribución fija:
- **Ejercicio 1: Memoria y Structs Anidados (15%)**
  - Sub-pregunta a: Tamaño de variable simple del struct base o compuesto (**7.5%**).
  - Sub-pregunta b: Tamaño en memoria de un arreglo de $N$ registros (**7.5%**).
- **Ejercicio 2: Ordenamiento y Búsqueda (20%)**
  - Algoritmo de ordenamiento paso a paso sobre vector de 8 elementos (**12%**).
  - Búsqueda binaria - Clave 1 [Éxito] con tabla de seguimiento (**4%**).
  - Búsqueda binaria - Clave 2 [Fracaso] con tabla de seguimiento (**4%**).
- **Ejercicio 3: Notaciones y Expresiones Aritméticas (15%)**
  - Transformación, evaluación con pila o árbol sintáctico (**15%**).
- **Ejercicio 4: Recursión con Código Incógnito / Función Misterio (5%)**
  - Sub-pregunta a: Deducción analítica de caso base, caso recursivo y propósito (**2.5%**).
  - Sub-pregunta b: Traza manual con árbol de llamadas para vector de prueba (**2.5%**).
- **Ejercicio 5: Problema Integrador en C++ con TDAs Dinámicos (45%)**
  - Carga y validación estricta de la palabra [5 a 25 caracteres] (**5%**).
  - Carga distribuida en Estructura 1 y Estructura 2 (**10%**).
  - Algoritmo de codificación con alternancia de mitades y vaciado completo (**10%**).
  - Muestra y visualización de estructuras intermedias (**5%**).
  - Menú interactivo modular y documentación interna (**5%**).
  - Implementación/modificación segura de TDAs con punteros (**10%**).

---

## 3. Matriz Comparativa Global de las 4 Variantes (Iteración 5)

A continuación se resume la matriz de diversificación asignada a cada variante para garantizar que no existan ejercicios repetidos o meros cambios numéricos:

```
+========================================================================================================================+
|                                    MATRIZ COMPARATIVA DE VARIANTES - ITERACIÓN 5                                       |
+================================+===========================+===========================+===============================+
| Dimensión Evaluada             | Variante 1 (Tema 1)       | Variante 2 (Tema 2)       | Variante 3 (Tema 3)           | Variante 4 (Tema 4)           |
+================================+===========================+===========================+===============================+
| Identidad / Eje Temático       | Criptoactivos & Finanzas  | Smart Grid & Energía      | Satélites & Exploración       | Robótica Industrial & IoT     |
| Color Primario Tailwind        | Cyan / Indigo (`cyan-500`)| Emerald / Lime (`emerald`)| Violet / Purple (`purple-500`)| Amber / Rose (`amber-500`)    |
+--------------------------------+---------------------------+---------------------------+-------------------------------+-------------------------------+
| 1. Dominio de Structs          | Transacciones & Ledger    | Medición en Subestaciones | Telemetría Satelital          | Cinemática y Actuadores       |
|    - Struct Base               | stCotizacion (18 B)       | stFaseElectrica (22 B)    | stCoordenadaOrbital (26 B)    | stArticulacionRobot (18 B)    |
|    - Struct Compuesto          | stOperacionCripto (112 B) | stTransformador (118 B)   | stModuloSatelite (130 B)      | stBrazoIndustrial (104 B)     |
|    - Arreglo a Calcular        | Arreglo de 40 elementos   | Arreglo de 30 elementos   | Arreglo de 25 elementos       | Arreglo de 35 elementos       |
+--------------------------------+---------------------------+---------------------------+-------------------------------+-------------------------------+
| 2. Ordenamiento y Búsqueda     | Quicksort (Pivote Primero)| Inserción Directa         | Burbuja con Centinela         | Método Shell                  |
|    - Vector Inicial            | [58, 24, 91, 33, 76, 15,  | [72, 38, 19, 85, 43, 26,  | [63, 17, 88, 42, 29, 95,      | [45, 82, 16, 67, 34, 90,      |
|                                |  62, 47]                  |  94, 51]                  |  50, 71]                      |  23, 59]                      |
|    - Claves Búsqueda Binaria   | 62 (éxito) y 30 (fracaso) | 43 (éxito) y 60 (fracaso) | 50 (éxito) y 35 (fracaso)     | 59 (éxito) y 40 (fracaso)     |
+--------------------------------+---------------------------+---------------------------+-------------------------------+-------------------------------+
| 3. Notaciones y Expresiones    | Infija a Prefija (Polaca) | Evaluación Postfija (Pila)| Árbol Sintáctico + 3 Recorrid.| Postfija a Infija (Paréntesis)|
|    - Expresión Evaluada        | ((m + n) * p^2) /         | 36 4 / 2 3 ^ * 14 + 8 -   | ((a * b) - (c / 3)^2) +       | x y + w z - * k 3 ^ /         |
|                                | (r - s * 4)               |                           | (d + 8) * h                   | m n * +                       |
|    - Técnica Exigida           | Reglas de prioridad/pila  | Tabla de estados de pila  | Grafo en árbol + pre/in/post  | Reconstrucción sin redundancia|
+--------------------------------+---------------------------+---------------------------+-------------------------------+-------------------------------+
| 4. Función Misterio Recursiva  | Filtro Condicional        | Predicado Booleano        | Búsqueda de Mínimo            | Productorio Acumulado         |
|    - Propósito del Código      | Contar impares mayores a K| Verificar orden ascendente| Encontrar menor par recursivo | Producto de elementos > 0     |
|    - Vector de Prueba (Traza)  | V = [7, 12, 15, 4, 21],K=9| V = [5, 11, 18, 14, 27]   | V = [33, 14, 28, 9, 6]        | V = [4, -2, 3, 5, -1]         |
+--------------------------------+---------------------------+---------------------------+-------------------------------+-------------------------------+
| 5. Problema Integrador C++     | Pila + Cola               | Lista Enlazada + Pila     | Cola + Lista Enlazada         | Pila + Lista Enlazada         |
|    - Estructuras Dinámicas     | Pila (LIFO) + Cola (FIFO) | Lista (Enlazada) + Pila   | Cola (FIFO) + Lista (Enlazada)| Pila (LIFO) + Lista (Enlazada)|
|    - Criterio de Distribución  | Vocales -> Pila           | Rango ['a'..'m'] -> Lista | Índices pares -> Cola         | Consonantes -> Pila           |
|                                | Consonantes -> Cola       | Rango ['n'..'z'] -> Pila  | Índices impares -> Lista      | Vocales -> Lista              |
|    - Orden de Alternancia      | 1ª Mit. Pila -> 1ª M.Cola | 1ª Mit. Lista -> 1ª M.Pila| 1ª Mit. Cola -> 1ª M.Lista    | 1ª Mit. Lista -> 1ª M.Pila    |
|                                | 2ª Mit. Pila -> 2ª M.Cola | 2ª Mit. Lista -> 2ª M.Pila| 2ª Mit. Cola -> 2ª M.Lista    | 2ª Mit. Lista -> 2ª M.Pila    |
|    - Palabra de Prueba         | "criptografia" (13 car.)  | "redesenergeticas" (16 c.)| "satelital" (10 car.)         | "automatizacion" (14 car.)    |
+================================+===========================+===========================+===============================+
```

---

## 4. Especificación Detallada de Cada Variante

### 4.1 Variante 1 (Tema 1: Criptoactivos & Finanzas Digitales)
- **Identificador UI:** `tema1.html`
- **Acento cromático:** Cyan / Azul Eléctrico (`border-cyan-500/30`, `text-cyan-400`, `bg-cyan-500/10`).

#### Ejercicio 1: Memoria y Structs Anidados (15%)
```c
struct stCotizacion {
    float PrecioUSD;           // 4 bytes
    float Variacion24h;        // 4 bytes
    unsigned shortint Volumen; // 2 bytes
    char IndicadorTendencia;   // 1 byte ('S'=Suba, 'B'=Baja, 'L'=Lateral)
    char ParTrading[7];        // 7 bytes (ej: "BTCUSDT")
};                             // Subtotal = 4 + 4 + 2 + 1 + 7 = 18 bytes

struct stOperacionCripto {
    char HashTransaccion[36];      // 36 bytes
    char BilleteraDestino[42];     // 42 bytes
    stCotizacion DatosMercado;     // 18 bytes
    unsigned shortint Confirmaciones; // 2 bytes
    float ComisionFee;             // 4 bytes
    char TipoOrden;                // 1 byte ('C'=Compra, 'V'=Venta)
    char RedBlockchain[9];         // 9 bytes (ej: "ETHEREUM")
};                                 // Subtotal = 36 + 42 + 18 + 2 + 4 + 1 + 9 = 112 bytes
```
- **Consignas:**
  - **a.** Cantidad de bytes ocupados por `stCotizacion miTicker;` $\to$ **18 bytes**.
  - **b.** Cantidad de bytes ocupados por `stOperacionCripto Mempool[40];` $\to$ $112 \times 40 =$ **4480 bytes**.

#### Ejercicio 2: Ordenamiento y Búsqueda (20%)
- **Vector Base:** $V = [58, 24, 91, 33, 76, 15, 62, 47]$ ($N=8$).
- **Método de Ordenamiento:** **Quicksort (Pivote = Primer elemento)**.
  - Partición inicial con pivote $58$: reubicación de menores a la izquierda y mayores a la derecha.
  - Mostrar llamadas recursivas con sub-arreglos resultantes en cada etapa.
  - *Vector Ordenado Final:* $[15, 24, 33, 47, 58, 62, 76, 91]$.
- **Búsqueda Binaria:**
  - **Clave 1 (Éxito):** Buscar $62$. Mostrar tabla con columnas: `Paso`, `izq`, `der`, `medio`, `V[medio]`, `Acción`.
  - **Clave 2 (Fracaso):** Buscar $30$. Mostrar seguimiento hasta condición de corte `izq > der`.

#### Ejercicio 3: Notaciones y Expresiones (15%)
- **Técnica:** **Conversión de Infija a Prefija (Notación Polaca Directa)**.
- **Expresión Infija:**
  $$\frac{(m + n) \cdot p^2}{r - s \cdot 4}$$
  *(En formato de texto: `((m + n) * p^2) / (r - s * 4)`)*
- **Requerimiento:** Procedimiento analítico paso a paso respetando jerarquía de operadores (`^` > `*`, `/` > `+`, `-`) y paréntesis.
- **Resultado Prefijo Canónico:**
  `/ * + m n ^ p 2 - r * s 4`

#### Ejercicio 4: Recursión con Función Misterio (5%)
```cpp
int misterio1(const int arr[], int n, int k) {
    if (n == 0) {
        return 0; // Caso base: vector vacío o fin del recorrido
    }
    int acumulador = misterio1(arr, n - 1, k);
    if (arr[n - 1] % 2 != 0 && arr[n - 1] > k) {
        return 1 + acumulador;
    } else {
        return acumulador;
    }
}
```
- **Consignas:**
  - **a.** Deducir qué calcula la función e identificar caso base y paso inductivo. *(Respuesta: Cuenta la cantidad de números impares estrictamente mayores que $k$)*.
  - **b.** Traza manual completa con $V = [7, 12, 15, 4, 21]$, $n=5$ y $k=9$. Retorno esperado: **2** (los impares $>9$ son $15$ y $21$; $7$ no es $>9$, $12$ y $4$ son pares).

#### Ejercicio 5: Problema Integrador en C++ con TDAs (45%)
- **Estructuras:** Pila Dinámica (LIFO) + Cola Dinámica (FIFO).
- **Distribución de Caracteres:**
  - **Vocales** $\to$ Insertadas en la **Pila**.
  - **Consonantes** $\to$ Insertadas en la **Cola**.
- **Alternancia y Vaciado:**
  - Comienza la codificación con la **Pila**:
    1. Desapilar la primera mitad de la Pila ($M_{p1} = \lfloor N_p / 2 \rfloor + (N_p \% 2)$).
    2. Desencolar la primera mitad de la Cola ($M_{c1} = \lfloor N_c / 2 \rfloor + (N_c \% 2)$).
    3. Desapilar los elementos restantes de la Pila ($M_{p2}$).
    4. Desencolar los elementos restantes de la Cola ($M_{c2}$).
- **Ejemplo Resuelto en SDD:**
  - Palabra de prueba: `"criptografia"` (longitud: 12 letras sin espacios).
  - Letras:
    - Vocales: `'i'`, `'o'`, `'a'`, `'i'`, `'a'` (5 vocales en Pila).
      - Pila (tope al final): `fondo -> ['i', 'o', 'a', 'i', 'a'] <- tope`.
    - Consonantes: `'c'`, `'r'`, `'p'`, `'t'`, `'g'`, `'r'`, `'f'` (7 consonantes en Cola).
      - Cola: `frente -> ['c', 'r', 'p', 't', 'g', 'r', 'f'] <- fin`.
  - Mitades:
    - Pila: 5 elementos $\to M_{p1} = 3$, $M_{p2} = 2$.
    - Cola: 7 elementos $\to M_{c1} = 4$, $M_{c2} = 3$.
  - Extracción:
    - 1) 3 letras desapiladas de Pila: `'a'`, `'i'`, `'a'`.
    - 2) 4 letras desencoladas de Cola: `'c'`, `'r'`, `'p'`, `'t'`.
    - 3) 2 letras restantes de Pila: `'o'`, `'i'`.
    - 4) 3 letras restantes de Cola: `'g'`, `'r'`, `'f'`.
  - **Palabra Codificada Final:** `"aiacrpt oigrf"` $\to$ `"aiacrptoigrf"`.

---

### 4.2 Variante 2 (Tema 2: Smart Grid & Distribución de Energía)
- **Identificador UI:** `tema2.html`
- **Acento cromático:** Esmeralda / Lima (`border-emerald-500/30`, `text-emerald-400`, `bg-emerald-500/10`).

#### Ejercicio 1: Memoria y Structs Anidados (15%)
```c
struct stFaseElectrica {
    float TensionVoltios;      // 4 bytes
    float CorrienteAmperios;   // 4 bytes
    float PotenciaActivaKw;    // 4 bytes
    unsigned shortint FrecuenciaHz; // 2 bytes
    char EstadoFase;           // 1 byte ('N'=Normal, 'S'=Sobrecarga, 'C'=Corte)
    char CodigoSensor[7];      // 7 bytes
};                             // Subtotal = 4 + 4 + 4 + 2 + 1 + 7 = 22 bytes

struct stTransformador {
    char IdSubestacion[15];        // 15 bytes
    char UbicacionBarrio[35];      // 35 bytes
    stFaseElectrica FasePrimaria;  // 22 bytes
    unsigned shortint TemperaturaC;// 2 bytes
    float CapacidadMaximaKva;      // 4 bytes
    char TipoAislacion;            // 1 byte ('A'=Aceite, 'S'=Seco)
    char RedZonaDistribucion[39];  // 39 bytes
};                                 // Subtotal = 15 + 35 + 22 + 2 + 4 + 1 + 39 = 118 bytes
```
- **Consignas:**
  - **a.** Cantidad de bytes ocupados por `stFaseElectrica MonitoreoR;` $\to$ **22 bytes**.
  - **b.** Cantidad de bytes ocupados por `stTransformador ParqueTransformadores[30];` $\to$ $118 \times 30 =$ **3540 bytes**.

#### Ejercicio 2: Ordenamiento y Búsqueda (20%)
- **Vector Base:** $V = [72, 38, 19, 85, 43, 26, 94, 51]$ ($N=8$).
- **Método de Ordenamiento:** **Inserción Directa (Insertion Sort)**.
  - Mostrar el estado del vector en cada pasada de inserción ($i = 1$ hasta $7$), indicando elemento insertado y desplazamientos generados.
  - *Vector Ordenado Final:* $[19, 26, 38, 43, 51, 72, 85, 94]$.
- **Búsqueda Binaria:**
  - **Clave 1 (Éxito):** Buscar $43$.
  - **Clave 2 (Fracaso):** Buscar $60$.

#### Ejercicio 3: Notaciones y Expresiones (15%)
- **Técnica:** **Evaluación de Expresión Postfija con Pila de Operandos**.
- **Expresión Postfija:**
  `36 4 / 2 3 ^ * 14 + 8 -`
- **Requerimiento:** Tabla paso a paso de estados de la pila:
  1. `36` $\to$ push(36)
  2. `4` $\to$ push(4)
  3. `/` $\to 36 / 4 = 9 \to$ push(9)
  4. `2` $\to$ push(2)
  5. `3` $\to$ push(3)
  6. `^` $\to 2^3 = 8 \to$ push(8)
  7. `*` $\to 9 \times 8 = 72 \to$ push(72)
  8. `14` $\to$ push(14)
  9. `+` $\to 72 + 14 = 86 \to$ push(86)
  10. `8` $\to$ push(8)
  11. `-` $\to 86 - 8 = 78 \to$ push(78)
- **Resultado Final:** **78**.

#### Ejercicio 4: Recursión con Función Misterio (5%)
```cpp
bool misterio2(const int arr[], int n) {
    if (n <= 1) {
        return true; // Caso base: vector de 0 o 1 elemento siempre está ordenado
    }
    if (arr[n - 2] >= arr[n - 1]) {
        return false; // Violación del orden estrictamente creciente
    }
    return misterio2(arr, n - 1);
}
```
- **Consignas:**
  - **a.** Deducir qué propiedad matemática comprueba la función. *(Respuesta: Predicado booleano que retorna `true` si el arreglo está estrictamente ordenado en forma creciente de izquierda a derecha)*.
  - **b.** Traza manual completa con $V = [5, 11, 18, 14, 27]$, $n=5$. Explicar en qué llamada y con qué índices se detecta la condición de salida falsa (`arr[2] = 18 >= arr[3] = 14`).

#### Ejercicio 5: Problema Integrador en C++ con TDAs (45%)
- **Estructuras:** Lista Simplemente Enlazada + Pila Dinámica.
- **Distribución de Caracteres:**
  - Caracteres alfabéticos en rango `['a'..'m']` $\to$ Insertados en la **Lista Enlazada** (al final).
  - Caracteres alfabéticos en rango `['n'..'z']` $\to$ Insertados en la **Pila** (apilados).
- **Alternancia y Vaciado:**
  - Inicia con la **Lista Enlazada**:
    1. Extraer del frente la primera mitad de la Lista ($M_{l1}$).
    2. Desapilar la primera mitad de la Pila ($M_{p1}$).
    3. Extraer las letras restantes de la Lista ($M_{l2}$).
    4. Desapilar las letras restantes de la Pila ($M_{p2}$).
- **Ejemplo Resuelto en SDD:**
  - Palabra: `"redesenergeticas"` (longitud: 16).
  - Separación:
    - Rango `a..m`: `'e'`, `'d'`, `'e'`, `'e'`, `'g'`, `'e'`, `'i'`, `'c'`, `'a'` (9 letras en Lista).
      - Lista: `inicio -> ['e', 'd', 'e', 'e', 'g', 'e', 'i', 'c', 'a'] -> NULL`.
    - Rango `n..z`: `'r'`, `'s'`, `'n'`, `'r'`, `'t'`, `'s'` (6 letras en Pila).
      - Pila: `fondo -> ['r', 's', 'n', 'r', 't', 's'] <- tope`.
    - Mitades:
      - Lista (9): $M_{l1} = 5$, $M_{l2} = 4$.
      - Pila (6): $M_{p1} = 3$, $M_{p2} = 3$.
    - Extracción:
      - 1) 5 letras de Lista: `'e'`, `'d'`, `'e'`, `'e'`, `'g'`.
      - 2) 3 desapiladas de Pila: `'s'`, `'t'`, `'r'`.
      - 3) 4 letras de Lista: `'e'`, `'i'`, `'c'`, `'a'`.
      - 4) 3 desapiladas de Pila: `'n'`, `'s'`, `'r'`.
  - **Palabra Codificada Final:** `"edeegstreicansr"`.

---

### 4.3 Variante 3 (Tema 3: Telemetría Satelital & Exploración Espacial)
- **Identificador UI:** `tema3.html`
- **Acento cromático:** Violeta / Púrpura (`border-purple-500/30`, `text-purple-400`, `bg-purple-500/10`).

#### Ejercicio 1: Memoria y Structs Anidados (15%)
```c
struct stCoordenadaOrbital {
    float ApogeoKm;            // 4 bytes
    float PerigeoKm;           // 4 bytes
    float InclinacionGrados;   // 4 bytes
    float VelocidadOrbitalKms; // 4 bytes
    unsigned shortint OrbitaNro;// 2 bytes
    char EstadoPropulsion;     // 1 byte ('I'=Inercial, 'M'=Maniobra)
    char IdSatelite[7];        // 7 bytes
};                             // Subtotal = 4*4 + 2 + 1 + 7 = 26 bytes

struct stModuloSatelite {
    char CodigoMision[16];          // 16 bytes
    char AgenciaEspacial[30];       // 30 bytes
    stCoordenadaOrbital OrbitaGPS;  // 26 bytes
    float CargaBateriaWatts;        // 4 bytes
    unsigned int TiempoMisionDias;  // 4 bytes
    char NivelRadiacion;            // 1 byte ('B'=Baja, 'M'=Media, 'A'=Alta)
    char NombreModuloInstrumento[49];// 49 bytes
};                                  // Subtotal = 16 + 30 + 26 + 4 + 4 + 1 + 49 = 130 bytes
```
- **Consignas:**
  - **a.** Cantidad de bytes de `stCoordenadaOrbital PosicionSat;` $\to$ **26 bytes**.
  - **b.** Cantidad de bytes de `stModuloSatelite ConstelacionSat[25];` $\to$ $130 \times 25 =$ **3250 bytes**.

#### Ejercicio 2: Ordenamiento y Búsqueda (20%)
- **Vector Base:** $V = [63, 17, 88, 42, 29, 95, 50, 71]$ ($N=8$).
- **Método de Ordenamiento:** **Burbujeo con Bandera / Centinela (Optimizado)**.
  - Mostrar pasadas de comparaciones adyacentes, intercambios ocurridos y el estado del indicador `huboIntercambio` para justificar cuándo finaliza el ordenamiento.
  - *Vector Ordenado Final:* $[17, 29, 42, 50, 63, 71, 88, 95]$.
- **Búsqueda Binaria:**
  - **Clave 1 (Éxito):** Buscar $50$.
  - **Clave 2 (Fracaso):** Buscar $35$.

#### Ejercicio 3: Notaciones y Expresiones (15%)
- **Técnica:** **Construcción de Árbol Sintáctico de Expresión y Recorridos**.
- **Expresión Infija:**
  $$\left((a \cdot b) - \left(\frac{c}{3}\right)^2\right) + (d + 8) \cdot h$$
- **Requerimiento:**
  - Dibujar la estructura del árbol binario con operadores como nodos internos y operandos como hojas.
  - Obtener los tres recorridos canónicos:
    - **Preorden (Prefija):** `+ - * a b ^ / c 3 2 * + d 8 h`
    - **Inorden (Infija original):** `a * b - c / 3 ^ 2 + d + 8 * h`
    - **Postorden (Postfija):** `a b * c 3 / 2 ^ - d 8 + h * +`

#### Ejercicio 4: Recursión con Función Misterio (5%)
```cpp
int misterio3(const int arr[], int n) {
    if (n == 1) {
        return (arr[0] % 2 == 0) ? arr[0] : 999999; // Caso base
    }
    int minResto = misterio3(arr, n - 1);
    int candidato = (arr[n - 1] % 2 == 0) ? arr[n - 1] : 999999;
    return (candidato < minResto) ? candidato : minResto;
}
```
- **Consignas:**
  - **a.** Deducir el propósito algorítmico y qué ocurre con valores impares. *(Respuesta: Halla recursivamente el valor mínimo par presente en el arreglo, ignorando los impares mediante un centinela alto)*.
  - **b.** Traza manual completa con $V = [33, 14, 28, 9, 6]$, $n=5$. Retorno esperado: **6** (pares evaluados: 14, 28, 6; mínimo = 6).

#### Ejercicio 5: Problema Integrador en C++ con TDAs (45%)
- **Estructuras:** Cola Dinámica (FIFO) + Lista Simplemente Enlazada.
- **Distribución de Caracteres:**
  - Caracteres en **posiciones con índice par** de la palabra original ($0, 2, 4, \dots$) $\to$ Insertados en la **Cola**.
  - Caracteres en **posiciones con índice impar** de la palabra original ($1, 3, 5, \dots$) $\to$ Insertados en la **Lista Enlazada**.
- **Alternancia y Vaciado:**
  - Inicia con la **Cola**:
    1. Desencolar la primera mitad de la Cola ($M_{c1}$).
    2. Extraer del frente la primera mitad de la Lista ($M_{l1}$).
    3. Desencolar los elementos restantes de la Cola ($M_{c2}$).
    4. Extraer los elementos restantes de la Lista ($M_{l2}$).
- **Ejemplo Resuelto en SDD:**
  - Palabra: `"satelital"` (longitud: 9).
  - Índices:
    - `0:'s'`, `1:'a'`, `2:'t'`, `3:'e'`, `4:'l'`, `5:'i'`, `6:'t'`, `7:'a'`, `8:'l'`.
    - Pares (Cola): `'s'`, `'t'`, `'l'`, `'t'`, `'l'` (5 letras).
      - Cola: `frente -> ['s', 't', 'l', 't', 'l'] <- fin`.
    - Impares (Lista): `'a'`, `'e'`, `'i'`, `'a'` (4 letras).
      - Lista: `inicio -> ['a', 'e', 'i', 'a'] -> NULL`.
    - Mitades:
      - Cola (5): $M_{c1} = 3$, $M_{c2} = 2$.
      - Lista (4): $M_{l1} = 2$, $M_{l2} = 2$.
    - Extracción:
      - 1) 3 letras de Cola: `'s'`, `'t'`, `'l'`.
      - 2) 2 letras de Lista: `'a'`, `'e'`.
      - 3) 2 letras de Cola: `'t'`, `'l'`.
      - 4) 2 letras de Lista: `'i'`, `'a'`.
  - **Palabra Codificada Final:** `"stlaetlia"`.

---

### 4.4 Variante 4 (Tema 4: Robótica Industrial & Industria 4.0)
- **Identificador UI:** `tema4.html`
- **Acento cromático:** Ámbar / Rojo Fuego (`border-amber-500/30`, `text-amber-400`, `bg-amber-500/10`).

#### Ejercicio 1: Memoria y Structs Anidados (15%)
```c
struct stArticulacionRobot {
    float AnguloRadianes;       // 4 bytes
    float VelocidadAngular;     // 4 bytes
    float TorqueMotorNm;        // 4 bytes
    unsigned shortint CargaCorrienteMa; // 2 bytes
    char EstadoFreno;           // 1 byte ('A'=Activo, 'L'=Liberado)
    char EjeId[3];              // 3 bytes (ej: "J1")
};                              // Subtotal = 4*3 + 2 + 1 + 3 = 18 bytes

struct stBrazoIndustrial {
    char NumeroSerieCelda[18];      // 18 bytes
    char FabricanteRobot[26];       // 26 bytes
    stArticulacionRobot EjeMuneca;  // 18 bytes
    unsigned int CiclosCompletados; // 4 bytes
    float HorasOperacion;           // 4 bytes
    char ModoOperacion;             // 1 byte ('A'=Auto, 'M'=Manual, 'E'=Emergencia)
    char ModeloControlador[33];     // 33 bytes
};                                  // Subtotal = 18 + 26 + 18 + 4 + 4 + 1 + 33 = 104 bytes
```
- **Consignas:**
  - **a.** Cantidad de bytes de `stArticulacionRobot EjeCentral;` $\to$ **18 bytes**.
  - **b.** Cantidad de bytes de `stBrazoIndustrial LineaMontaje[35];` $\to$ $104 \times 35 =$ **3640 bytes**.

#### Ejercicio 2: Ordenamiento y Búsqueda (20%)
- **Vector Base:** $V = [45, 82, 16, 67, 34, 90, 23, 59]$ ($N=8$).
- **Método de Ordenamiento:** **Método Shell (Shell Sort)**.
  - Saltos decrecientes $k = \lfloor 8/2 \rfloor = 4$, luego $k = 2$, luego $k = 1$.
  - Mostrar intercambios y comparaciones por sub-listas para cada valor de $k$.
  - *Vector Ordenado Final:* $[16, 23, 34, 45, 59, 67, 82, 90]$.
- **Búsqueda Binaria:**
  - **Clave 1 (Éxito):** Buscar $59$.
  - **Clave 2 (Fracaso):** Buscar $40$.

#### Ejercicio 3: Notaciones y Expresiones (15%)
- **Técnica:** **Conversión de Postfija a Infija con Paréntesis Mínimos Requeridos**.
- **Expresión Postfija:**
  `x y + w z - * k 3 ^ / m n * +`
- **Requerimiento:** Emplear una pila de sub-expresiones para reconstruir la notación infija tradicional, insertando paréntesis únicamente donde sea indispensable para no violar la precedencia.
- **Resultado Canónico Reconstruido:**
  $$\frac{(x + y) \cdot (w - z)}{k^3} + m \cdot n$$
  *(En texto: `((x + y) * (w - z)) / k^3 + m * n`)*

#### Ejercicio 4: Recursión con Función Misterio (5%)
```cpp
long long misterio4(const int arr[], int n) {
    if (n == 0) {
        return 1; // Caso base: elemento neutro de la multiplicación
    }
    long long prodParcial = misterio4(arr, n - 1);
    if (arr[n - 1] > 0) {
        return prodParcial * arr[n - 1];
    } else {
        return prodParcial;
    }
}
```
- **Consignas:**
  - **a.** Deducir qué magnitud calcula la función y justificar el valor retornado en el caso base ($1$). *(Respuesta: Productorio acumulado de todos los elementos positivos del vector; el 1 es el neutro multiplicativo que evita anular el resultado)*.
  - **b.** Traza manual completa con $V = [4, -2, 3, 5, -1]$, $n=5$. Retorno esperado: $4 \times 3 \times 5 =$ **60**.

#### Ejercicio 5: Problema Integrador en C++ con TDAs (45%)
- **Estructuras:** Pila Dinámica (LIFO) + Lista Simplemente Enlazada.
- **Distribución de Caracteres:**
  - **Consonantes** $\to$ Insertadas en la **Pila**.
  - **Vocales** $\to$ Insertadas en la **Lista Enlazada**.
- **Alternancia y Vaciado:**
  - Inicia la codificación con la **Lista Enlazada**:
    1. Extraer del frente la primera mitad de la Lista ($M_{l1}$).
    2. Desapilar la primera mitad de la Pila ($M_{p1}$).
    3. Extraer los caracteres restantes de la Lista ($M_{l2}$).
    4. Desapilar los caracteres restantes de la Pila ($M_{p2}$).
- **Ejemplo Resuelto en SDD:**
  - Palabra: `"automatizacion"` (longitud: 14).
  - Distribución:
    - Vocales (Lista): `'a'`, `'u'`, `'o'`, `'a'`, `'i'`, `'a'`, `'i'`, `'o'` (8 vocales).
      - Lista: `inicio -> ['a', 'u', 'o', 'a', 'i', 'a', 'i', 'o'] -> NULL`.
    - Consonantes (Pila): `'t'`, `'m'`, `'t'`, `'z'`, `'c'`, `'n'` (6 consonantes).
      - Pila: `fondo -> ['t', 'm', 't', 'z', 'c', 'n'] <- tope`.
    - Mitades:
      - Lista (8 vocales): $M_{l1} = 4$, $M_{l2} = 4$.
      - Pila (6 consonantes): $M_{p1} = 3$, $M_{p2} = 3$.
    - Extracción:
      - 1) 4 vocales de Lista: `'a'`, `'u'`, `'o'`, `'a'`.
      - 2) 3 consonantes de Pila: `'n'`, `'c'`, `'z'`.
      - 3) 4 vocales de Lista: `'i'`, `'a'`, `'i'`, `'o'`.
      - 4) 3 consonantes de Pila: `'t'`, `'m'`, `'t'`.
  - **Palabra Codificada Final:** `"auoancziaiotmt"`.

---

## 5. Arquitectura de Software Web y Sistema de Diseño (HTML + Tailwind + JS)

### 5.1 Estructura del Árbol de Archivos en `iteracion5`
```
d:\Taller de IA\Examenes\iteracion5\
├── SDD.md                   <-- [Este Documento Rector de Especificación]
├── index.html               <-- Dashboard Hub central para navegación de los 4 temas
├── tema1.html               <-- Examen Interactivo Tema 1 (Finanzas / Cripto)
├── tema2.html               <-- Examen Interactivo Tema 2 (Energía / Smart Grid)
├── tema3.html               <-- Examen Interactivo Tema 3 (Satelital / Espacial)
├── tema4.html               <-- Examen Interactivo Tema 4 (Robótica Industrial)
└── README_VARIANTES.md      <-- Resumen pedagógico comparativo y guía docente
```

### 5.2 Componentes de la Interfaz Web (UI) en cada `temaN.html`

Cada archivo `temaN.html` es una aplicación web de una sola página (*SPA*) completamente funcional, sin compilación externa, con la siguiente anatomía de componentes:

1. **Header Principal con Metadatos:**
   - Badge temático estilizado (Ej: `🪙 Finanzas Digitales`, `⚡ Smart Grid`, etc.).
   - Chip de tiempo estimado (`⏱️ 120-150 min`) y ponderación total (`🎯 100%`).
   - Botón de **Impresión / PDF (`🖨️ Imprimir Examen`)** con reglas `@media print` que formatean la hoja para entregas presenciales.
2. **Barra de Navegación por Pestañas (Tab Controller):**
   - **Tab 1: 📋 Consignas Oficiales:** Renderizado estructurado de los 5 ejercicios con insignias de porcentaje interactivo (tooltips explicativos con la rúbrica al pasar el cursor).
   - **Tab 2: 🧪 Simulador en Vivo:** Herramientas interactivas en JavaScript para que el estudiante o docente valide en tiempo real:
     - *Simulador TDA (Ejercicio 5):* Campo de entrada donde se escribe una palabra, se valida la longitud (5 a 25) y los caracteres alfabéticos, y un visualizador gráfico muestra la carga en la Pila/Cola/Lista y la reconstrucción animada de la palabra codificada.
     - *Simulador de Búsqueda y Ordenamiento (Ejercicio 2):* Animación interactiva de las pasadas del vector y pasos de la búsqueda binaria.
     - *Inspector de Traza Recursiva (Ejercicio 4):* Formulario interactivo para ingresar el vector y el parámetro $k$, mostrando el árbol de llamadas paso a paso.
   - **Tab 3: 📊 Rúbrica y Calculadora Docente:** Matriz de evaluación interactiva con casillas de verificación (*checkboxes*) y controles deslizantes (*range sliders*) que calculan el puntaje acumulado en vivo (0 a 100 puntos) con mensajes cualitativos (*Insuficiente*, *Regular*, *Aprobado*, *Promocionado*).
   - **Tab 4: 💻 Código Base / Starter C++:** Bloque de código C++ pre-configurado con las librerías necesarias, prototipos de función y comentarios guía, acompañado por un botón interactivo **"Copiar al Portapapeles"**.

### 5.3 Estilos y Experiencia Visual (Tailwind CSS)
- **Fondo General:** `bg-slate-950 text-slate-100` con gradientes radiales oscuros.
- **Contenedores:** `bg-slate-900/90 backdrop-blur-md rounded-2xl border border-white/10 shadow-2xl`.
- **Bloques de Código:** Formato de terminal IDE (`bg-[#1e1e1e]`, texto en `Fira Code`, sintaxis destacada con etiquetas span y colores VS Code).
- **Estilos de Impresión (`@media print`):**
  - Ocultamiento de botones de navegación, simuladores y sliders (`display: none !important`).
  - Fondo blanco y texto negro puro para optimizar tóner y nitidez de fotocopias.
  - Saltos de página inteligentes (`page-break-inside: avoid;`).

---

## 6. Rúbrica Estándar de Corrección Unificada (100%)

La siguiente tabla define el desglose oficial de corrección aplicado de forma homogénea a las cuatro variantes:

| Bloque | Ponderación | Sub-criterio Evaluado | Criterio de Corrección |
| :--- | :---: | :--- | :--- |
| **Ejercicio 1: Memoria** | **15%** | **a. Variable Simple (7.5%)**<br>**b. Arreglo Unidimensional (7.5%)** | Deducción exacta de bytes de tipos primitivos (`float`=4, `short`=2, `char`=1, `int`=4) y structs anidados.<br>Multiplicación sin errores por la dimensión del vector ($N$). |
| **Ejercicio 2: Ordenamiento y Búsqueda** | **20%** | **Ordenamiento Paso a Paso (12%)**<br>**Búsqueda Binaria - Éxito (4%)**<br>**Búsqueda Binaria - Fracaso (4%)** | Gráfica y seguimiento riguroso de pasadas según el algoritmo exigido.<br>Tabla con límites (`izq`, `der`, `medio`), elemento comparado y decisión lógica. |
| **Ejercicio 3: Notaciones** | **15%** | **Conversión / Evaluación (15%)** | Aplicación correcta de precedencia de operadores, uso de pilas de control o construcción de árbol sintáctico con sus tres recorridos. |
| **Ejercicio 4: Recursión** | **5%** | **a. Análisis Conceptual (2.5%)**<br>**b. Traza Manual de Escritorio (2.5%)** | Identificación precisa de caso(s) base y caso(s) recursivo(s) con explicación clara.<br>Árbol de llamadas, parámetros en cada nivel y retorno exacto. |
| **Ejercicio 5: Problema C++ con TDAs** | **45%** | **Carga y Control de Palabra (5%)**<br>**Carga en Estructuras TDA (10%)**<br>**Algoritmo de Codificación y Vaciado (10%)**<br>**Muestra de Estructuras Intermedias (5%)**<br>**Menú Modular y Documentación (5%)**<br>**Implementación / Modificación de TDAs (10%)** | Validación estricta de 5 a 25 caracteres, solo letras sin espacios.<br>Criterio de partición exacto.<br>Lógica de mitades $(\lfloor L/2 \rfloor + 1)$ y vaciado total de estructuras.<br>Función de visualización sin corromper el TDA.<br>Bucle interactivo con menú `switch` y buenas prácticas.<br>Manejo seguro de punteros y memoria dinámica en C++. |

---

## 7. Criterios de Aceptación y Validación de Calidad

Para dar por aprobada la implementación de la Iteración 5, los artefactos deberán cumplir con los siguientes puntos de control:

- [ ] **Checklist Pedagógico:**
  - Cada variante totaliza exactamente 100% en su rúbrica.
  - Ningún método de ordenamiento se repite entre las 4 variantes (Quicksort, Inserción, Burbuja con centinela y Shell).
  - Los 4 ejercicios de notaciones exploran técnicas disímiles (Prefija, Postfija con pila, Árbol sintáctico y Postfija a Infija).
  - Todas las funciones misterio tienen casos base y recursivos verificados matemáticamente.
  - El ejercicio 5 cuenta con una solución demostrada paso a paso en el SDD.
- [ ] **Checklist Web y Frontend:**
  - Todos los archivos `.html` se abren localmente sin requerir servidor HTTP ni Node.js.
  - Tailwind CSS carga correctamente vía CDN con diseño responsivo (móvil, tablet y desktop).
  - El sistema de pestañas conmuta instantáneamente sin saltos de scroll indeseados.
  - Los simuladores en JavaScript validan entradas inválidas y presentan retroalimentación visual clara.
  - La hoja de estilos de impresión genera un documento prolijo y legible en hojas A4.
  - El archivo `index.html` vincula de manera bidireccional los 4 exámenes.

---

## 8. Siguientes Pasos

Una vez validada esta especificación SDD, se procederá a:
1. Crear el dashboard central [`index.html`](index.html) con selector de temas y matriz comparativa.
2. Desarrollar de forma modular [`tema1.html`](tema1.html), [`tema2.html`](tema2.html), [`tema3.html`](tema3.html) y [`tema4.html`](tema4.html).
3. Redactar el documento resumen [`README_VARIANTES.md`](README_VARIANTES.md).
