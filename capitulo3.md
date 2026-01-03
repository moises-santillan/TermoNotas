# Capítulo 3: Física Estadística Cuántica

# Capítulo 3: Física Estadística Cuántica

## La matriz de densidad

Desde la perspectiva de la mecánica cuántica, un sistema termodinámico nunca puede considerarse estrictamente aislado. Incluso aquellos sistemas confinados por paredes perfectamente adiabáticas, rígidas e impermeables mantienen una interacción residual con los constituyentes microscópicos de dichas fronteras. En consecuencia, el operador Hamiltoniano de un sistema termodinámico real se describe mediante la expresión:

$$
\hat{H}_{o}\left(x_{i}\right)+\hat{H}_{i}\left(x_{i}, q_{j}\right),
$$

donde $\hat{H}_{o}$ es el Hamiltoniano intrínseco que rige la dinámica interna del sistema, mientras que $\hat{H}_{i}$ representa el término de interacción con el entorno. Aquí, las variables $x_{i}$ denotan las coordenadas generalizadas de los elementos que integran el sistema, y las variables $q_{j}$ representan las coordenadas asociadas al medio externo.

Bajo la premisa de que $\hat{H}_{i}$ puede tratarse como una perturbación débil, la función de onda total del sistema, $\Psi\left(x_{i}, q_{j}\right)$, puede expandirse como una combinación lineal de las eigenfunciones de la dinámica interna, $\phi_{n}\left(x_{i}\right)$, asociadas a $\hat{H}_{o}$:

$$
\Psi\left(x_{i}, q_{j}\right)=\sum_{n} a_{n}\left(q_{j}\right) \phi_{n}\left(x_{i}\right).
$$

En esta formulación, el valor esperado de un observable representado por el operador $\hat{f}\left(x_{i}\right)$ se obtiene mediante el promedio sobre todos los grados de libertad:

$$
\bar{f}=\int \Psi^{*}\left(x_{i}, q_{j}\right) \hat{f}\left(x_{i}\right) \Psi\left(x_{i}, q_{j}\right) d x_{i} d q_{j}=\sum_{n, m} f_{n m} w_{m n},
$$

donde los elementos de matriz del observable en la base de $\hat{H}_{o}$ se definen como:

$$
f_{n m}=\int \phi_{n}^{*}\left(x_{i}\right) \hat{f}\left(x_{i}\right) \phi_{m}\left(x_{i}\right) d x_{i}
$$

en tanto que los coeficientes que ponderan la interacción con el medio se agrupan en la matriz de densidad, $w_{n m}$, están dados por:

$$
w_{n m}=\int a_{m}\left(q_{j}\right) a_{n}^{*}\left(q_{j}\right) d q_j.
$$

Las entradas de esta matriz codifican el efecto de las interacciones externas sobre el sistema. Debido a la invariancia de la traza ante cambios de base, el valor esperado del operador $\hat{f}$ puede expresarse de manera compacta como:

$$
\bar{f}=\operatorname{tr}(\underline{\underline{f}} \underline{\underline{w}}).
$$

Asumiendo, sin pérdida de generalidad, que la función de onda total $\Psi\left(x_{i}, q_{j}\right)$ está normalizada y que el conjunto $\left\{\phi_{n}\left(x_{i}\right)\right\}$ constituye una base ortonormal, la probabilidad $p_{n}$ de encontrar al sistema en el estado cuántico $\phi_{n}$ tras una medición se define como:

$$
p_{n}=\int a_{n}^{*}\left(q_{j}\right) a_{n}\left(q_{j}\right) d q_{j}=w_{n n}.
$$

## Ensemble Cuántico

Un ensemble estadístico cuántico se define como una colección virtual de un número muy grande de copias del sistema bajo estudio. Todos los miembros del ensemble están regidos por el mismo Hamiltoniano interno ($\hat{H}_{o}(x_{i})$), se encuentran sujetos a las mismas condiciones externas ($\hat{H}_{i}(x_{i}, q_{j})$) y permanecen en equilibrio termodinámico.

Esto implica que todos los sistemas del ensemble comparten el mismo espectro de estados cuánticos accesibles ($\phi_{n}(x_{i})$) y la misma probabilidad $p_{n}$ de ser hallados en un estado determinado tras una medición.

## Definición de Entropía

### Microestado del ensemble
El microestado del ensemble está determinado por la configuración de los microestados de cada uno de los sistemas integrantes. La función de estado global se construye como el producto de las funciones de estado individuales. En este contexto, al ser sistemas macroscópicos, las copias que conforman el ensemble son tratables como entidades distinguibles entre sí.

### Hipótesis de igual probabilidad a priori
Se postula que todos los microestados del ensemble compatibles con las restricciones termodinámicas impuestas son igualmente probables.

### Mesoestado cuántico
Para un ensemble de $N^{*}$ sistemas, el mesoestado se define mediante el conjunto de números de ocupación $\{\tilde{n}_{i}\}$, donde cada $\tilde{n}_{i}$ representa el número de sistemas que se encuentran en el estado cuántico $\phi_{i}$.

### Probabilidad de un mesoestado
Bajo la hipótesis de igual probabilidad a priori, la probabilidad de un mesoestado es proporcional a su peso estadístico (el número de microestados compatibles), dado por el coeficiente multinomial:

$$
W = \frac{N^{*}!}{\tilde{n}_{1}! \tilde{n}_{2}! \dots}.
$$

### Entropía
El mesoestado de máxima probabilidad es aquel que caracteriza el equilibrio macroscópico del sistema. Basándonos en la aditividad de la entropía y la relación logarítmica con la probabilidad, definimos la entropía del ensemble ($S^{*}$) como:

$$
S^{*} = k_{B} \ln \frac{N^{*}!}{\tilde{n}_{1}^{*}! \tilde{n}_{2}^{*}! \dots}. 
$$

Dado que el ensemble está compuesto por sistemas idénticos, la entropía individual ($S$) de cada sistema se deduce como:

$$
S = \frac{S^{*}}{N^{*}}. 
$$

Aplicando la aproximación de Stirling ($\ln N! \approx N \ln N - N$), se obtiene la expresión fundamental de la entropía de Gibbs:

$$
S = -k_{B} \sum_{n} p_{n} \ln p_{n}, 
$$ (eq01)

donde $p_{n} = \tilde{n}_{n}^{*} / N^{*}$ es la probabilidad de que el sistema ocupe el estado $n$. Aunque esta probabilidad está vinculada a la dinámica microscópica, en la práctica se determina mediante las restricciones macroscópicas y la segunda ley de la termodinámica.

## Ensembles Microcanónico y Canónico

Determinar la entropía mediante la resolución directa de la ecuación de Schrödinger para un sistema macroscópico es una tarea impracticable debido a la inmensa cantidad de grados de libertad. Sin embargo, este obstáculo se supera aplicando la segunda ley de la termodinámica: en condiciones de equilibrio, la distribución de probabilidades $\{p_n\}$ es aquella que maximiza la entropía bajo las restricciones macroscópicas impuestas.

A continuación, se analizan los dos formalismos fundamentales resultantes de este principio extremal.

### Ensemble Microcanónico

El ensemble microcanónico describe sistemas termodinámicamente aislados, con energía ($E$), volumen ($V$) y número de partículas ($N$) constantes. Para garantizar el equilibrio, la distribución de probabilidad sólo debe satisfacer la condición de normalización:

$$
\sum_{n} p_{n}=1. 
$$

Al maximizar la entropía funcional sujeta a esta restricción, se obtiene que todos los microestados accesibles son igualmente probables:

$$
p_{n}=\frac{1}{W}, 
$$

donde $W$ representa el número total de microestados compatibles con la energía $E$. Sustituyendo este resultado en la definición de entropía de Gibbs, recuperamos la expresión fundamental de Boltzmann:

$$
S=k_{B} \ln W. 
$$ (eq02)

### Ensemble Canónico

El ensemble canónico describe sistemas en contacto térmico con un reservorio a temperatura $T$. En este escenario, la energía del sistema puede fluctuar, por lo que las restricciones para maximizar la entropía son la normalización y la constancia de la energía promedio ($\bar{E}$):

$$
\sum_{n} p_{n}=1, \quad \sum_{n} E_{n} p_{n}=\bar{E}. 
$$

El uso de multiplicadores de Lagrange, junto con la definición estadística de temperatura ($1/T = \partial S / \partial \bar{E}$), conduce a la distribución de Boltzmann:

$$
p_{n}=\frac{\exp \left(-E_{n} / k_{B} T\right)}{Z}, 
$$

donde la función de partición $Z$ actúa como el factor de normalización y contiene la información estadística del sistema:

$$
Z=\sum_{n} \exp \left(-E_{n} / k_{B} T\right).
$$

La conexión con la termodinámica macroscópica se establece a través de la energía libre de Helmholtz ($F$), que constituye la ecuación fundamental de este ensemble:

$$
F=-k_{B} T \ln Z. 
$$ (eq03)

### Ensemble gran canónico

Este ensemble describe sistemas en equilibrio con un reservorio que intercambia tanto energía (a temperatura $T$) como partículas (a potencial químico $\mu$), manteniendo el volumen $V$ constante. 

Para asegurar el equilibrio del ensemble gran canónico como un sistema globalmente aislado, se imponen las condiciones de normalización, energía promedio y número promedio de partículas constantes:

\begin{align*}
\sum_{n} p_{n} &= 1, \\
\sum_{n} E_{n} p_{n} &= \bar{E}, \\
\sum_{n} N_{n} p_{n} &= \bar{N}. 
\end{align*}

La distribución de probabilidad que maximiza la entropía funcional {eq}`eq01` sujeta a estas restricciones se halla mediante multiplicadores de Lagrange:

$$
p_{n} = \frac{e^{-\beta(E_{n} - \mu N_{n})}}{\mathcal{Z}} 
$$

donde $\mathcal{Z}$ es la gran función de partición:

$$
\mathcal{Z} = \sum_{n} e^{-\beta(E_{n} - \mu N_{n})}. 
$$

El potencial termodinámico natural de este ensemble es el gran potencial ($\Omega$), definido como:

$$
\Omega(T, V, \mu) = U - TS - \mu N. 
$$

Comparando con la estadística, se deduce que:

$$
\Omega(T, V, \mu) = -k_{B} T \ln \mathcal{Z}(T, V, \mu). 
$$

Finalmente, los valores promedio de la energía y el número de partículas se obtienen mediante las relaciones:

$$
\bar{E} = -\frac{\partial \ln \mathcal{Z}}{\partial \beta}, \quad \bar{N} = k_{B} T \frac{\partial \ln \mathcal{Z}}{\partial \mu}. 
$$

## El sólido paramagnético

Considere un sistema compuesto por $N$ dipolos magnéticos fijos en una red espacial. En presencia de un campo magnético externo $\vec{B}$, cada dipolo puede alinearse de forma paralela o antiparalela a la dirección del campo. La energía de interacción entre un dipolo individual y el campo $\vec{B}$ se define como $-\vec{\mu} \cdot \vec{B}$, donde $\vec{\mu}$ representa el momento magnético del dipolo.

### Ensemble microcanónico

Para aplicar el formalismo microcanónico, suponemos que el sistema de $N$ dipolos se mantiene a una energía constante $E$. Dado que los dipolos ocupan posiciones fijas en el espacio, la restricción de volumen constante se satisface de forma natural, al igual que la constancia de $N$, implícita en la definición del modelo.

La energía total del sistema se expresa como:

$$
E = \mu B ((N-n) - n) = \mu B (N - 2n), 
$$ (eq04)

donde $n$ es el número de dipolos alineados paralelamente a $\vec{B}$, mientras que $B$ y $\mu$ son las magnitudes del campo y del momento magnético, respectivamente. El número de microestados $W$ compatibles con una energía fija es equivalente al número de combinaciones en las que se pueden organizar $n$ dipolos paralelos y $N-n$ antiparalelos:

$$
W = \frac{N!}{n!(N-n)!}. 
$$

Utilizando la aproximación de Stirling ($\ln N! \approx N \ln N - N$) en la definición de Boltzmann {eq}`eq02`, la entropía del sistema resulta ser:

$$
S = k_{B} \ln W \approx k_{B} \left[ N \ln \frac{N}{N-n} - n \ln \frac{n}{N-n} \right]. 
$$

Empleando la relación termodinámica $1/T = \partial S / \partial E$ y combinando con {eq}`eq04`, se obtiene la ecuación de estado que vincula la energía con la temperatura:

$$
E = -N \mu B \tanh \left( \frac{\mu B}{k_{B} T} \right). 
$$

### Ensemble canónico

En el formalismo canónico, el sistema se encuentra en equilibrio con un baño térmico a temperatura $T$, permitiendo que su energía fluctúe. En este caso, todas las $2^N$ configuraciones posibles de orientaciones de dipolos son microestados accesibles para el ensemble.

La función de partición del sistema, según la ecuación {eq}`eq03`, se calcula como la suma sobre todos los estados de espín individuales:

$$
Z = \sum_{n_{1}, \dots, n_{N} = \pm 1} \exp \left( \frac{\sum n_{i} \mu B}{k_{B} T} \right) = \left( e^{\mu B / k_{B} T} + e^{-\mu B / k_{B} T} \right)^{N}. 
$$

A partir de $Z$, la energía interna promedio del sistema se obtiene como:

$$
\bar{E} = -\frac{\partial \ln Z}{\partial \beta} = -N \mu B \tanh \left( \frac{\mu B}{k_{B} T} \right).
$$

donde $\beta = 1 / k_{B} T$. Nótese que, en el límite termodinámico, ambos ensembles conducen al mismo resultado físico.

## Estadísticas de Bose-Einstein y Fermi-Dirac

### Ecuación de onda del gas ideal cuántico

Considere un gas compuesto por $N$ partículas idénticas e indestinguibles que no interactúan entre sí. En este sistema, cada partícula está regida por el mismo Hamiltoniano de una sola partícula, $\hat{H}^{(1)}(x)$. Sean $\psi_{n}(x)$ y $\varepsilon_{n}$ las eigenfunciones y los eigenvalores de $\hat{H}^{(1)}(x)$ tales que $\hat{H}^{(1)} \psi_{n} = \varepsilon_{n} \psi_{n}$. 

Dado que el gas es ideal (ausencia de interacción interparticular), el Hamiltoniano total del sistema es la suma de los Hamiltonianos individuales:

$$
\hat{H}(x_{1}, x_{2}, \dots, x_{N}) = \sum_{i=1}^{N} \hat{H}^{(1)}(x_{i}). 
$$

Consecuentemente, la energía total del gas —el eigenvalor de $\hat{H}(x_{1}, \dots, x_{N})$— resulta ser la suma de las energías de cada partícula:

$$
E_{n_{1}, n_{2}, \dots, n_{N}} = \sum_{i=1}^{N} \varepsilon_{n_{i}}. 
$$

Donde el índice $n_{i}$ (con $i=1, 2, \dots, N$) determina el estado $\psi_{n_{i}}$ de la $i$-ésima partícula. Para construir la función de estado global del gas, $\Psi_{n_{1}, \dots, n_{N}}(x_{1}, \dots, x_{N})$, a partir de las funciones de estado individuales $\psi_{n_{i}}(x_{i})$, debemos asegurar que satisfaga la ecuación de Schrödinger:

$$
\hat{H}(x_{1}, \dots, x_{N}) \Psi_{n_{1}, \dots, n_{N}} = E_{n_{1}, \dots, n_{N}} \Psi_{n_{1}, \dots, n_{N}}. 
$$

Debido a la indistinguibilidad de las partículas, la función de estado debe preservar la misma información física ante el intercambio de cualesquiera dos partículas. Dado que el significado físico reside en la densidad de probabilidad $|\Psi|^2$ y no en $\Psi$ directamente, se debe cumplir que:

$$
\Psi(\dots, x_{i}, \dots, x_{j}, \dots) = \pm \Psi(\dots, x_{j}, \dots, x_{i}, \dots). 
$$

Esta simetría de intercambio divide a las partículas en dos categorías fundamentales:
* **Bosones:** Aquellas con funciones de estado simétricas (+).
* **Fermiones:** Aquellas con funciones de estado antisimétricas (-).

Para un gas de bosones, la función de estado se construye como una combinación lineal simétrica de las funciones individuales:

$$
\Psi_{B}(x_{1}, \dots, x_{N}) = \frac{\sqrt{N_{1}! N_{2}! \dots}}{\sqrt{N!}} \sum_{\sigma} \psi_{n_{\sigma_{1}}}(x_{1}) \dots \psi_{n_{\sigma_{N}}}(x_{N}), 
$$ (eq05)

donde la suma se realiza sobre todas las permutaciones posibles $\sigma$ del conjunto $\{1, 2, \dots, N\}$ y $N_{\nu} = \sum_{i=1}^{N} \delta_{n_{i}, \nu}$ representa el número de ocupación del estado $\psi_{\nu}$. En el caso de los bosones, el número de ocupación puede variar desde cero hasta $N$.

Para un gas de fermiones, la función de estado debe ser totalmente antisimétrica y se expresa mediante el tensor de Levi-Civita $\epsilon^{\sigma_{1} \dots \sigma_{N}}$ (o equivalentemente, mediante un determinante de Slater):

$$
\Psi_{F}(x_{1}, \dots, x_{N}) = \frac{1}{\sqrt{N!}} \sum_{\sigma} \epsilon^{\sigma_{1}, \dots, \sigma_{N}} \psi_{n_{\sigma_{1}}}(x_{1}) \dots \psi_{n_{\sigma_{N}}}(x_{N}). 
$$ (eq06)

La antisimetría intrínseca de los fermiones impide que dos partículas ocupen el mismo estado cuántico ($n_{i} \neq n_{j}$ para todo $i \neq j$), principio conocido como el Principio de Exclusión de Pauli. Como consecuencia directa, el número de ocupación $N_{\nu}$ para cualquier estado fermiónico solo puede tomar los valores cero o uno.

### Representación de los números de ocupación

A partir de las expresiones {eq}`eq05` y {eq}`eq06`, se concluye que si se dispone del conjunto de funciones de estado de una partícula $\{\psi_{n}\}$, el estado global del gas queda unívocamente determinado por los números de ocupación $\{N_{n}\}$, independientemente de si el sistema está constituido por fermiones o bosones. 

Esto sugiere la adopción de una representación cuántica donde los números de ocupación actúan como los números cuánticos del sistema (espacio de Fock). En este formalismo, la función de estado del gas se escribe como:

$$
\Psi = | N_{1}, N_{2}, \dots \rangle. 
$$

### Números de ocupación promedio

En esta representación, la gran función de partición ($\mathcal{Z}$) para un gas de bosones se calcula sumando sobre todos los posibles valores de los números de ocupación ($N_{\nu} = 0, 1, 2, \dots$):

$$
\mathcal{Z} = \sum_{N_{1}, N_{2}, \dots = 0}^{\infty} \exp \left[ -\beta \left( N_{1}(\varepsilon_{1} - \mu) + N_{2}(\varepsilon_{2} - \mu) + \cdots  \right) \right] = \prod_{\nu} \left( 1 - e^{-\beta(\varepsilon_{\nu} - \mu)} \right)^{-1}, 
$$

donde el índice $\nu$ identifica los distintos estados monoportícula. Por otro lado, para un gas de fermiones, debido al principio de exclusión de Pauli, los números de ocupación solo admiten los valores $0$ y $1$:

$$
\mathcal{Z} = \sum_{N_{1}, N_{2}, \dots = 0, 1} \exp \left[ -\beta \left( N_{1}(\varepsilon_{1} - \mu) + N_{2}(\varepsilon_{2} - \mu) + \cdots  \right) \right]  = \prod_{\nu} \left( 1 + e^{-\beta(\varepsilon_{\nu} - \mu)} \right). 
$$

Ambos resultados pueden sintetizarse en una única expresión compacta:

$$
\mathcal{Z} = \prod_{\nu} \left( 1 \pm e^{-\beta(\varepsilon_{\nu} - \mu)} \right)^{\pm 1}, 
$$

donde los signos superior ($+$) e inferior ($-$) corresponden a fermiones y bosones, respectivamente. Utilizando la relación termodinámica para el número promedio de partículas $\bar{N}$, se obtiene:

$$
\bar{N} = \sum_{\nu} \frac{1}{e^{\beta(\varepsilon_{\nu} - \mu)} \pm 1}. 
$$

Considerando que $\bar{N} = \sum_{\nu} \bar{n}_{\nu}$, se deduce que los números de ocupación promedio para cada estado en un gas ideal cuántico están dados por:

$$
\bar{n}_{\nu} = \frac{1}{e^{\beta(\varepsilon_{\nu} - \mu)} \pm 1}. 
$$

En el límite de temperatura cero ($\beta \to \infty$), el comportamiento de estas distribuciones diverge notablemente:
* Para **fermiones**, $\bar{n}_{\nu}$ tiende a una función escalón que vale uno si $\varepsilon_{\nu} < \mu$ y cero en caso contrario.
* Para **bosones**, la condición $\bar{n}_{\nu} \geq 0$ exige que $\varepsilon_{\nu} \geq \mu$. De hecho, cuando $\varepsilon_{\nu} \to \mu$, $\bar{n}_{\nu}$ diverge al infinito (condensación de Bose-Einstein).

Puesto que el número de ocupación promedio solo depende de la energía del estado, se utiliza habitualmente la notación simplificada $\bar{n}(\varepsilon)$:

$$
\bar{n}(\varepsilon) = \frac{1}{e^{\beta(\varepsilon - \mu)} \pm 1}. 
$$

## Función de densidad de estados

Considere una partícula de masa $m$ confinada en un recipiente cúbico de lado $L$ y volumen $V = L^3$. La ecuación de Schrödinger para este sistema de partícula libre está dada por:

$$
-\frac{\hbar^{2}}{2 m} \nabla^{2} \psi(x, y, z) = \varepsilon \psi(x, y, z). 
$$

Imponiendo las condiciones de frontera de pozo de potencial infinito (donde la función de onda se anula en las paredes del recipiente):

$$
\psi = 0 \quad \text{en} \quad x,y,z \in \{0, L\}.
$$

La solución para la función de onda es:

$$
\psi(x, y, z) = C \sin \left(\frac{\kappa_{x} \pi}{L} x\right) \sin \left(\frac{\kappa_{y} \pi}{L} y\right) \sin \left(\frac{\kappa_{z} \pi}{L} z\right), 
$$

donde los números cuánticos $\kappa_{x}, \kappa_{y}, \kappa_{z}$ son enteros positivos que deben satisfacer la relación de energía:

$$
\kappa_{x}^{2} + \kappa_{y}^{2} + \kappa_{z}^{2} = \frac{2 m \varepsilon L^{2}}{\pi^{2} \hbar^{2}}. 
$$

Geométricamente, los estados accesibles se representan como los vértices de una red cúbica unitaria en el octante positivo del espacio $\vec{\kappa}$. En el límite de energías elevadas, el número de estados acumulados con energía menor o igual a $\varepsilon$, denotado como $\Gamma(\varepsilon)$, se aproxima como la octava parte del volumen de una esfera:

$$
\Gamma(\varepsilon) = \frac{V}{6 \pi^{2}} \left(\frac{2 m \varepsilon}{\hbar^{2}}\right)^{3/2}. 
$$

La función de densidad de estados, $\mathcal{D}(\varepsilon)$, representa el número de estados por unidad de energía en el intervalo $[\varepsilon, \varepsilon + d\varepsilon]$ y se calcula como $d\Gamma/d\varepsilon$:

$$
\mathcal{D}(\varepsilon) d\varepsilon = \frac{\gamma V}{4 \pi^{2}} \left(\frac{2 m}{\hbar^{2}}\right)^{3/2} \varepsilon^{1/2} d\varepsilon, 
$$

donde $\gamma$ es el factor de degeneración (por ejemplo, $\gamma=2$ para el espín). El valor promedio de cualquier observable $F(\varepsilon)$ se determina mediante:

$$
\bar{F} = \int_{0}^{\infty} F(\varepsilon) \bar{n}(\varepsilon) \mathcal{D}(\varepsilon) d\varepsilon. 
$$

## El límite clásico

Consideremos el régimen en el que el número de ocupación promedio es mucho menor que la unidad ($\bar{n} \ll 1$). Esta condición se cumple cuando $\exp[(\varepsilon - \mu)/k_{B}T] \gg 1$, permitiendo aproximar la ocupación mediante la estadística de Boltzmann:

$$
\bar{n}(\varepsilon) = \lambda e^{-\varepsilon / k_{B} T}, 
$$

donde $\lambda = \exp(\mu / k_{B} T)$ es la fugacidad. En este límite de baja ocupación, la distinción cuántica entre fermiones y bosones se vuelve irrelevante.

El número promedio de partículas $\bar{N}$ se calcula integrando sobre todos los estados:

$$
\bar{N} = \int_{0}^{\infty} \bar{n}(\varepsilon) \mathcal{D}(\varepsilon) d\varepsilon = V \lambda \left(\frac{m k_{B} T}{2 \pi \hbar^{2}}\right)^{3/2}. 
$$

Al despejar $\lambda$, obtenemos la ocupación promedio en términos de variables macroscópicas:

$$
\bar{n}(\varepsilon) = \frac{N}{V} \left(\frac{2 \pi \hbar^{2}}{m k_{B} T}\right)^{3/2} e^{-\varepsilon / k_{B} T}. 
$$

Finalmente, la energía promedio del sistema en este límite resulta ser:

$$
\bar{\varepsilon} = \frac{3}{2} \bar{N} k_{B} T. 
$$

Este resultado coincide exactamente con la energía interna de un gas ideal clásico, confirmando que la estadística de Boltzmann constituye el límite clásico de los gases cuánticos.

## La energía de Fermi

En el límite de temperatura cero ($T \to 0$), la distribución de ocupación promedio para fermiones se comporta como una función escalón: los estados con energía inferior al potencial químico $\mu$ están totalmente ocupados ($\bar{n}=1$), mientras que aquellos con energía superior están vacíos ($\bar{n}=0$). En este régimen, el potencial químico se define como la **energía de Fermi** ($\varepsilon_{F} = \mu$).

Bajo estas condiciones, el número total de partículas de un gas de fermiones se calcula integrando la densidad de estados hasta el nivel de Fermi:

$$
\bar{N} = \int_{0}^{\varepsilon_{F}} \mathcal{D}(\varepsilon) d \varepsilon. 
$$

Resolviendo la integral a partir de la expresión para $\mathcal{D}(\varepsilon)$ y despejando el término energético, se obtiene la expresión para la energía de Fermi:

$$
\varepsilon_{F} = \frac{\hbar^{2}}{2 m} \left( \frac{6 \pi^{2} \bar{N}}{\gamma V} \right)^{2/3}. 
$$

## Gas de electrones

Consideremos el incremento en la energía total ($\Delta \bar{E}$) de un gas de $N$ electrones cuando el sistema se calienta desde el cero absoluto hasta una temperatura $T$. Esta variación se expresa como la diferencia entre la energía térmica y la energía en el estado fundamental:

$$
\Delta \bar{E} = \int_{0}^{\infty} \varepsilon \mathcal{D}(\varepsilon) \bar{n}(\varepsilon) d \varepsilon - \int_{0}^{\varepsilon_{F}} \varepsilon \mathcal{D}(\varepsilon) d \varepsilon.
$$

Utilizando la identidad del número de partículas $N = \int \bar{n} \mathcal{D} d\varepsilon$ y manipulando las integrales mediante la energía de Fermi, podemos reescribir la variación de energía de una forma más intuitiva:

$$
\Delta \bar{E} = \int_{\varepsilon_{F}}^{\infty} (\varepsilon - \varepsilon_{F}) \mathcal{D}(\varepsilon) \bar{n}(\varepsilon) d \varepsilon + \int_{0}^{\varepsilon_{F}} (\varepsilon_{F} - \varepsilon) \mathcal{D}(\varepsilon) [1 - \bar{n}(\varepsilon)] d \varepsilon. 
$$

En esta ecuación, el primer término representa la energía necesaria para promover electrones desde el nivel de Fermi hacia niveles superiores, mientras que el segundo término representa la energía requerida para desplazar electrones desde orbitales profundos hacia la superficie de Fermi.

### Capacidad calorífica electrónica

Dado que la dependencia térmica reside exclusivamente en $\bar{n}(\varepsilon)$, la capacidad calorífica del gas de electrones se define como:

$$
C_{\mathrm{el}} = \frac{d \bar{E}}{d T} = \int_{0}^{\infty} (\varepsilon - \varepsilon_{F}) \mathcal{D}(\varepsilon) \frac{d \bar{n}(\varepsilon)}{d T} d \varepsilon. 
$$

En metales a temperaturas ordinarias ($T \ll T_F$), la derivada $d\bar{n}/dT$ solo es significativa en la vecindad de $\varepsilon_{F}$. Por lo tanto, aproximamos la densidad de estados como una constante $\mathcal{D}(\varepsilon) \simeq \mathcal{D}(\varepsilon_{F})$:

$$
C_{\mathrm{el}} \simeq \mathcal{D}(\varepsilon_{F}) \int_{0}^{\infty} (\varepsilon - \varepsilon_{F}) \frac{d \bar{n}}{d T} d \varepsilon. 
$$

Realizando el cambio de variable $x = (\varepsilon - \varepsilon_{F}) / k_{B} T$ y utilizando el valor de la integral estándar ($\pi^{2} / 3$), junto con la relación $\mathcal{D}(\varepsilon_{F}) = 3N / 2\varepsilon_{F}$, la capacidad calorífica electrónica final resulta ser:

$$
C_{\mathrm{el}} \simeq \frac{1}{2} \pi^{2} N k_{B} \left( \frac{k_{B} T}{\varepsilon_{F}} \right). 
$$

Este resultado demuestra que la contribución electrónica a la capacidad calorífica es lineal con la temperatura, lo cual explica el comportamiento observado en metales a bajas temperaturas donde la contribución de la red (proporcional a $T^3$) se vuelve despreciable.

### Radiación de cuerpo negro

Considere un gas de fotones en equilibrio térmico a una temperatura $T$ dentro de un recipiente de volumen $V$. La energía de cada fotón está determinada por su frecuencia angular $\omega$ mediante la relación $\varepsilon = \hbar \omega$. Dado que el número de fotones no se conserva en el sistema, el potencial químico del gas es nulo ($\mu = 0$). En consecuencia, el número de ocupación promedio se rige estrictamente por la estadística de Bose-Einstein:

$$
\bar{n}(\omega) = \frac{1}{e^{\hbar \omega / k_{B} T} - 1}. 
$$

Considerando que para cada frecuencia existen dos estados de polarización independientes, la resolución de la ecuación de onda electromagnética permite derivar la densidad de estados para los fotones:

$$
\mathcal{D}(\omega) d \omega = \frac{V}{\pi^{2} c^{3}} \omega^{2} d \omega, 
$$

donde $c$ representa la velocidad de la luz. La energía por unidad de volumen para los fotones en el intervalo de frecuencias $[\omega, \omega + d\omega]$, conocida como densidad de energía espectral, se define como:

$$
u_{\omega} d \omega = \frac{\bar{n}(\omega) \hbar \omega \mathcal{D}(\omega)}{V} d \omega = \frac{\hbar}{\pi^{2} c^{3}} \frac{\omega^{3}}{e^{\hbar \omega / k_{B} T} - 1} d \omega. 
$$

La densidad de energía total del gas se obtiene integrando sobre todas las frecuencias posibles:

$$
u = \int_{0}^{\infty} u_{\omega} d \omega = \left( \frac{\pi^{2} k_{B}^{4}}{60 \hbar^{3} c^{2}} \right) T^{4}.
$$

Este resultado constituye la Ley de Stefan-Boltzmann. Si se practica un pequeño orificio en el recipiente, este actúa como un cuerpo negro ideal. La intensidad de la radiación emitida ($I$) se relaciona con la densidad de energía mediante $I = cu/4$, resultando en:

$$
I = \left( \frac{\pi^{2} k_{B}^{4}}{15 \hbar^{3} c^{3}} \right) T^{4} = \sigma T^4. 
$$

## Capacidad calorífica del sólido cristalino

Un sólido cristalino compuesto por $N$ átomos dispuestos en una red periódica posee $3N$ modos normales de oscilación. Según la mecánica cuántica, la energía de estas vibraciones está cuantizada en paquetes de magnitud $\hbar \omega$. Estas excitaciones elementales se comportan como un gas ideal de cuasipartículas denominadas fonones.

Los fonones son bosones de potencial químico nulo ($\mu = 0$) y presentan una degeneración característica de 3, correspondiente a las tres ramas de polarización: dos transversales y una longitudinal. A diferencia de los fotones, el espectro de frecuencias de los fonones es finito, existiendo una frecuencia de corte superior $\omega_{\text{max}}$ impuesta por la naturaleza discreta de la red atómica.

Bajo este modelo, la energía promedio del sólido en equilibrio térmico se calcula integrando sobre el espectro de frecuencias permitido:

$$
\bar{E} = \int_{0}^{\omega_{\text{max}}} \frac{\hbar \omega}{e^{\beta \hbar \omega} - 1} \mathcal{D}(\omega) d \omega. 
$$ (eq07)

### Aproximación de Einstein

En 1907, Albert Einstein propuso un modelo fundamental para la capacidad calorífica de los sólidos cristalinos. Su hipótesis central consistía en suponer que todos los modos normales de oscilación de la red poseen una única frecuencia angular característica $\omega_E$. Matemáticamente, esto se traduce en una densidad de estados proporcional a una función delta de Dirac: $\mathcal{D}(\omega) = 3N\delta(\omega - \omega_E)$. 

Bajo esta premisa, la energía promedio del sistema (derivada de la ecuación {eq}`eq07`) se reduce a:

$$
\bar{E} = \frac{3N\hbar\omega_E}{e^{\beta\hbar\omega_E} - 1}. 
$$

Al derivar esta expresión respecto a la temperatura $T$ (donde $\beta = 1/k_B T$), se obtiene la capacidad calorífica a volumen constante para el modelo de Einstein:

$$
C_V = 3Nk_B \left( \frac{\Theta_E}{T} \right)^2 \frac{e^{\Theta_E/T}}{(e^{\Theta_E/T} - 1)^2}. 
$$

donde $\Theta_E = \hbar\omega_E / k_B$ es la temperatura de Einstein. El calor específico molar se expresa entonces como:

$$
c_V^* = 3R \left( \frac{\Theta_E}{T} \right)^2 \frac{e^{\Theta_E/T}}{(e^{\Theta_E/T} - 1)^2}. 
$$

Este modelo predice correctamente que, en el límite de altas temperaturas ($T \gg \Theta_E$), el calor específico tiende al valor clásico de $3R$ (Ley de Dulong y Petit). Sin embargo, en el límite $T \to 0$, predice un decaimiento exponencial que contradice la evidencia experimental, la cual muestra una dependencia proporcional a $T^3$.


### Aproximación de Debye

Para corregir la discrepancia del modelo de Einstein, Peter Debye propuso en 1912 una densidad de estados basada en el comportamiento de las ondas elásticas en un medio continuo (fonones acústicos), siguiendo una ley cuadrática hasta una frecuencia de corte $\omega_D$:

$$
\mathcal{D}(\omega) = 
\begin{cases} 
\frac{3V}{2\pi^2 v_s^3} \omega^2, & \omega \leq \omega_D. \\ 
0, & \omega > \omega_D .
\end{cases} 
$$

La frecuencia de Debye ($\omega_D$) se determina mediante la normalización del número total de modos ($3N$):

$$
\omega_D = \left( \frac{6\pi^2 N v_s^3}{V} \right)^{1/3}. 
$$

La energía elástica promedio del sólido queda expresada por:

$$
\bar{E} = \frac{9N(k_B T)^4}{(\hbar\omega_D)^3} \int_{0}^{x_D} \frac{x^3}{e^x - 1} dx, 
$$

donde $x_D = \Theta_D / T$ y $\Theta_D = \hbar\omega_D / k_B$ es la temperatura de Debye. En el límite de bajas temperaturas ($T \ll \Theta_D$), la integral puede aproximarse extendiendo el límite a infinito, resultando en:

$$
\bar{E} \simeq \frac{3\pi^4 N k_B T^4}{5 \Theta_D^3}. 
$$

Finalmente, el calor específico molar en este régimen resulta ser:

$$
c_V^* = \frac{12\pi^4 R}{5} \left( \frac{T}{\Theta_D} \right)^3. 
$$

Esta famosa ley de $T^3$ de Debye concuerda con gran precisión con los resultados experimentales, capturando correctamente la física de las excitaciones de baja energía (fonones de gran longitud de onda) a bajas temperaturas.













