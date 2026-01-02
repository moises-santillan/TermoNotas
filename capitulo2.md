# Capítulo 2: Física Estadística Clásica

## Conceptos Fundamentales

**Sistema Termodinámico:** Se define como un sistema dinámico (mecánico en este contexto) cuyo número de grados de libertad es del orden del número de Avogadro ($N_A \approx 10^{23}$). Esta escala masiva es la que permite la emergencia de leyes estadísticas a partir del comportamiento individual de sus constituyentes.

**Estado Macroscópico (Macroestado):** El macroestado de un sistema es sinónimo de su estado de equilibrio. En un sistema con $n$ grados de libertad termodinámicos, el macroestado queda unívocamente determinado por el valor de sus $n$ variables independientes. Para los fines de esta sección, utilizaremos la representación de la entropía, donde el conjunto de variables independientes es $(U, V, N_{i})$.

**Estado Microscópico (Microestado):** Representa la configuración detallada y puntual de todas las partículas del sistema. Para un sistema con $f$ grados de libertad dinámicos ($f \approx 10^{23}$), el microestado está determinado por el valor instantáneo de las $f$ coordenadas generalizadas y los $f$ momentos generalizados.

**Espacio de Fase Termodinámico:** Es un espacio cartesiano de $n$ dimensiones, donde cada eje corresponde a una de las variables termodinámicas independientes. Por construcción, el estado macroscópico de un sistema se representa mediante un único punto en este espacio, simplificando la vasta complejidad interna en unos pocos parámetros globales.

**Espacio de Fase Dinámico o Espacio $\Gamma$:** Para un sistema con $f$ grados de libertad dinámicos, el espacio $\Gamma$ es un espacio cartesiano de $2f$ dimensiones ($f$ posiciones y $f$ momentos). En cualquier instante, el estado microscópico completo se representa mediante un punto en el espacio $\Gamma$. La evolución del sistema en el tiempo traza una trayectoria continua dentro de este espacio.

**Ensemble Termodinámico:** Es una construcción mental que consiste en un conjunto de sistemas dinámicos que obedecen al mismo Hamiltoniano microscópico y cuyos macroestados son idénticos. Aunque todos los sistemas del ensamble comparten las mismas variables externas (como $U, V, N$), sus microestados son, en general, distintos y evolucionan de forma independiente.

## Microestados, Macroestados y Mesoestados 

### Representación de un Macroestado en el espacio $\Gamma$

En un macroestado de equilibrio, los valores de las variables termodinámicas permanecen constantes en el tiempo. Sin embargo, a nivel microscópico, el sistema es dinámico y su configuración cambia continuamente. Esto implica que, para un único macroestado, existe una vasta cantidad de microestados compatibles, los cuales están determinados estrictamente por las restricciones macroscópicas.

Geométricamente, el conjunto de todos los microestados compatibles con un macroestado dado define una región en el espacio $\Gamma$, que denominaremos **región $\Omega$**. El tamaño y la topología de $\Omega$ dependen de las restricciones externas. Así, mientras que el **microestado** se representa como un punto exacto en el espacio de fase (requiriendo conocer $2f \approx 10^{23}$ variables), el **macroestado** es una descripción "gruesa" que define simplemente el volumen $\Omega$ donde dicho punto debe residir, utilizando un conjunto mínimo de variables (del orden de $10^1$), como $U, V$ y $N_i$.

### Representación del Microestado de un Ensemble en $\Gamma$

Para determinar el microestado de un ensemble de tamaño $N^*$, es necesario especificar el microestado individual de cada uno de los sistemas que lo integran. Esto implica conocer los valores de $2 N^* f$ variables. Dado que para un sistema termodinámico $f \approx 10^{23}$, la cantidad de información necesaria es colosal. En el espacio $\Gamma$, el microestado del ensemble se representa mediante una "nube" de $N^*$ puntos representativos, cada uno correspondiente a la configuración instantánea de un sistema del colectivo.

### Representación del Macroestado de un Ensemble en $\Gamma$

Puesto que todos los sistemas que componen el ensemble son macroscópicamente idénticos, su macroestado queda definido por el número total de sistemas ($N^*$) y las variables termodinámicas comunes ($U, V, N_i$). Por tanto, la región $\Omega$ que representa el macroestado de un sistema individual también representa el macroestado del ensemble completo. La diferencia radica en la densidad de ocupación: en esta descripción, simplemente establecemos que los $N^*$ puntos representativos deben encontrarse contenidos dentro de la región $\Omega$.

Mientras que el microestado del ensemble ofrece la descripción más exhaustiva (la posición exacta de cada punto), el macroestado proporciona una caracterización simplificada que solo delimita el espacio permitido para dichos puntos.

### Estado Mesoscópico o Mesoestado

La conexión entre las descripciones micro y macroscópica se construye estadísticamente a través del estado mesoscópico o mesoestado. Para definirlo, se divide la región $\Omega$ en $r$ celdas o elementos de volumen de fase. Para que este estado sea efectivamente una escala intermedia, el número de celdas debe cumplir la condición $1 \ll r \ll f$. Asimismo, se asume que cada celda posee un volumen de fase equivalente ($\omega_i \approx \omega_j$).

El mesoestado queda definido por el conjunto de números de ocupación $\{n_i^*\}$, donde cada $n_i^*$ indica cuántos puntos representativos del ensemble se encuentran en la $i$-ésima celda. Estos valores deben satisfacer la condición de conservación:

$$\sum_{i=1}^{r} n_i^* = N^*.$$

La descripción mesoscópica es un punto medio en todos los sentidos:
1.  **Precisión:** Es más detallada que la macroscópica (especifica la distribución dentro de $\Omega$), pero no alcanza la resolución microscópica (ignora la posición exacta dentro de cada celda).
2.  **Información:** El número de variables requeridas ($r$ números de ocupación más las variables macroscópicas) es mucho mayor que el del macroestado, pero drásticamente menor que las $2N^*f$ variables del microestado. 

Esta escala intermedia permite aplicar herramientas combinatorias para encontrar el mesoestado más probable, el cual corresponderá, en el límite termodinámico, al estado de equilibrio macroscópico.

## Conexión entre las Descripciones Micro y Macroscópicas

### Hipótesis de Igualdad de Probabilidad a Priori

Este es el pilar fundamental de la mecánica estadística clásica. La hipótesis establece que, para un sistema en equilibrio, todos los estados microscópicos compatibles con las restricciones macroscópicas son igualmente probables. Es importante subrayar que este enunciado no se deriva de principios dinámicos elementales, sino que es un postulado cuya validez se justifica mediante la comprobación experimental de las predicciones termodinámicas resultantes.

### Probabilidad de un Mesoestado

Dado que la descripción macroscópica solo delimita la región $\Omega$ del espacio de fase sin especificar la ubicación exacta de los microestados, cualquier configuración de números de ocupación $\{n_i^*\}$ que cumpla con la restricción de conservación $\sum_{i} n_{i}^* = N^*$ representa un mesoestado físicamente admisible. 

Bajo la hipótesis de igualdad de probabilidad a priori, la probabilidad de encontrar al ensemble en un mesoestado particular es directamente proporcional al número de microestados que lo conforman. Este número, denominado peso estadístico o multiplicidad del mesoestado, se calcula mediante la expresión:

$$W(\{n_i^*\}) = \frac{N^*!}{n_1^*! n_2^*! \ldots n_r^*!} \omega_1^{n_1^*} \omega_2^{n_2^*} \ldots \omega_r^{n_r^*}$$

### Definición Estadística de la Entropía

A medida que el microestado del sistema evoluciona en el espacio $\Gamma$, el sistema transita entre distintos mesoestados. Sea $\{\tilde{n}_i^*\}$ el conjunto de números de ocupación que define este mesoestado más probable.

En el límite termodinámico, el mesoestado más probable es el que caracteriza las propiedades del macroestado de equilibrio. Por otro lado, la Segunda Ley de la Termodinámica establece que un sistema aislado en equilibrio alcanza un estado de entropía máxima. Esta coincidencia sugiere una relación funcional entre la probabilidad y la entropía. 

Dado que la probabilidad es multiplicativa y la entropía es aditiva, la única relación funcional consistente es la logarítmica. De este razonamiento se deriva la expresión para la entropía del estado de equilibrio del ensemble ($S^*$):

$$S^* = k \ln \left[ \frac{N^*!}{\tilde{n}_1^*! \tilde{n}_2^*! \ldots \tilde{n}_r^*!} \omega_1^{\tilde{n}_1^*} \omega_2^{\tilde{n}_2^*} \ldots \omega_r^{\tilde{n}_r^*} \right],$$ (entro)

donde $k$ es la constante de Boltzmann, la constante universal que vincula la información estadística con las unidades térmicas (J/K). Esta relación constituye el puente definitivo entre el caos microscópico y el orden macroscópico.

## La Entropía de Gibbs

### Entropía de Cada Sistema del Ensemble

La expresión para la entropía del ensemble permite calcular el valor correspondiente a un único sistema ($S$). Dado que todos los sistemas del ensemble son macroscópicamente idénticos y la entropía es una propiedad aditiva, tenemos:

$$S = \frac{S^*}{N^*} = \frac{k}{N^*} \ln \left[ \frac{N^*!}{\tilde{n}_1^*! \tilde{n}_2^*! \ldots \tilde{n}_r^*!} \omega_1^{\tilde{n}_1^*} \omega_2^{\tilde{n}_2^*} \ldots \omega_r^{\tilde{n}_r^*} \right].$$

Al aplicar la **aproximación de Stirling** ($\ln N! \approx N \ln N - N$) y las leyes de los logaritmos, bajo la condición $\sum_{i} \tilde{n}_{i}^* = N^*$, la ecuación se reduce a:

$$S = -k \sum_{i} p_i \ln(p_i) \omega_i.$$ 

Aquí, $p_i = \frac{\tilde{n}_i^*}{N^* \omega_i}$ representa la **densidad de probabilidad** de encontrar el punto representativo del sistema en la $i$-ésima celda. Esta cantidad cumple con la normalización $\sum_{i} p_i \omega_i = 1$.

### El Límite al Continuo

Para evitar que el valor de la entropía dependa de la discretización arbitraria del espacio de fase, tomamos el límite al continuo considerando un volumen de fase infinitesimal $d\gamma$. En este límite, la sumatoria converge a una integral sobre la región $\Omega$:

$$S = -k \int_{\Omega} \rho(x) \ln \rho(x) \, d\gamma,$$ (eq:03)

Donde $\rho(x)$ es la función de densidad de probabilidad en el espacio $\Gamma$, la cual está normalizada:

$$\int_{\Omega} \rho(x) \, d\gamma = 1.$$ (eq:04)

La definición de entropía dada por la ecuación {eq}`eq:03` se conoce como la entropía de Gibbs.

## Ensembles Microcanónico y Canónico

La definición de entropía presentada en la ecuación {eq}`eq:03` permite determinar la entropía de un macroestado a partir de la densidad de probabilidad $\rho(x)$ que define al mesoestado más probable. No obstante, en la práctica, esta expresión es difícil de aplicar directamente, ya que rara vez se conoce la forma funcional de $\rho(x)$ mediante resultados experimentales. Afortunadamente, la segunda ley de la termodinámica proporciona el criterio necesario para deducir este mesoestado a partir de las restricciones macroscópicas impuestas al ensemble.

En la representación de la entropía, la segunda ley establece que el estado de equilibrio de un sistema aislado es aquel que, de entre todos los estados compatibles con sus restricciones, maximiza la entropía. Si equiparamos los mesoestados (definidos por cada función de distribución que satisfaga la normalización) con los estados termodinámicos, el problema se reduce a un ejercicio de optimización: debemos hallar la función $\rho(x)$ que maximice la ecuación {eq}`eq:03`, sujeta a la condición de normalización {eq}`eq:04` y a las ligaduras físicas que garanticen que el ensemble representa a un sistema aislado.

### Ensemble Microcanónico

Por definición, el ensemble microcanónico está constituido por un colectivo de sistemas en equilibrio, delimitados por paredes rígidas, adiabáticas e impermeables; es decir, sistemas estrictamente aislados. En consecuencia, todos los sistemas que conforman este ensemble poseen valores constantes e idénticos de energía interna ($U$), volumen ($V$) y número de partículas ($N_i$).

Bajo estas condiciones de aislamiento, no se requieren restricciones energéticas adicionales más allá de la condición de normalización {eq}`eq:04`. Por tanto, la densidad de probabilidad de equilibrio será aquella que maximice la entropía de Gibbs {eq}`eq:03` sujeta a {eq}`eq:04`. Este problema se resuelve elegantemente mediante el cálculo variacional y el método de los multiplicadores de Lagrange. Para ello, definimos el funcional Lagrangiano:

$$
\Lambda = \int_{\Omega} [\rho(x) \ln \rho(x) - \alpha \rho(x)] d\gamma,
$$

donde $\alpha$ es un multiplicador de Lagrange asociado a la restricción de normalización. De acuerdo con la teoría variacional, la función $\rho(x)$ óptima es aquella que anula la variación de $\Lambda$:

$$
\delta \Lambda = \int_{\Omega} [\ln \rho(x) + 1 - \alpha] \delta \rho(x) d\gamma = 0.
$$

Dado que la variación $\delta \rho(x)$ es arbitraria, la única forma de garantizar que la integral se anule es que el término entre corchetes sea igual a cero en toda la región:

$$
\ln \rho(x) + 1 - \alpha = 0.
$$

Al despejar $\rho(x)$, obtenemos la densidad de probabilidad para el ensemble microcanónico:

$$
\rho(x) = C,
$$

donde $C = \exp(\alpha - 1)$ es una constante de proporcionalidad. El valor de esta constante se determina imponiendo la condición de normalización {eq}`eq:04`, lo que nos conduce a la densidad de probabilidad de equilibrio final:

$$
\rho(x) = \frac{1}{\Gamma}.
$$ (eq:05)

En esta expresión, $\Gamma = \int_{\Omega} d\gamma$ representa el volumen de fase total de la región $\Omega$. Es fundamental notar que el tamaño y la geometría de esta región están unívocamente determinados por las condiciones macroscópicas impuestas: $\Gamma = \Gamma(U, V, N_i)$.

Finalmente, al sustituir la densidad de probabilidad constante {eq}`eq:05` en la definición de entropía {eq}`eq:03`, obtenemos la ecuación fundamental para cada uno de los sistemas del ensemble microcanónico:

$$
S(U, V, N_i) = k \ln \Gamma(U, V, N_i).
$$ (eq:06)

Esta relación constituye el puente definitivo entre la extensión geométrica del sistema en el espacio de fase ($\Gamma$) y su propiedad termodinámica fundamental ($S$).

### Ensemble Canónico

El ensemble canónico está constituido por un colectivo de sistemas que mantienen valores constantes e idénticos de volumen ($V$) y número de partículas ($N_i$). A diferencia del microcanónico, los sistemas de este ensemble se encuentran en contacto térmico y en equilibrio con una fuente de calor a una temperatura $T$. Si bien cada sistema individual es termodinámicamente cerrado, no está aislado, ya que intercambia energía con el reservorio.

Para tratar al ensemble como un sistema aislado en su totalidad, consideramos que el reservorio térmico es el propio ensemble: cada sistema individual interactúa térmicamente con el resto de los sistemas del colectivo. Esta restricción sobre la energía media del sistema se expresa como:

$$
\int_{\Omega} \epsilon(x) \rho(x) d\gamma = \bar{\epsilon},
$$ (eq:07)

donde $\epsilon(x)$ es la energía del sistema en el punto $x$ del espacio de fase y $\bar{\epsilon}$ representa la energía promedio del ensemble.

Siguiendo la segunda ley de la termodinámica, la densidad de probabilidad de equilibrio $\rho(x)$ es aquella que maximiza la entropía {eq}`eq:03`, sujeta a la normalización {eq}`eq:04` y a la conservación de la energía media {eq}`eq:07`. Aplicando el cálculo variacional, definimos el funcional Lagrangiano $\Lambda$ como:

$$
\Lambda = \int_{\Omega} [\rho(x) \ln \rho(x) - (\alpha - 1 - \beta \epsilon(x)) \rho(x)] d\gamma,
$$

donde $\alpha$ y $\beta$ son multiplicadores de Lagrange. La variación de este funcional es:

$$
\delta \Lambda = \int_{\Omega} [\ln \rho(x) + 1 - (\alpha - 1) + \beta \epsilon(x)] \delta \rho(x) d\gamma.
$$

Para que $\delta \Lambda = 0$ ante una variación arbitraria $\delta \rho(x)$, el integrando debe anularse. Al despejar $\rho(x)$, obtenemos la distribución canónica:

$$
\rho(x) = \frac{1}{Z} e^{-\beta \epsilon(x)}.
$$ (eq:08)

La función de partición, $Z$, se determina mediante la condición de normalización {eq}`eq:04`:

$$
Z = \int_{\Omega} e^{-\beta \epsilon(x)} d\gamma.
$$ (eq:09)

Al sustituir la densidad de probabilidad {eq}`eq:08` en la definición de entropía {eq}`eq:03`, obtenemos:

$$
S = k \beta \bar{\epsilon} + k \ln Z.
$$ (eq:10)

Imponiendo la relación termodinámica $1/T = (\partial S / \partial \bar{\epsilon})_{V, N_i}$, identificamos que:

$$
\beta = \frac{1}{kT}.
$$ (eq:11)

Puesto que las variables independientes son $(T, V, N_i)$, la ecuación fundamental se obtiene a partir de la energía libre de Helmholtz ($F$):

$$
F(T, V, N_i) = -kT \ln Z(T, V, N_i).
$$ (eq:12)

## Física Estadística del Gas Ideal

### Ensemble Canónico

Por definición, un gas ideal es un sistema compuesto por partículas que no interactúan entre sí (fuerzas intermoleculares nulas) y cuya energía total es puramente cinética. Por lo tanto, para un gas de $N$ partículas, el Hamiltoniano se expresa como la suma de los cuadrados de los momentos:

$$
H = \sum_{i=1}^{3N} \frac{p_{i}^{2}}{2m}.
$$

Consideremos este gas contenido en un recipiente de volumen $V$. Su función de partición canónica se calcula integrando sobre todo el espacio de fase:

\begin{align*}
Z = & \int_{0}^{V^{1/3}} \dots \int_{0}^{V^{1/3}} dx_{1} \dots dx_{3N} \\
& \int_{-\infty}^{\infty} \dots \int_{-\infty}^{\infty} e^{-\frac{\beta}{2m}(p_{1}^{2} + \dots + p_{3N}^{2})} dp_{1} \dots dp_{3N}.
\end{align*}

Los límites de integración para los momentos $p_i$ se extienden de $-\infty$ a $\infty$ debido a que el sistema está en contacto con una fuente térmica; esto permite fluctuaciones de energía que, aunque estadísticamente improbables en magnitudes extremas, son matemáticamente posibles. 

La integral sobre las coordenadas espaciales $x_i$ se simplifica a $V^N$. Por su parte, la integral de los momentos se descompone en $3N$ integrales gaussianas independientes de la forma $\int_{-\infty}^{\infty} e^{-\frac{\beta p^2}{2m}} dp = \sqrt{\frac{2\pi m}{\beta}}$. Combinando estos resultados, obtenemos la función de partición del gas ideal:

$$
Z = \left[ V (2 \pi m k T)^{3/2} \right]^{N}.
$$ (eq:13)

A partir de esta función, derivamos la energía libre de Helmholtz ($F$), que constituye la ecuación fundamental del sistema:

\begin{align*}
F(T, V, N) &= -k T \ln Z \\
&= -k T N \left[ \ln V + \frac{3}{2} \ln (2 \pi m k T) \right].
\end{align*} (eq:14)

De esta ecuación fundamental emanan las siguientes ecuaciones de estado mediante diferenciación parcial:

```{math}
:label: eq:15
\begin{align*}
S &= -\left( \frac{\partial F}{\partial T} \right)_{V, N} = -\frac{F}{T} + \frac{3}{2} N k. \\
P &= -\left( \frac{\partial F}{\partial V} \right)_{T, N} = \frac{N k T}{V}. \\
\mu &= \left( \frac{\partial F}{\partial N} \right)_{T, V} = -k T \left[ \ln V + \frac{3}{2} \ln (2 \pi m k T) \right].
\end{align*}
```

La primera expresión en {eq}`eq:15` representa la ecuación de estado térmica del gas ideal. Asimismo, a partir de la segunda expresión y de la definición de la energía libre de Helmholtz ($F = \bar{\epsilon} - TS$), es posible derivar la energía interna promedio del sistema:

$$
\bar{\epsilon} = F + TS = \frac{3}{2} N k T. 
$$

Esta relación constituye la ecuación de estado energética del gas ideal. Cabe señalar que la tercera expresión en {eq}`eq:15` no coincide aún con la ecuación de estado correspondiente al potencial químico del sistema; no obstante, las causas de esta discrepancia serán analizadas detalladamente más adelante.

En conclusión, el formalismo del ensemble canónico ha permitido recuperar con éxito las leyes fundamentales del gas ideal. Este resultado valida empíricamente las premisas teóricas sobre las que se fundamenta esta disciplina, en particular la hipótesis de igual probabilidad a priori y la definición estadística de la entropía de Gibbs.

### Ensemble Microcanónico

Consideremos un gas de $N$ partículas contenido en un recipiente de volumen fijo $V$, delimitado por paredes adiabáticas e impermeables. Bajo estas condiciones de aislamiento, la energía interna del sistema se mantiene constante dentro de un intervalo infinitesimal $[E - \delta E, E]$, donde $\delta E \ll E$.

El Hamiltoniano de este sistema es puramente cinético:

$$
H = \sum_{i=1}^{3N} \frac{p_{i}^{2}}{2m}.
$$

Esta restricción energética define la geometría de la región $\Omega$ en el espacio de fase. La proyección de $\Omega$ en el espacio de momentos corresponde a un cascarón hiperesférico de $3N$ dimensiones con radio externo $R = \sqrt{2mE}$. Por otro lado, la proyección en el espacio de configuración resulta en un volumen total de $V^N$.

En dimensiones elevadas ($3N \to \infty$), el volumen de una hiperesfera se concentra casi exclusivamente cerca de su superficie, por lo que el volumen del cascarón se aproxima al de la esfera completa. El volumen de una hiperesfera de $f$ dimensiones y radio $R$ es:

$$
V_{f}(R) = \frac{\pi^{f/2}}{(f/2)!} R^{f}.
$$

De aquí se sigue que el volumen de la proyección de $\Omega$ en el espacio de momentos es:

$$
\Phi_p = \frac{(2\pi m E)^{3N/2}}{(3N/2)!}.
$$

Combinando esto con el volumen del espacio de configuración, obtenemos el volumen de fase ($\Gamma$) total de la región $\Omega$:

$$
\Gamma = \frac{V^N (2\pi m E)^{3N/2}}{(3N/2)!}.
$$

Sustituyendo este resultado en la ecuación fundamental del ensemble microcanónico {eq}`eq:06`, obtenemos la entropía del gas ideal:

$$
S = k N \left\{ \ln \left[ V \left( \frac{4\pi m E}{3N} \right)^{3/2} \right] + \frac{3}{2} \right\}. 
$$ (eq:19)

Las ecuaciones de estado derivadas son:

\begin{align*}
\frac{1}{T} &= \frac{3}{2} \frac{kN}{E}, \\
\frac{P}{T} &= \frac{kN}{V}, \\
\frac{\mu}{T} &= -k \left[ \ln V + \frac{3}{2} \ln \left( \frac{4\pi m E}{3N} \right) \right]. 
\end{align*}

Estos resultados son plenamente consistentes con los obtenidos mediante el ensemble canónico en {eq}`eq:15`, validando la equivalencia de ambos enfoques en el límite termodinámico.


## Fluctuaciones Termodinámicas

En el ensemble canónico, el valor promedio de cualquier observable físico $f(x)$ se calcula mediante el promedio estadístico ponderado por la densidad de probabilidad $\rho(x)$ definida en la ecuación {eq}`eq:08`:

$$
\bar{f} = \int_{\Omega} f(x) \rho(x) d\gamma.
$$

Utilizando esta definición y la estructura matemática de la función de partición {eq}`eq:09`, se demuestra que la energía promedio del sistema está vinculada a la primera derivada logarítmica de $Z$ respecto a $\beta$:

$$
\bar{\epsilon} = -\frac{\partial \ln Z}{\partial \beta}.
$$

Asimismo, la varianza de la energía, que representa la magnitud de las fluctuaciones térmicas en torno al promedio, se obtiene a partir de la segunda derivada:

$$
\sigma_{\epsilon}^{2} = \overline{\Delta \epsilon^{2}} = \frac{\partial^{2} \ln Z}{\partial \beta^{2}}.
$$

Dado que $\ln Z$ es una cantidad extensiva (proporcional al número de partículas $N$) y $\beta = (kT)^{-1}$ es una variable intensiva, se concluye que la desviación estándar de la energía escala como $\sqrt{N}$. Por lo tanto, la fluctuación relativa de la energía obedece la relación:

$$
\frac{\sqrt{\overline{\Delta \epsilon^{2}}}}{\bar{\epsilon}} \approx \frac{1}{\sqrt{N}}.
$$ (eq:25)

Esta relación es fundamental en el límite termodinámico ($N \to \infty$): las fluctuaciones relativas se vuelven despreciables, lo que garantiza que las predicciones del ensemble canónico coincidan con las del microcanónico.

## Paradoja de Gibbs y Otros Problemas

Las expresiones obtenidas para el gas ideal en las ecuaciones {eq}`eq:13` y {eq}`eq:19` presentan inconsistencias que requieren una revisión de los postulados puramente clásicos.

### El Problema de las Unidades y el Límite Cuántico
En primer lugar, los argumentos de las funciones logarítmicas en las expresiones clásicas poseen dimensiones físicas de volumen y momento, lo cual es matemáticamente incorrecto (el argumento de un logaritmo debe ser adimensional). El origen de este problema reside en el uso del volumen fase continuo sin una escala de referencia.

La mecánica cuántica resuelve esta inconsistencia mediante el principio de incertidumbre de Heisenberg, el cual sugiere que el espacio de fase está discretizado en celdas de volumen elemental $h^{3N}$ (donde $h$ es la constante de Planck). Al normalizar el volumen de fase por este factor, el conteo de estados se vuelve adimensional y las ecuaciones fundamentales se corrigen como:

\begin{align*}
S(U, V, N) &= k \ln \left( \frac{\Gamma}{h^{3N}} \right) = k N \left\{ \ln \left[ V \left( \frac{4 \pi m E}{3 N h^{2}} \right)^{3/2} \right] + \frac{3}{2} \right\}, \\
F(T, V, N) &= -k T \ln \left( \frac{Z}{h^{3N}} \right) = -k T N \left[ \ln V + \frac{3}{2} \ln \left( \frac{2 \pi m k T}{h^{2}} \right) \right].
\end{align*}

### La Paradoja de Gibbs y la Indistinguibilidad
A pesar de corregir las unidades, las expresiones anteriores aún no son extensivas. Si duplicamos el tamaño del sistema ($V \to 2V, N \to 2N$), la entropía $S$ no se duplica proporcionalmente, lo que contradice las leyes de la termodinámica. Este fenómeno se conoce como la paradoja de Gibbs.

La solución reside en reconocer que las partículas de un gas son indistinguibles. En el conteo clásico, se trata a cada partícula como si fuera única, sobreestimando el número de microestados por un factor de $N!$. Al introducir este factor de corrección cuántico, obtenemos finalmente las ecuaciones fundamentales correctas:

\begin{align*}
S(U, V, N) &= k \ln \left( \frac{\Gamma}{h^{3N} N!} \right) = k N \left\{ \ln \left[ \frac{V}{N} \left( \frac{4 \pi m E}{3 N h^{2}} \right)^{3/2} \right] + \frac{5}{2} \right\}, \\
F(T, V, N) &= -k T \ln \left( \frac{Z}{h^{3N} N!} \right) = -k T N \left[ \ln \frac{V}{N} + \frac{3}{2} \ln \left( \frac{2 \pi m k T}{h^{2}} \right) + 1 \right].
\end{align*}

Con estas correcciones, tanto $S$ como $F$ escalan linealmente con el número de partículas, resolviendo definitivamente las inconsistencias del formalismo.

### Derivación del Potencial Químico Correcto

A partir de la energía libre de Helmholtz corregida, el potencial químico se obtiene como:

$$\mu = \left( \frac{\partial F}{\partial N} \right)_{T, V}.$$

Calculando la derivada y simplificando obtenemos la ecuación de estado correcta para el potencial químico:

$$\mu = -kT \left[ \ln \left( \frac{V}{N} \right) + \frac{3}{2} \ln \left( \frac{2 \pi m kT}{h^2} \right) \right].$$

Esta expresión es físicamente consistente por las siguientes razones:

* **Intensividad:** A diferencia de la versión previa a la corrección de Gibbs, el argumento del logaritmo ahora depende del volumen específico $(v = V/N)$, lo que garantiza que $\mu$ sea una propiedad intensiva (no cambia si duplicamos el tamaño del sistema manteniendo la densidad constante).
* **Adimensionalidad:** Gracias a la introducción de $h^2$, el argumento del logaritmo es adimensional.

Es común en aplicaciones prácticas escribir la expresión anterior como:

$$
\mu = \mu^0 + kT \ln c,
$$

con $c = N/V$ la concentración de moléculas del gas.

## Teorema de Equipartición de la Energía

Consideremos un sistema cuya dinámica está descrita por un Hamiltoniano cuadrático de la forma:

$$
H = K + V = \sum_{i=1}^{f} A_{i} p_{i}^{2} + \sum_{i, j=1}^{f} B_{ij} q_{i} q_{j}.
$$

Donde $f$ representa el número de grados de libertad, $p_{i}$ los momentos generalizados, $q_{i}$ las coordenadas generalizadas, y las constantes $A_{i}$ y $B_{ij}$ son coeficientes arbitrarios. Bajo esta forma, tanto la energía cinética ($K$) como la energía potencial ($V$) son funciones homogéneas de segundo orden respecto a los momentos y las coordenadas, respectivamente. Por el teorema de Euler para funciones homogéneas, se cumplen las siguientes relaciones:

```{math}
:label: eq:28
\begin{align*}
& \sum_{j=1}^{f} p_{j} \frac{\partial K}{\partial p_{j}} = 2 \sum_{j=1}^{f} A_{j} p_{j}^{2} = 2K, \\
& \sum_{j=1}^{f} q_{j} \frac{\partial V}{\partial q_{j}} = 2 \sum_{i, j=1}^{f} B_{ij} q_{i} q_{j} = 2V. 
\end{align*}
```
Para encontrar el valor promedio de estos términos, empleamos el formalismo del ensemble canónico:

$$
\overline{p_{j} \frac{\partial K}{\partial p_{j}}}=\overline{p_{j} \frac{\partial H}{\partial p_{j}}}=\frac{1}{Z} \int e^{-\beta H} p_{j} \frac{\partial H}{\partial p_{j}} d \gamma. 
$$ (eq:30)

La integración se realiza sobre todo el espacio de fase. Si aislamos la integral respecto al momento $p_{j}$ y aplicamos el método de integración por partes, obtenemos:

```{math}
:label: eq:31
\begin{align*}
\int_{-\infty}^{\infty} e^{-\beta H} \left( p_{j} \frac{\partial H}{\partial p_{j}} \right) dp_{j} &= -\frac{1}{\beta} \int_{-\infty}^{\infty} p_{j} \frac{\partial e^{-\beta H}}{\partial p_{j}} dp_{j}, \\
&= -\left[ \frac{p_{j} e^{-\beta H}}{\beta} \right]_{-\infty}^{\infty} + \frac{1}{\beta} \int_{-\infty}^{\infty} e^{-\beta H} dp_{j}. 
\end{align*}
```
Debido a que el Hamiltoniano depende cuadráticamente de $p_{j}$, el término evaluado en los límites se anula, ya que la función exponencial decrece más rápido de lo que crece el término lineal $p_{j}$. Al sustituir el resultado de {eq}`eq:31` en la expresión {eq}`eq:30`, hallamos que:

$$
\overline{p_{j} \frac{\partial K}{\partial p_{j}}}=\frac{1}{\beta} \int \frac{e^{-\beta H}}{Z} d \gamma=k T. 
$$ (eq:32)

Finalmente, combinando los resultados de las ecuaciones {eq}eq:32 y {eq}eq:28, obtenemos el valor promedio de la energía cinética:

$$
\bar{K}=\frac{f}{2} k T
$$

Siguiendo un procedimiento análogo para las coordenadas generalizadas q_{j} y la energía potencial, se demuestra que:

$$
\bar{V}=\frac{f}{2} k T. 
$$

Estos resultados constituyen el Teorema de Equipartición de la Energía. Este teorema establece que, si la energía cinética y potencial son funciones homogéneas de segundo orden, la energía total del sistema en equilibrio térmico se distribuye equitativamente, asignando un promedio de $\frac{1}{2}kT$ a cada término cuadrático ("grado de libertad") del Hamiltoniano.

​Cabe mencionar que este teorema es de carácter general y también puede ser demostrado bajo el formalismo del ensemble microcanónico.

## El Sólido Cristalino Clásico

Una aplicación fundamental del teorema de equipartición de la energía es el estudio del sólido cristalino. El Hamiltoniano general para un sistema de este tipo se expresa como:

$$
H = \sum_{i=1}^{3N} \frac{p_{i}^{2}}{2m} + V(q_{1}, \dots, q_{3N}).
$$

Donde $N$ es el número de átomos en la red, $p_{i}$ representa las componentes de los momentos lineales y $q_{i}$ las coordenadas de posición. En este modelo, las coordenadas $q_{i}$ representan los desplazamientos respecto a las posiciones de equilibrio de los átomos. Por convención, definimos el origen del potencial en el equilibrio, $V(0, \dots, 0) = 0$. Dado que el equilibrio mecánico implica que la fuerza neta es nula, se cumple que $\partial V / \partial q_{i} = 0$ para todo $i$ cuando $\{q_{j} = 0\}$.

En un sólido cristalino, los átomos están fuertemente ligados y sus oscilaciones térmicas alrededor de las posiciones de equilibrio son muy pequeñas ($q_{j} \simeq 0$). Esto permite expandir la energía potencial $V$ en una serie de Taylor truncada al segundo orden:

$$
V(q_{1}, \dots, q_{3N}) \simeq \frac{1}{2} \sum_{i, j=1}^{3N} \left( \frac{\partial^{2} V}{\partial q_{i} \partial q_{j}} \right)_{0} q_{i} q_{j}.
$$

Este enfoque se conoce como aproximación armónica. Bajo esta premisa, el Hamiltoniano del sólido cristalino se convierte en una función cuadrática tanto de los momentos como de las posiciones, satisfaciendo estrictamente las condiciones del teorema de equipartición.

Al haber $3N$ grados de libertad cuadráticos para la energía cinética y $3N$ para la energía potencial, la energía interna total ($U$) resulta ser:

$$
U = 3NkT.
$$

A partir de esta expresión, el calor específico molar a volumen constante se calcula como:

$$
c_{V} = 3R.
$$

Este resultado es la célebre ley de Dulong y Petit. Aunque esta ley describe con precisión el comportamiento de muchos sólidos a temperaturas elevadas, falla sistemáticamente en el límite de bajas temperaturas, donde se observa experimentalmente que el calor específico disminuye proporcionalmente a $T^{3}$. 

De hecho, la Ley de Dulong y Petit contradice la tercera ley de la termodinámica, la cual establece que el calor específico de cualquier sistema debe tender a cero cuando la temperatura absoluta se aproxima al cero operacional. Esta discrepancia histórica evidenció las limitaciones de la física clásica y fue uno de los motores principales para el desarrollo de los modelos cuánticos de Einstein y Debye.
