# Capítulo 1: Termodinámica

## Tópicos Fundamentales

### Los Objetos de la Termodinámica

A continuación, se describen los conceptos y términos fundamentales empleados en la termodinámica. Para favorecer la claridad pedagógica, se prioriza la comprensión conceptual sobre el rigor formal extremo en ciertas definiciones.

* **Sistema:** Son las entidades macroscópicas objeto de estudio, capaces de ser sometidas a procesos de medición convencionales. Están constituidos por un gran número de constituyentes (moléculas, átomos, electrones, etc.) o por campos de fuerza (como el electromagnético). Se definen como sistemas dinámicos con un número extremadamente elevado de grados de libertad; aquellos con pocos grados de libertad no pertenecen al ámbito de estudio de la termodinámica.
* **Ambiente:** Representa el entorno o alrededores del objeto de estudio. Si una porción del universo es seleccionada como sistema, el resto constituye el ambiente. Este actúa definiendo las condiciones impuestas al sistema, tales como temperatura, presión, potencial químico o volumen constantes.
* **Sistema Aislado:** Es aquel sistema independiente que no posee interacción alguna con sus alrededores.
* **Sistema Cerrado:** Es un sistema que no intercambia materia con su ambiente, aunque puede intercambiar energía.
* **Sistema Abierto:** Es aquel que permite el intercambio tanto de materia como de energía con sus alrededores.


### El Concepto de Equilibrio 4ermodinámico (Ley Cero de la Termodinámica)

* **Equilibrio Termodinámico de un Sistema Aislado:** Independientemente de la complejidad de su estado inicial, si un sistema aislado evoluciona libremente, alcanzará eventualmente un estado final estacionario. Este estado se denomina equilibrio térmico o termodinámico.
* **Equilibrio Térmico de dos Sistemas:** Al poner en contacto dos sistemas aislados ($A$ y $B$), el sistema compuesto ($A+B$) relajará con el tiempo hacia un estado de equilibrio. En este punto, se dice que $A$ y $B$ están en equilibrio entre sí, encontrándose también cada uno en su propio equilibrio termodinámico. Esta condición de equilibrio es persistente: no se pierde si el contacto se interrumpe y se restaura posteriormente. Por lo tanto, dos sistemas están en equilibrio térmico ($A \sim B$) si sus estados permanecen inalterados al ser puestos en contacto.
* **Ley Cero de la Termodinámica (Ley de Transitividad del Equilibrio):** Establece que si el sistema $A$ está en equilibrio con el sistema $B$, y a su vez $B$ está en equilibrio con el sistema $C$, entonces $A$ y $C$ están necesariamente en equilibrio térmico entre sí:

$$
A \sim B, \quad B \sim C \quad \rightarrow \quad A \sim C.
$$

* **Estado Termodinámico:** Aunque frecuentemente se utiliza como sinónimo de estado de equilibrio, en un sentido más general, un sistema compuesto se encuentra en un estado termodinámico si sus partes constituyentes poseen equilibrio térmico local, incluso si el sistema total aún no ha alcanzado el equilibrio global.


### Contacto Termodinámico

Se denominan contactos termodinámicos a aquellos vínculos que permiten las siguientes interacciones:

* **Interacción Mecánica:** Ocurre cuando un sistema realiza trabajo sobre otro mediante fuerzas mecánicas o campos electromagnéticos.
* **Interacción Térmica:** Es el intercambio de energía en forma de calor (ya sea por conducción o radiación). Una pared que impide este intercambio se denomina adiabática.
* **Interacción de Masa:** Aquella que involucra el transporte de materia entre dos sistemas.


### Cantidades Termodinámicas

* **Cantidades de Estado:** Son magnitudes físicas que poseen un valor unívoco y bien definido para cada estado de equilibrio del sistema.
* **Variables de Estado o Termodinámicas:** Generalmente coinciden con las cantidades de estado, pero en un contexto más amplio, definen las propiedades físicas del equilibrio local. Al seleccionar un conjunto apropiado de variables independientes que resulten necesarias y suficientes para describir el equilibrio, las demás propiedades se convierten en funciones de estas. El número de variables independientes (grados de libertad termodinámicos) se determina de manera empírica.
* **Cantidades Intensivas y Extensivas:** Si un sistema en equilibrio se divide en partes mediante paredes impermeables, rígidas y adiabáticas, cada fracción conserva el equilibrio original. Las propiedades que son iguales en todos los subsistence, y por lo tanto independientes del tamaño o extensión (como la temperatura, la presión o el potencial químico) se denominan intensivas. Por el contrario, las propiedades que varían proporcionalmente a la extensión o masa del sistema (como la energía, la entropía o la masa de los componentes) se denominan extensivas.


### Procesos Termodinámicos

La termodinámica se enfoca en procesos donde los estados inicial y final son estados termodinámicos. Los estados intermedios suelen ser complejos y fuera del equilibrio, a menos que el proceso ocurra con extrema lentitud. Son de particular interés los siguientes tipos de procesos:

* **Ciclo:** Proceso en el cual el estado final es idéntico al inicial.
* **Proceso Infinitesimal:** Aquel donde la diferencia entre el estado inicial y final es infinitamente pequeña.
* **Proceso Reversible:** Es un proceso ideal donde el camino inverso puede ocurrir de manera espontánea, devolviendo al sistema y al ambiente a sus condiciones originales.
* **Proceso Cuasiestático:** Es un proceso idealizado en el que todos los estados intermedios son estados de equilibrio local. Se logra mediante cambios infinitamente lentos. Cabe destacar que, si bien todos los procesos reversibles son cuasiestáticos, no todos los procesos cuasiestáticos son reversibles (por ejemplo, una sucesión de expansiones libres infinitesimales e infinitamente lentas).


## Leyes de la Termodinámica

### Ley Cero de la Termodinámica

Basada en el principio de transitividad del equilibrio termodinámico, esta ley postula la existencia de una función de estado escalar denominada temperatura ($T$). De acuerdo con este postulado, dos sistemas aislados $A$ y $B$ se encuentran en equilibrio térmico entre sí si, y solo si, sus temperaturas son iguales:

$$
T_{A} = T_{B}.
$$

### Primera Ley de la Termodinámica

Esta ley representa el principio de conservación de la energía aplicado a sistemas termodinámicos. Postula la existencia de una propiedad intrínseca del sistema llamada energía interna ($U$).

Cuando un sistema transita de un estado inicial (1) a un estado final (2), el cambio neto de su energía interna es igual a la suma de las energías transferidas a través de su frontera en forma de trabajo mecánico ($W$), calor ($Q$) y trabajo químico ($Z$). Esta variación depende exclusivamente de los estados inicial y final, siendo independiente de la trayectoria o procesos intermedios seguidos:

$$
U_{2} - U_{1} = W + Q + Z.
$$

Para procesos infinitesimales, la primera ley se expresa en forma diferencial como:

$$
dU = d'Q + d'W + d'Z.
$$

Es fundamental notar el uso del símbolo $d'$ para el calor, el trabajo mecánico y el trabajo químico. Esto indica que estas cantidades no son diferenciales exactas, ya que sus valores dependen de la trayectoria específica del proceso y no son funciones de estado. Cualquier proceso cíclico que pretenda generar trabajo neto sin consumo de energía violaría esta ley; tales dispositivos se denominan móviles perpetuos de primera especie.

### Segunda Ley de la Termodinámica

La segunda ley introduce el concepto de entropía ($S$), una función de estado extensiva que determina la dirección de los procesos espontáneos y la degradación de la energía. Matemáticamente, para un sistema que pasa de un estado $A$ a un estado $B$, se cumple la desigualdad de Clausius:

$$
\int_{A}^{B} \frac{d'Q}{T} \leq S(B) - S(A)
$$

* La igualdad rige para procesos reversibles.
* La desigualdad estricta rige para procesos irreversibles (espontáneos).

Cualquier proceso que resulte en una disminución neta de la entropía del universo (sistema más alrededores) es físicamente imposible. Los dispositivos que pretendan convertir íntegramente calor en trabajo en un ciclo operando con una sola fuente térmica se conocen como móviles perpetuos de segunda especie y están prohibidos por esta ley.

### Tercera Ley de la Termodinámica

Este postulado establece que la entropía de un sistema en equilibrio térmico se aproxima a una constante universal cuando la temperatura absoluta tiende a cero. Dicha constante puede tomarse, por convención, como nula. Se suele presentar en dos niveles de generalidad:

* **Forma Débil (Teorema de Nernst):** $$
\lim_{T \rightarrow 0} \left( \frac{\partial S}{\partial X_{i}} \right)_{X_{j}, T} = 0.
$$
* **Forma Fuerte (Postulado de Planck):** $$
\lim_{T \rightarrow 0} S = 0.
$$


## Consideraciones Sobre la Ley Cero

### Construcción de un Termómetro

La construcción de un termómetro requiere identificar una propiedad termométrica $y$ tal que $y=f(T)$. En el enfoque más elemental, se asume una dependencia lineal:

$$
y = a + bT.
$$

Para determinar las constantes $a$ y $b$, se seleccionan dos estados patrón $(y_1, y_2)$ con temperaturas asignadas $(T_1, T_2)$:

$$
b = \frac{y_{2} - y_{1}}{T_{2} - T_{1}} \quad \text{y} \quad a = y_{1} - bT_{1}.
$$

**Requisitos Indispensables:** Todos los termómetros deberían proporcionar el mismo valor para un sistema dado. Sin embargo, la suposición de linealidad de las propiedades físicas suele ser una aproximación, lo que genera discrepancias entre distintos tipos de termómetros.

### Termómetro de Gas a Volumen Constante

Este dispositivo proporciona lecturas independientes de la sustancia de trabajo en el límite de densidades muy bajas pues la presión de un gas diluido varía linealmente con la temperatura; esta escala será validada posteriormente mediante la Segunda Ley.

## Consideraciones sobre la Primera Ley

### Energía interna ($U$)

Representa la energía total del sistema, excluyendo efectos cinéticos o potenciales macroscópicos. La Primera Ley enfatiza que $U$ es una función de estado. Microscópicamente, equivale a la suma de energías cinéticas e interacciones moleculares, aunque la termodinámica clásica se limita a su comportamiento macroscópico.

### El calor y el Trabajo como Funciones de Trayectoria

A diferencia de $U$, el trabajo mecánico ($W$), el trabajo químico ($Z$) y el calor ($Q$) dependen del tipo de proceso realizado. No son cantidades de estado. No obstante, la Primera Ley establece que la suma $W + Q + Z$ es igual a la variación de la energía interna ($\Delta U$), la cual sí es independiente de la trayectoria.

### Móvil Perpetuo de Primera Especie

En un ciclo ($\Delta U = 0$), se cumple que $W + Q + Z = 0$. Un sistema solo puede realizar trabajo a expensas de absorber calor o masa. La Primera Ley prohíbe el "móvil perpetuo de primera especie", que es aquel que produciría trabajo sin consumo de energía.

## Consideraciones sobre la Segunda Ley

### Postulados Originales

La Segunda Ley de la Termodinámica puede enunciarse a través de dos proposiciones fundamentales que subrayan la irreversibilidad de los procesos naturales:

* **Postulado de Kelvin:** No existe proceso termodinámico cuyo único efecto sea la extracción de calor de una fuente a una temperatura determinada y su conversión íntegra en trabajo.
* **Postulado de Clausius:** No existe proceso termodinámico cuyo único efecto sea la extracción de calor de una fuente fría y su transferencia hacia una fuente más caliente.

La equivalencia entre ambos se demuestra comprobando que la negación de uno invalida necesariamente al otro.

**I. Si Clausius es Falso $\implies$ Kelvin es Falso:** Supongamos un refrigerador capaz de extraer calor $Q_2$ de un foco frío y entregarlo a uno caliente con un trabajo $W = 0$. Si una máquina térmica convencional extrae $Q_1$ del foco caliente, produce un trabajo $W$ y libera $Q_2$ al foco frío, el refrigerador "devolvería" dicho $Q_2$ al foco caliente. El efecto neto sería la extracción de calor $(Q_1 - Q_2)$ de una sola fuente para producir trabajo, violando así el postulado de Kelvin.

**II. Si Kelvin es Falso $\implies$ Clausius es Falso:** Supongamos un motor que convierte íntegramente el calor $Q$ en trabajo $W$. Si empleamos ese trabajo para accionar un refrigerador que extrae $Q_f$ de un foco frío, este entregaría $Q_f + W$ al foco caliente. El resultado neto es el flujo de calor $Q_f$ desde el foco frío al caliente sin aporte externo neto, violando el postulado de Clausius.

### El Teorema de Carnot

**La Máquina de Carnot:** Se define como una máquina térmica ideal que opera entre dos fuentes de temperatura, en la cual todos los procesos que conforman el ciclo son reversibles.

**Teorema de Carnot:** Ninguna máquina térmica que opere entre dos fuentes de temperatura dadas puede ser más eficiente que una máquina de Carnot trabajando entre las mismas fuentes.

**Demostración:** Consideremos dos máquinas operando entre las mismas fuentes con eficiencias $\eta_I$ (irreversible) y $\eta_R$ (reversible), produciendo el mismo trabajo $W$. Si suponemos que $\eta_I > \eta_R$, entonces $Q_I < Q_R$ (la máquina $I$ consume menos calor del foco caliente).

1. Utilizamos el trabajo $W$ generado por $I$ para accionar a $R$ en reversa (como refrigerador).
2. El foco caliente recibe $Q_R$ y entrega $Q_I$; el balance neto es un flujo de entrada $Q_R - Q_I > 0$.
3. El foco frío entrega calor para compensar el ciclo sin aporte de trabajo externo.
4. Como resultado, el calor fluye espontáneamente del foco frío al caliente, lo que contradice el postulado de Clausius.
5. **Conclusión:** Por reducción al absurdo, debe cumplirse que $\eta_I \leq \eta_R$.

**Corolario:** Todas las máquinas de Carnot que operan entre las mismas dos fuentes de temperatura poseen la misma eficiencia. Utilizando un gas ideal, se encuentra que la eficiencia de Carnot $\eta_{C}$ es:

$$
\eta_{C} = 1 - \frac{T_{2}}{T_{1}},
$$

donde $T_1$ y $T_2$ ($T_1 > T_2$) son las temperaturas medidas con el termómetro de gas ideal a volumen constante.

### Escala Absoluta de Temperaturas

El teorema de Carnot permite definir una escala de temperatura independiente de la sustancia de trabajo. Manipulando algebraicamente la expresión de eficiencia de Carnot:

$$
\frac{T_{2}}{T_{1}} = 1 - \eta_{C}.
$$

Puesto que $0 \leq \eta_{C} \leq 1$, la temperatura absoluta debe ser siempre positiva. Para establecer una escala uniforme, se construye una serie de máquinas de Carnot acopladas (el calor expulsado por una es absorbido por la siguiente) que realicen el mismo trabajo $W$. La eficiencia de la $n$-ésima máquina es:

$$
1 - \frac{Q_{n+1}}{Q_{n}} = 1 - \frac{T_{n+1}}{T_{n}} \implies \frac{T_{n}}{Q_{n}} = \frac{T_{n+1}}{Q_{n+1}} = x.
$$

Esto implica que $T_{n} - T_{n+1} = x W$. Al elegir $W$ de forma que $xW = 1$ K, se obtiene la escala Kelvin.

* Esta escala es absoluta pues depende únicamente de la Segunda Ley de la Termodinámica.
* El cero absoluto ($T = 0$) es el límite inferior de temperatura e inaccesible según la tercera ley.


### Teorema de Clausius

En cualquier transformación cíclica donde la temperatura esté bien definida, se cumple la desigualdad de Clausius:

$$
\oint \frac{d Q}{T} \leq 0.
$$

La igualdad se satisface estrictamente en procesos reversibles.

**Demostración (Caso Discreto):** Sea un sistema que intercambia calores $Q_i$ con fuentes a temperaturas $T_i$.

1. Acoplamos cada fuente $T_i$ a un depósito común $T_0$ mediante máquinas de Carnot reversibles.
2. Para cada máquina $i$, el calor extraído de $T_0$ es $Q_{0,i} = T_0 \frac{Q_i}{T_i}$.
3. El sistema total solo intercambia calor con $T_0$. Según el postulado de Kelvin, el trabajo neto $W_{total}$ no puede ser positivo: $W_{total} = Q_{0,total} = \sum Q_{0,i} \leq 0$.
4. Sustituyendo: $\sum T_0 \frac{Q_i}{T_i} \leq 0$. Como $T_0 > 0$, se obtiene $\sum \frac{Q_i}{T_i} \leq 0$.

Para el **Caso Continuo**, al hacer los intercambios infinitesimales ($dQ$) a través de una trayectoria cíclica, la sumatoria se convierte en una integral de línea: $\oint \frac{dQ}{T} \leq 0$.

**Corolario:** Para una transformación reversible, la integral $\int_{A}^{B} \frac{d Q}{T}$ es independiente de la trayectoria, ya que sobre un ciclo cerrado la integral es nula. Esto implica que el resultado depende únicamente de los estados inicial y final.

### Definición de Entropía

La independencia de la trayectoria permite definir una función de estado llamada entropía ($S$) para cualquier estado $A$:

$$
S(A) = \int_{0}^{A} \frac{d Q}{T},
$$

donde $0$ es un estado de referencia arbitrario y la integración se realiza sobre una trayectoria reversible. Así, la diferencia de entropía entre dos estados es:

$$
S(B) - S(A) = \int_{A}^{B} \frac{d Q}{T} \implies d S = \frac{d Q}{T},
$$

donde $dS$ constituye una diferencial exacta.

### Formulación más General de la Segunda Ley

Cualquier proceso que lleve al sistema de un estado $A$ a un estado $B$ debe satisfacer:

$$
\int_{A}^{B} \frac{d Q}{T} \leq S(B) - S(A).
$$

En el caso particular de un sistema aislado (paredes adiabáticas, $dQ = 0$), se tiene que:

$$
S(B) - S(A) \geq 0.
$$

## Ecuación Fundamental (Representación de la Energía Interna)

Para resolver un sistema termodinámico de manera completa, se requiere, además de las leyes generales, información específica sobre la naturaleza del sistema en cuestión. El primer paso para ello es caracterizar el tipo de entidades bajo estudio.

**Sistemas Simples:** Se definen como sistemas macroscópicamente homogéneos, isotrópicos y eléctricamente neutros. Poseen dimensiones lo suficientemente grandes como para que los efectos de superficie sean despreciables y se asume que no están bajo la influencia significativa de campos eléctricos, magnéticos o gravitacionales externos.

**Postulado:** Para un sistema simple de un solo componente, el conjunto natural de variables independientes que definen el estado en la representación de la energía interna ($U$) está constituido por la entropía ($S$), el volumen ($V$) y el número de partículas ($N$).

### Relación Fundamental de Gibbs

La primera ley de la termodinámica se expresa en forma diferencial como:

$$
dU = d'Q + d'W.
$$

Si consideramos que el trabajo mecánico está definido por $d'W = -P dV$ y el trabajo químico por $d'Z = \mu dN$, la expresión se convierte en:

$$
dU = d'Q - P dV + \mu dN.
$$

Por otro lado, a partir de la definición de entropía para un proceso infinitesimal reversible, el calor transferido es:

$$
d'Q = T dS.
$$

Finalmente, al combinar estas relaciones, obtenemos la expresión para un cambio infinitesimal reversible:

$$
dU = T dS - P dV + \mu dN
$$

Esta ecuación se denomina Relación Fundamental de Gibbs. Por construcción, constituye una síntesis de la primera y la segunda ley de la termodinámica aplicada a procesos reversibles.

### Ecuación Fundamental

En la representación de la energía interna para un sistema simple monocomponente, la ecuación fundamental se escribe como una función de sus variables naturales:

$$
U = U(S, V, N).
$$

### Ecuaciones de Estado

Al realizar la diferencial total de la ecuación fundamental se obtiene:

$$
dU = \left(\frac{\partial U}{\partial S}\right)_{V, N} d S + \left(\frac{\partial U}{\partial V}\right)_{S, N} d V + \left(\frac{\partial U}{\partial N}\right)_{S, V} d N.
$$

Comparando término a término con la relación fundamental de Gibbs, se derivan las ecuaciones de estado del sistema, que vinculan las variables intensivas con las extensivas:

\begin{align*}
T(S, V, N) &= \left(\frac{\partial U}{\partial S}\right)_{V, N},\\
P(S, V, N) &= -\left(\frac{\partial U}{\partial V}\right)_{S, N},\\
\mu(S, V, N) &= \left(\frac{\partial U}{\partial N}\right)_{S, V}.
\end{align*}

## Representación de la Entropía

En la termodinámica, es posible transitar hacia un conjunto distinto de variables independientes sin que se produzca una pérdida de información en el proceso. Al despejar el diferencial de entropía $dS$ de la relación de Gibbs (originalmente expresada en la representación de la energía interna), obtenemos la relación de Gibbs en la representación de la entropía:

$$
d S = \frac{1}{T} d U + \frac{P}{T} d V - \frac{\mu}{T} d N.
$$

Bajo este esquema, es posible recuperar todas las ecuaciones de estado del sistema si seleccionamos a $U$, $V$ y $N$ como las variables independientes fundamentales. En esta representación, la ecuación fundamental se escribe como:

$$
S = S(U, V, N).
$$

A partir de la expresión anterior, el diferencial total de la entropía se define como:

$$
d S = \left(\frac{\partial S}{\partial U}\right)_{V, N} d U + \left(\frac{\partial S}{\partial V}\right)_{U, N} d V + \left(\frac{\partial S}{\partial N}\right)_{U, V} d N.
$$

Al comparar este diferencial término a término con la relación de Gibbs para la entropía, derivamos las siguientes ecuaciones de estado:

\begin{align*}
\frac{1}{T(U, V, N)} &= \left(\frac{\partial S}{\partial U}\right)_{V, N},\\
\frac{P(U, V, N)}{T(U, V, N)} &= \left(\frac{\partial S}{\partial V}\right)_{U, N},\\
\frac{\mu(U, V, N)}{T(U, V, N)} &= -\left(\frac{\partial S}{\partial N}\right)_{U, V}.
\end{align*}

A esta descripción del sistema se le conoce formalmente como la representación de la entropía.

## Interdependencia de las Ecuaciones de Estado

Para sistemas simples de un solo componente, es factible seleccionar cualquier tríada de cantidades extensivas como variables independientes. Para ello, basta con despejar la variable deseada de la relación de Gibbs y de la ecuación fundamental; las cantidades intensivas asociadas se obtienen directamente de las ecuaciones de estado resultantes. Aunque también es posible emplear variables intensivas como variables independientes, dicho procedimiento se formalizará más adelante mediante la introducción de los potenciales termodinámicos.

A fin de ilustrar la interdependencia entre estas ecuaciones, supongamos que elegimos el conjunto $(T, V, N)$ como variables independientes. Bajo esta elección, la energía interna puede expresarse como:

$$
U = U(T, V, N).
$$

En sistemas donde el número de partículas $N$ permanece constante, podemos simplificar la dependencia y diferenciar la función:

$$
d U = \left(\frac{\partial U}{\partial T}\right)_{V} d T + \left(\frac{\partial U}{\partial V}\right)_{T} d V.
$$

Sustituyendo esta expresión en la relación de Gibbs en su representación de entropía ($d S = \frac{1}{T} d U + \frac{P}{T} d V - \frac{\mu}{T} d N$) y considerando que el término en $dN$ se anula por la restricción $N = \text{cte}$, obtenemos:

$$
d S = \frac{1}{T}\left(\frac{\partial U}{\partial T}\right)_{V} d T + \frac{1}{T}\left\{ \left(\frac{\partial U}{\partial V}\right)_{T} + P \right\} d V.
$$

Dado que la entropía $S$ es una función de estado, su diferencial $dS$ es necesariamente una diferencial exacta. Aplicando el criterio de Euler para la igualdad de las derivadas cruzadas:

$$
\left(\frac{\partial}{\partial V}\right)_{T} \left[ \frac{1}{T} \left(\frac{\partial U}{\partial T}\right)_{V} \right] = \left(\frac{\partial}{\partial T}\right)_{V} \left[ \frac{1}{T} \left(\frac{\partial U}{\partial V}\right)_{T} + \frac{P}{T} \right].
$$

Al desarrollar las derivadas en ambos miembros de la ecuación y simplificar los términos resultantes, llegamos a la siguiente relación:

$$
\left(\frac{\partial U}{\partial V}\right)_{T} = T \left(\frac{\partial P}{\partial T}\right)_{V} - P.
$$

Como ejemplo de aplicación, si sustituimos la ecuación de estado del gas ideal ($P = \frac{NkT}{V}$) en el lado derecho de la ecuación anterior, obtenemos:

$$
\left(\frac{\partial U}{\partial V}\right)_{T} = T \left( \frac{Nk}{V} \right) - P = P - P = 0
$$

Este resultado demuestra que, para un gas ideal, la energía interna $U$ depende exclusivamente de la temperatura ($U = U(T)$), lo cual confirma de manera analítica que las ecuaciones de estado no son independientes entre sí, sino que están vinculadas por la estructura matemática de la termodinámica.

## Principios Extremales y Potenciales Termodinámicos

### El Principio de Máxima Entropía

La segunda ley de la termodinámica establece la siguiente restricción para cualquier proceso:

$$
\int_{A}^{B} \frac{d Q}{T} \leq S(B)-S(A).
$$

En el caso particular de un sistema aislado (donde $d Q=0$), se deduce que:

$$
\Delta S = S(B) - S(A) \geq 0.
$$

Asimismo, para un sistema simple de un solo componente en el que se fijan las variables independientes de la representación entrópica ($d U=d V=d N=0$), la primera ley dicta que:

$$
d Q = d U + P d V - \mu d N = 0.
$$

En consecuencia, cuando en un sistema simple se mantienen constantes $U, V$ y $N$, cualquier proceso interno tenderá invariablemente a incrementar su entropía.

### El equilibrio como Estado Extremal

Dado que un sistema simple monocomponente posee únicamente tres grados de libertad termodinámicos, la fijación de los valores de $U, V$ y $N$ determina un único estado de equilibrio global. No obstante, es posible concebir una infinidad de estados termodinámicos en equilibrio local mediante la imposición de restricciones internas (como paredes adiabáticas o rígidas).

Al liberarse estas restricciones internas, el sistema relaja hacia el único estado de equilibrio determinado por las restricciones externas. Como este proceso es irreversible y ocurre sin transferencia de calor, la entropía alcanza su valor más alto posible.

**Principio de Máxima Entropía:** De todos los estados termodinámicos compatibles con las restricciones externas ($U, V, N$), el estado de equilibrio es aquel que posee la máxima entropía.

### Principio de Mínima Energía Interna

En la representación de la energía interna, la segunda ley toma la forma de un principio de minimización.

**Postulado:** Cuando se fijan las variables $S, V$ y $N$, el estado de equilibrio del sistema es, de entre todos los estados compatibles, aquel que minimiza la energía interna.

**Demostración (por Reducción al Absurdo):** Supongamos la existencia de un estado fuera del equilibrio con energía $U_{no-eq} < U_{eq}$ para una misma entropía $S$.

1. Consideremos el estado inicial $E_1 = (U_{no-eq}, S, V, N)$.
2. Suministramos energía al sistema en forma de calor hasta que su energía alcance el valor $U_{eq}$.
3. Puesto que $dS = dQ/T$ y hemos añadido calor, la nueva entropía $S_{final}$ será estrictamente mayor que $S$.
4. El sistema resultante $E_2 = (U_{eq}, S_{final}, V, N)$ presenta una entropía $S_{final} > S_{eq}$.
5. Esto contradice el principio de máxima entropía (que dicta que $S_{eq}$ es el valor máximo para esa $U$).

Por lo tanto, el estado de equilibrio debe ser aquel que **minimiza la energía interna** para una entropía constante.

## Transformaciones de Legendre

Para transitar de variables extensivas (como $S$ o $V$) a variables intensivas (como $T$ o $P$) sin perder la información contenida en la ecuación fundamental, recurrimos a las transformaciones de Legendre.

Geométricamente, una curva $y = y(x)$ puede representarse de dos formas:

1. Como el conjunto de puntos $(x, y)$.
2. Como la envolvente de una familia de rectas tangentes.

La pendiente $P$ y la ordenada al origen $\psi$ de la recta tangente en el punto $(x,y)$ están relacionadas mediante la siguiente expression:
$$
\psi = y - Px .
$$
Si $x$ y $y$ se escriben cono funciones de $P$, obtenemos una transformación que permite que la pendiente actúe como la nueva variable independiente, preservando la capacidad de reconstruir la función original.

## Potenciales Termodinámicos

Utilizando el formalismo de Legendre, definimos los potenciales que actúan como funciones de estado fundamentales para distintos conjuntos de variables.

### Energía Libre de Helmholtz ($F$)

Es el potencial natural cuando se controla la temperatura y el volumen.

* **Definición:** \$F = U - TS. \$
* **Relación de Gibbs:** $d F = -S d T - P d V + \mu d N.$
* **Ecuaciones de Estado:**

$$
S = -\left(\frac{\partial F}{\partial T}\right)_{V, N} ; \quad P = -\left(\frac{\partial F}{\partial V}\right)_{T, N} ; \quad \mu = \left(\frac{\partial F}{\partial N}\right)_{T, V}.
$$


### Energía Libre de Gibbs ($G$)

Es el potencial fundamental en procesos a presión y temperatura constantes (típico en química).

* **Definición:** $G = U - TS + PV = F + PV.$
* **Relación de Gibbs:** $d G = -S d T + V d P + \mu d N.$
* **Ecuaciones de Estado:**

$$
S = -\left(\frac{\partial G}{\partial T}\right)_{P, N} ; \quad V = \left(\frac{\partial G}{\partial P}\right)_{T, N} ; \quad \mu = \left(\frac{\partial G}{\partial N}\right)_{T, P}.
$$


### Entalpía ($H$)

Es útil en sistemas donde la presión y la entropía son las variables naturales.

* **Definición:** $H = U + PV.$
* **Relación de Gibbs:** $d H = T d S + V d P + \mu d N.$
* **Ecuaciones de Estado:**

$$
T = \left(\frac{\partial H}{\partial S}\right)_{P, N} ; \quad V = \left(\frac{\partial H}{\partial P}\right)_{S, N} ; \quad \mu = \left(\frac{\partial H}{\partial N}\right)_{S, P}.
$$


## Principios Extremales: Segunda Ley y Representaciones Termodinámicas

### Energía Libre de Helmholtz

Consideremos un sistema con volumen $V$ y número de partículas $N$ constantes, en contacto térmico con una fuente (reservorio) a temperatura $T_{f}$. El sistema compuesto (sistema más fuente) posee un volumen total $V+V_{f}$ y un número de partículas $N+N_{f}$ invariantes, dado que estas magnitudes son constantes en cada subsistema.

Por otro lado, aunque la entropía de los subsistemas varía debido al intercambio continuo de calor, todo el calor cedido por la fuente es absorbido por el sistema (y viceversa). En consecuencia, la entropía del sistema compuesto $S+S_{f}$ permanece constante.

Dado que la entropía, el volumen y el número de partículas del sistema compuesto están fijos, su estado de equilibrio puede estudiarse mediante la representación de la energía interna. El equilibrio obedece al principio de mínima energía interna, expresado como

$$
d(U+U_{f})=0, \quad
d^{2}(U+U_{f})>0, 
$$ (eq:01)

sujeto a la restricción

$$
d(S+S_{f})=0 .
$$

De la ecuación {eq}`eq:01` se deduce que $dU + dU_{f} = 0$. Asumiendo que la energía interna de la fuente térmica solo cambia mediante el intercambio de calor, tenemos:

$$
d U_{f}=T_{f} d S_{f}. 
$$

Combinando estas expresiones, y considerando que $dS_f = -dS$ por la restricción de entropía constante, obtenemos:

$$
0 = d U - T_{f} d S = d(U - T_{f} S).
$$

Si nos restringimos a estados donde la temperatura del sistema iguala a la de la fuente ($T = T_{f}$), llegamos a $dF = 0$. Al analizar la diferencial de segundo orden:

$$
d^{2} F = d^{2}(U - T_{f} S) = d^{2}(U + U_{f}) > 0
$$

De lo anterior demuestra el **Principio de Mínima Energía Libre de Helmholtz:** Para un sistema con volumen y número de partículas constantes en contacto con una fuente térmica, el estado de equilibrio es aquel que, de todos los estados termodinámicos posibles, minimiza la energía libre de Helmholtz ($F = U - TS$).

De manera análoga se puede demostrar el **Principio de Mínima Energía Libre de Gibbs:** Para un sistema con número de partículas constantes en contacto con una fuente térmica y una fuente de presión, el estado de equilibrio es aquel que, de todos los estados termodinámicos posibles, minimiza la energía libre de Gibbs ($F = U - TS + PV$).

## Interpretación Física de los Potenciales

### Energía Libre de Helmholtz y Trabajo Mecánico

Consideremos un sistema con $N$ constante en contacto con una fuente a temperatura $T$. Según la segunda ley, en un proceso entre los estados $A$ y $B$:

$$
\int_{A}^{B} \frac{d Q}{T} \leq S(B)-S(A). 
$$

Como la temperatura de la fuente es constante, $Q \leq T[S(B)-S(A)]$. De la primera ley ($Q = \Delta U + W_{\mathrm{mec}}$), sustituyendo obtenemos:

$$
L_{\mathrm{mec}} \leq -[F(B)-F(A)]. 
$$

Esta desigualdad demuestra que el trabajo mecánico máximo obtenible de un sistema a temperatura constante, $L_{\mathrm{mec}}$, está acotado por la disminución de su energía libre de Helmholtz. Si el volumen es constante ($dV = 0$), entonces $\Delta F \leq 0$.

### Energía Libre de Gibbs y Trabajo Químico

Para un sistema en equilibrio con fuentes de temperatura ($T$) y presión ($P$) constantes, la primera ley establece:

$$
Q = \Delta U + P \Delta V + L_{\mathrm{quim}}, 
$$

donde $L_{\mathrm{quim}} = -\int \mu dN$ es el trabajo químico desarrollado por el sistema. Combinando con la segunda ley ($Q \leq T \Delta S$):

$$
L_{\mathrm{quim}} \leq -\Delta G = -[G(B)-G(A)].
$$

Por lo tanto, el trabajo químico máximo extraíble a $T$ y $P$ constantes está acotado por la disminución de la energía libre de Gibbs. Si $N$ es constante ($L_{\text{quim}} = 0$), entonces $\Delta G \leq 0$ para cualquier proceso espontáneo.

### Entalpía y Calor Isobárico

La entalpía se define como $H = U + PV$. Para un sistema con número de partículas fijo en contacto con una fuente de presión constante ($dP = 0$):

$$
d H = d U + P d V = d Q.
$$

En consecuencia, el cambio de entalpía mide directamente el calor intercambiado en un proceso isobárico. Esto define la capacidad calorífica a presión constante:

$$
C_{P} = \left(\frac{\partial H}{\partial T}\right)_{P}.
$$

