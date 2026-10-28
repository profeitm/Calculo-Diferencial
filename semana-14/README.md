# 📐 Diferenciación Implícita en Curvas Planas Clásicas y Notables
### Taller Avanzado: Análisis de Tangentes y Geometría de Curvas Implícitas Especiales (Guía Completa)

**Asignatura:** Cálculo Diferencial Virtual (Código: VXRCD03)  
**Unidad Temática:** Unidad 5 – Técnicas Avanzadas de Derivación y Aplicaciones  
**Profesor-Tutor:** Alexander Arias Londoño  
**Semillero de Investigación:** MMCC (*Modelamiento Matemático y Cómputo Científico*) – ITM  
**Texto Guía Base:** *Cálculo: Trascendentes Tempranas* – Dennis G. Zill & Warren S. Wright (4.ª Edición), Sección 3.6.

---

## 📌 1. Nombres Propuestos para el Tema / Taller

* **Nombre Principal (Recomendado):**
  * **"Diferenciación Implícita en Curvas Planas Clásicas y Notables"**
* **Opciones Alternativas según el Enfoque:**
  * **Enfoque Histórico-Geométrico:** *"Geometría Analítica y Tangentes en Curvas Históricas Famosas"*
  * **Enfoque Taller / Moodle:** *"Taller Avanzado: Análisis de Tangentes y Geometría de Curvas Implícitas Especiales"*
  * **Enfoque de Modelado:** *"Geometría Diferencial de Curvas Especiales del Cálculo"*

---

## 🏛️ 2. Introducción al Tema y a los 5 Ejercicios

En el estudio del Cálculo Diferencial, la mayoría de los primeros acercamientos a la derivada se realizan sobre funciones explícitas de la forma $y = f(x)$. Sin embargo, en la geometría analítica y en el modelamiento de fenómenos físicos y de ingeniería, las relaciones entre variables con frecuencia se presentan mediante ecuaciones donde la variable dependiente $y$ se encuentra entrelazada de forma inseparable con $x$, dando lugar a ecuaciones implícitas de la forma $F(x, y) = 0$.

Tras abordar ejemplos fundamentales como el **Folio de Descartes**, el estudio de las **Curvas Planas Clásicas** —como la *Cisoide de Diocles*, la *Lemniscata de Bernoulli*, el *Bifolio*, la *Bruja de Agnesi* y el *Astroide*— constituye el escenario ideal para profundizar en la **Diferenciación Implícita**. Estas curvas geométricas inmortalizadas entre los siglos III a. C. y XVIII no solo poseen un elevado valor histórico y estético, sino que exigen la aplicación rigurosa de la regla de la cadena, la regla del producto y el manejo de potencias racionales o cuadráticas compuestas.

A través de este bloque de 5 ejercicios emblemáticos, el estudiante transita de la simple ejecución operativa hacia el análisis geométrico avanzado: la determinación de rectas tangentes y normales, la localización de puntos con tangentes horizontales o verticales, y la comprensión de lazos, simetrías y asíntotas, conectando el rigor del álgebra analítica con la verificación gráfica computacional en herramientas como **GeoGebra**.

---

## ⚙️ 3. Marco Teórico y Algoritmo General de Diferenciación Implícita

1. **Diferenciación:** Derivar ambos miembros de la ecuación respecto a $x$.
2. **Regla de la Cadena en $y$:** Aplicar la regla de la cadena a cada término que contenga $y$, recordando que $\frac{d}{dx}[y] = y'$ y $\frac{d}{dx}[y^n] = n y^{n-1} y'$.
3. **Agrupación:** Reunir todos los términos con $y'$ en el miembro izquierdo y trasladar el resto al lado derecho.
4. **Despeje:** Factorizar $y'$ y despejar la expresión analítica de la derivada $\frac{dy}{dx}$.
5. **Ecuación de Tangente y Normal:** Evaluada la pendiente $m = \left.\frac{dy}{dx}\right|_{(x_0, y_0)}$, la recta tangente es $y - y_0 = m(x - x_0)$ y la normal es $y - y_0 = -\frac{1}{m}(x - x_0)$.

---

## 🌀 4. El Modelo Canónico: El Folio de Descartes

La curva $x^3 + y^3 = 6xy$ representa el arquetipo de la diferenciación implícita.

### 📐 Problema 0: Análisis de Tangente y Normal en el Folio
Dada la ecuación del Folio de Descartes $x^3 + y^3 = 6xy$:
1. Obtener $\frac{dy}{dx}$ implícitamente.
2. Determinar la recta tangente y normal en el punto $P(3, 3)$.

#### ✍️ Solución Paso a Paso:
1. **Derivación término a término:**
   $$\frac{d}{dx}[x^3] + \frac{d}{dx}[y^3] = \frac{d}{dx}[6xy]$$
   $$3x^2 + 3y^2 \frac{dy}{dx} = 6y(1) + 6x \frac{dy}{dx}$$

2. **Agrupación y Despeje:**
   $$3y^2 \frac{dy}{dx} - 6x \frac{dy}{dx} = 6y - 3x^2 \implies \frac{dy}{dx}(3y^2 - 6x) = 6y - 3x^2$$
   $$\frac{dy}{dx} = \frac{6y - 3x^2}{3y^2 - 6x} = \frac{2y - x^2}{y^2 - 2x}$$

3. **Evaluación de la Pendiente en $P(3, 3)$:**
   $$m = \left.\frac{dy}{dx}\right|_{(3,3)} = \frac{2(3) - 3^2}{3^2 - 2(3)} = \frac{6 - 9}{9 - 6} = \frac{-3}{3} = -1$$

4. **Ecuaciones de las Rectas:**
   * **Recta Tangente:** $y - 3 = -1(x - 3) \implies x + y = 6 \quad \text{o} \quad y = -x + 6$
   * **Recta Normal:** $m_N = 1 \implies y - 3 = 1(x - 3) \implies y = x$

---

## 🎯 5. Bloque de 5 Curvas Planas Clásicas y Notables

### 1️⃣ La Cisoide de Diocles
* **Ecuación Implícita:** $(4 - x)y^2 = x^3$
* **Contexto:** Concebida en la antigua Grecia (siglo II a. C.) para resolver el problema de la duplicación del cubo. Presenta una asíntota vertical en $x = 4$ y una cúspide en el origen.

#### ✍️ Solución Paso a Paso:
1. **Derivación Implícita (Regla del Producto en el lado izquierdo):**
   $$\frac{d}{dx}\left[(4 - x)y^2\right] = \frac{d}{dx}[x^3]$$
   $$(-1)y^2 + (4 - x)\cdot 2y \frac{dy}{dx} = 3x^2$$
   $$2y(4 - x)\frac{dy}{dx} = 3x^2 + y^2 \implies \frac{dy}{dx} = \frac{3x^2 + y^2}{2y(4 - x)}$$

2. **Recta Tangente en $P(2, 2)$:**
   $$m = \left.\frac{dy}{dx}\right|_{(2,2)} = \frac{3(2)^2 + 2^2}{2(2)(4 - 2)} = \frac{12 + 4}{4(2)} = \frac{16}{8} = 2$$
   $$y - 2 = 2(x - 2) \implies y = 2x - 2$$

---

### 2️⃣ La Lemniscata de Bernoulli
* **Ecuación Implícita:** $3(x^2 + y^2)^2 = 100xy$
* **Contexto:** Curva en forma de '8' acostado propuesta por Jakob Bernoulli en 1694.

#### ✍️ Solución Paso a Paso:
1. **Derivación Implícita (Regla de la Cadena y del Producto):**
   $$6(x^2 + y^2)\left(2x + 2y \frac{dy}{dx}\right) = 100\left(y + x \frac{dy}{dx}\right)$$
   $$12(x^2 + y^2)\left(x + y \frac{dy}{dx}\right) = 100\left(y + x \frac{dy}{dx}\right)$$
   $$3(x^2 + y^2)\left(x + y \frac{dy}{dx}\right) = 25\left(y + x \frac{dy}{dx}\right)$$
   $$\left[3y(x^2 + y^2) - 25x\right]\frac{dy}{dx} = 25y - 3x(x^2 + y^2)$$
   $$\frac{dy}{dx} = \frac{25y - 3x(x^2 + y^2)}{3y(x^2 + y^2) - 25x}$$

2. **Recta Tangente en $P(3, 1)$:**
   Como $x^2 + y^2 = 3^2 + 1^2 = 10$:
   $$m = \frac{25(1) - 3(3)(10)}{3(1)(10) - 25(3)} = \frac{25 - 90}{30 - 75} = \frac{-65}{-45} = \frac{13}{9}$$
   $$y - 1 = \frac{13}{9}(x - 3) \implies 13x - 9y = 30$$

---

### 3️⃣ El Bifolio (Bifolium)
* **Ecuación Implícita:** $(x^2 + y^2)^2 = 4x^2 y$
* **Contexto:** Curva de cuarto grado que forma dos lazos ("hojas") simétricos alineados con el eje $Y$.

#### ✍️ Solución Paso a Paso:
1. **Derivación Implícita:**
   $$2(x^2 + y^2)\left(2x + 2y \frac{dy}{dx}\right) = 4\left(2xy + x^2 \frac{dy}{dx}\right)$$
   $$(x^2 + y^2)\left(x + y \frac{dy}{dx}\right) = 2xy + x^2 \frac{dy}{dx}$$
   $$\left[y(x^2 + y^2) - x^2\right]\frac{dy}{dx} = 2xy - x(x^2 + y^2)$$
   $$\frac{dy}{dx} = \frac{2xy - x(x^2 + y^2)}{y(x^2 + y^2) - x^2}$$

2. **Recta Tangente en $P(1, 1)$:**
   Como $x^2 + y^2 = 2$:
   $$m = \frac{2(1)(1) - 1(2)}{1(2) - 1^2} = \frac{2 - 2}{2 - 1} = 0$$
   * **Recta Tangente (Horizontal):** $y = 1$
   * **Recta Normal (Vertical):** $x = 1$

---

### 4️⃣ La Bruja de Agnesi
* **Ecuación Implícita:** $(x^2 + 4)y = 8$
* **Contexto:** Curva suave en forma de campana estudiada por Maria Gaetana Agnesi en 1748.

#### ✍️ Solución Paso a Paso:
1. **Derivación Implícita:**
   $$2x \cdot y + (x^2 + 4)\frac{dy}{dx} = 0 \implies \frac{dy}{dx} = -\frac{2xy}{x^2 + 4}$$

2. **Recta Tangente en $P(2, 1)$:**
   $$m = -\frac{2(2)(1)}{2^2 + 4} = -\frac{4}{8} = -\frac{1}{2}$$
   $$y - 1 = -\frac{1}{2}(x - 2) \implies x + 2y = 4 \quad \text{o} \quad y = -\frac{1}{2}x + 2$$
   * **Recta Normal:** $m_N = 2 \implies y = 2x - 3$

---

### 5️⃣ El Astroide (Hipocicloide de 4 Cúspides)
* **Ecuación Implícita:** $x^{2/3} + y^{2/3} = 4$  (con $a = 8$, de modo que $a^{2/3} = 4$)
* **Contexto:** Curva trazada por un punto de una circunferencia que rueda dentro de otra de radio 4 veces mayor.

#### ✍️ Solución Paso a Paso:
1. **Derivación Implícita:**
   $$\frac{2}{3}x^{-1/3} + \frac{2}{3}y^{-1/3}\frac{dy}{dx} = 0 \implies \frac{dy}{dx} = -\frac{x^{-1/3}}{y^{-1/3}} = -\sqrt[3]{\frac{y}{x}}$$

2. **Recta Tangente en $P(3\sqrt{3}, 1)$:**
   Como $x = 3\sqrt{3} = 3^{3/2} \implies x^{1/3} = \sqrt{3}$ y $y = 1 \implies y^{1/3} = 1$:
   $$m = -\frac{1}{\sqrt{3}} = -\frac{\sqrt{3}}{3}$$
   $$y - 1 = -\frac{\sqrt{3}}{3}(x - 3\sqrt{3}) \implies y = -\frac{\sqrt{3}}{3}x + 4$$

3. **Demostración Geométrica de la Longitud Constante del Segmento Tangente:**
   * Intersección eje $Y$ ($x = 0$): $A(0, 4)$
   * Intersección eje $X$ ($y = 0$): $0 = -\frac{\sqrt{3}}{3}x + 4 \implies x = 4\sqrt{3} \implies B(4\sqrt{3}, 0)$
   * Distancia entre $A$ y $B$:
     $$D = \sqrt{(4\sqrt{3} - 0)^2 + (0 - 4)^2} = \sqrt{48 + 16} = \sqrt{64} = 8$$
   ¡La longitud del segmento tangente entre los ejes es exactamente constante e igual a $2a = 8$ para cualquier punto de la curva!

---

## 📊 6. Tabla Cuadro Comparativo de Curvas Clásicas

| Curva Clásica | Ecuación Implícita | Expresión de la Derivada $\frac{dy}{dx}$ | Punto Evaluado | Pendiente $m$ | Ecuación Recta Tangente |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Folio de Descartes** | $x^3 + y^3 = 6xy$ | $\frac{2y - x^2}{y^2 - 2x}$ | $(3, 3)$ | $m = -1$ | $x + y = 6$ |
| **Cisoide de Diocles** | $(4 - x)y^2 = x^3$ | $\frac{3x^2 + y^2}{2y(4 - x)}$ | $(2, 2)$ | $m = 2$ | $y = 2x - 2$ |
| **Lemniscata de Bernoulli** | $3(x^2 + y^2)^2 = 100xy$ | $\frac{25y - 3x(x^2 + y^2)}{3y(x^2 + y^2) - 25x}$ | $(3, 1)$ | $m = \frac{13}{9}$ | $13x - 9y = 30$ |
| **Bifolio (Bifolium)** | $(x^2 + y^2)^2 = 4x^2 y$ | $\frac{2xy - x(x^2 + y^2)}{y(x^2 + y^2) - x^2}$ | $(1, 1)$ | $m = 0$ | $y = 1$ |
| **Bruja de Agnesi** | $(x^2 + 4)y = 8$ | $-\frac{2xy}{x^2 + 4}$ | $(2, 1)$ | $m = -\frac{1}{2}$ | $x + 2y = 4$ |
| **Astroide** | $x^{2/3} + y^{2/3} = 4$ | $-\sqrt[3]{\frac{y}{x}}$ | $(3\sqrt{3}, 1)$ | $m = -\frac{\sqrt{3}}{3}$ | $y = -\frac{\sqrt{3}}{3}x + 4$ |

---

## 💻 7. Instrucciones para Verificación en GeoGebra

1. En GeoGebra Graphing / Suite, introduce la ecuación implícita directamente en la entrada de comandos (ej. `x^3 + y^3 = 6*x*y`).
2. Crea el punto $P$ sobre la curva (ej. `P = (3, 3)`).
3. Utiliza el comando `Tangente[P, c]` donde `c` es el nombre de la curva para visualizar la recta tangente y verificar analíticamente la pendiente.
