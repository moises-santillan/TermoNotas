# Capítulo 2: Física Estadística Clásica

## Conceptos Fundamentales

**Sistema Termodinámico:** Es un sistema dinámico (mecánico en este caso) con un número de grados de libertad del orden del número de Avogrado.

**Estado Macroscópico:** El estado macroscópico o mesoestado de un sistema termodinámico es sinónimo de estado de equilibrio. Así, en un sistema con $n$ grados de libertad termodinámicos, el macroestado está determinado por el valor de las $n$ variables independientes. Para propósitos de esta parte del curso consideraremos únicamente sistemas simples en la representación de la entropía, por lo que el conjunto de variables independientes es ( $U, V, N_{i}$ ).

**Estado Microscópico:** El estado microscópico o microestado de un sistema termodinámico con $f$ grados de libertad dinámicos $\left(f \approx 10^{23}\right)$ está determinado por el valor de las $f$ coordenadas generalizadas y los $f$ momentos generalizados.

**Espacio Fase Termodinámico:** Para un sistema con $n$ grados de libertad termodinámicos, el espacio fase termodinámico es un espacio cartesiano con $n$ dimensiones, cada una de las cuales corresponde a una de las variables termodinámicas independientes. Por construcción, el estado macroscópico de un sistema termodinámico se representa mediante un punto en el espacio fase termodinámico correspondiente.

**Espacio Fase Dinámico o Espacio $\Gamma$:** Para un sistema con $f$ grados de libertad dinámicos, el espacio $\Gamma$ es un espacio de $2 f$ dimensiones, $f$ de las cuales corresponden a las coordenadas generalizadas, mientras que las otras $f$ corresponden a los momentos generalizados. Por construcción, el estado microscópico de un sistema termodinámico se representa mediante un punto en el espacio $\Gamma$ correspondiente.

**Ensemble Termodinámico:** Es un conjunto de sistemas dinámicos que obedecen el mismo Hamiltoniano microscópico y cuyos macroestados son iguales, aunque sus microestados son generalmente distintos.

## Microestados, Macroestados y Mesoestados 

### Representación de un Macroestado en el espacio $\Gamma$

En un macroestado, el valor de todas las variables termodinámicas permanece constante en el tiempo. Sin embargo y aun cuando el sistema está en equilibrio, su microestado cambia constantemente. En otras palabras, dado un macroestado, existe una gran cantidad de microestados compatibles con él. Dicho conjunto de microestados está completamente determinado por las restricciones macroscópicas (los valores de las variables termodinámicas independientes).

Los puntos representativos de los microestados compatibles con el macroestado conforman una región en el espacio $\Gamma$. En adelante, llamaremos a esta región la región $\Omega$. El tamaño y forma de $\Omega$ están determinados por las restricciones macroscópicas. La región $\Omega$ es la representación de geométrica del macroestado en el espacio $\Gamma$.

Recapitulando, el estado microscópico describe al sistema de la manera más precisa. Geométricamente, establece la posición exacta del punto representativo del microestado en el espacio $\Gamma$. Para ello requiere de conocer el valor del orden de $10^{23}$ variables, $f$ coordenadas generalizadas y $f$ momentos generalizados. Por otra parte, el conocimiento del estado macroscópico establece una descripción mucho más gruesa. En esta descripción no es posible decir la posición exacta del punto representativo del microestado en el espacio $\Gamma$. Solamente establece una región en dicho espacio dentro de la se encuentra el punto representativo. Para ello se requiere un número mucho más pequeño de variables (del orden de $10^{1}$ ). Para sistemas simples en la representación de la entropía las variables del macroestado son $U, V$, y $N_{i}$.

### Representación del Microestado de un Ensemble en $\Gamma$

Para determinar el microestado de un ensemble es necesario especificar el microestado de cada uno de los sistemas que lo conforman. Esto significa conocer los valores de $2 N^{*} f$ variables, $N^{*} f$ correspondientes a coordenadas generalizadas y $N^{*} f$ correspondientes a momentos generalizados. $N^{*}$ es el número de sistemas que conforman el ensemble. Como se trata de un sistema termodinámico $f \approx 1 o^{23}$. El microestado del ensemble se representa en el espacio $\Gamma$ mediante los $N^{*}$ puntos representativos de los microestados de los sistemas del ensemble.

### Representación del Macroestado de un ensemble en $\Gamma$

Dado que todos los sistemas del ensemble son macroscópicamente idénticos, para especificar el macroestado del sistema solamente se necesita conocer el número de sistemas que lo conforman ( $N^{*}$ ), además de las variables macroscópicas que determinan el macroestado de cada sistema ( $U, V, N_{i}$ ). Por la misma razón, la región $\Omega$ que representa el macroestado de cada uno de los sistemas del ensemble también representa el macroestado del ensemble. Sólo que en este caso, hay $N^{*}$ puntos representativos en el interior de la misma.

Comparando, el microestado del ensemble establece la descripción más precisa posible (determina la posición exacta de los puntos representativos de los microestados de todos los sistemas) y con la mayor cantidad de información (los valores de las $N^{*} f$ coordenadas generalizadas y los $N^{*} f$ momentos generalizados). Por su parte, la descripción correspondiente al macroestado del ensemble es mucho más gruesa (solamente determina una región $\Omega$ dentro de la cual están los $N^{*}$ puntos representativos) e involucra mucho menor información (los valores de las variables $U, V, N_{i}$ y $N^{*}$ ).

### Estado Mesoscópico o Mesoestado

La conexión entre los estados micro y macroscópicos se construye estadísticamente a través de un estado intermedio. Este estado intermedio, conocido como estado mesoscópico o mesoestado, se construye de la siguiente forma. Se toma la región $\Omega$ que representa el macroestado y se divide en $r$ celdas. Para que el mesoestado que estamos construyendo sea en verdad intermedio, debemos tener que $1 \ll r \ll f$, con $f$ el número de grados de libertad dinámicos del sistema. Además, si $\omega_{i}$ representa el volumen fase de la $i$-ésima celda, $\omega_{i} \approx \omega_{j}, \forall i \neq j$. El mesoestado queda entonces definido por el conjunto de números de ocupación, $n_{i}^{*}$: el número de puntos representativos que yacen en la $i$-ésima celda. Evidentemente $n_{i}^{*}$ satisface $\sum_{i} n_{i}^{*}=N^{*}$.

Es fácil ver que así como está definido, es mesoestado establece una descripción intermedia en todos los sentidos entre el microestado y macroestado. La descripción mesoscópica es más fina que la macroscópica pues además de saber que los $N^{*}$ puntos representativos están en el interior de $\Omega$, tenemos información acerca de cómo están distribuidos en su interior. Sin embargo, no se alcanza la precisión de la descripción microscópica, en la que se establece la posición exacta de cada punto representativo. En cuanto al número de variables involucradas, el estado mesoscópico también es intermedio. El microestado requiere de $N^{*} f$ variables, el macroestado requiere sólo del orden de $10^{0}$ variables. Por su parte, el mesoestado está definido por las variables mesoscópicas (que determinan la región $\Omega$ ), más los $r$ números de ocupación. Y dado que sabemos que $1 \ll r \ll f$, tenemos que el número de variables requeridas por el mesoestado es mucho menos que el número de variables del microestado, pero mucho mayor que el del macroestado.

## Conexión entre las Descripciones Micro y Macroscópicas

### Hipótesis de Igualdad de Probabilidad a Priori

Esta hipótesis establece que todos los estados microscópicos compatibles con el macroestado son igualmente probables. Como su nombre lo dice, es una hipótesis. No está basada en primeros principios. Su validez está sujeta a la comprobación esperimental de los resultados derivados a partir de ella.

### Probabilidad de un Mesoestado

Dado que la representación gráfica del macroestado únicamente establece que los puntos representativos de los sistemas del ensemble yacen el la región $\Omega$, sin precisar dónde, todas las combinaciones de números de ocupación que satisfagan $\sum_{i} n_{i}^{*}=N^{*}$ definirán mesoestados compatibles con el estado macroscópico. Por otra parte, si se cambia la posición de un punto representativo dentro de una celda, o si se intercambian dos puntos representativos entre celdas distintas, el microestado del sistema cambia, pero sin alterar su mesoestado pues los números de ocupación permanecen iguales.

De lo anterior se sigue que dado un macroestado, hay muchos mesoestados compatibles con él. Y que para cada mesoestado, hay muchos microestados compatibles. Esto nos permite estimar la probabilidad de un mesoestado. En virtud de la hipótesis de equilibrio local, la probabilidad de un mesoestado es proporcional al número de microestados compatibles con él.

El número de microestados compatibles con el mesoestado determinado por el conjunto de números de ocupación $n_{i}^{*}$ se calcula como

$$
\frac{N^{*}!}{n_{1}^{*}!n_{2}^{*}!\ldots n_{r}^{*}!} \omega_{1}^{n_{r}^{*}} \omega_{2}^{n_{1}^{*}} \ldots \omega_{r}^{n_{r}^{*}}.
$$

La fracción con los factoriales da cuenta del número de maneras en que los $N^{*}$ puntos representativos se pueden acomodar en $r$ celdas, poniendo $n_{1}^{*}$ en la primera, $n_{2}^{*}$ en la segunda, etc. Los factores de la forma $\omega_{i}^{n_{i}^{*}}$ dan cuenta del número de posiciones que los $n_{i}^{*}$ puntos representativos de la $i$-ésima celda pueden tomar en su interior.

### Definición de Entropía

Como se vió anteriormente, la probabilidad de un mesoestado es función del conjunto de números de ocupación. Sea $\tilde{n}_{i}^{*}$ el conjunto de números de ocupación correspondientes al mesoestado más probable de todos.

El evolucionar en el tiempo, el microestado del sistema cambia constantemente. De acuerdo con la hipótesis de igualdad de probabilidad a priori, después de un tiempo bastante largo, el sistema pasa tanto tiempo en uno de sus microestados compatibles como en cualquier otro. Sin embargo, el tiempo que el sistema pasa en cada mesoestado no es el mismo, sino que es proporcional al número de microestados compatibles con él. En otras palabras, al evolucionar, el sistema pasa más tiempo en el mesoestado más probable que en cualquier otro. En este sentido, resulta razonable suponer que el mesoestado más probable caracteriza al macroestado. De esta forma, la conexión entre las descripciones meso y macroscópica a construiremos usando el mesoestado más probable.

De segunda ley sabemos que si el ensemble está aislado y en equilibrio termodinámico, el estado de equilibrio se caracteriza por tener la entropía máxima, con respecto al conjunto de estados termodinámicos compatibles con las restricciones macroscópicas.

Recapitulando, un ensemble en equilibrio tiene un único macroestado. Compatibles con este macroestado hay muchos mesoestados compatibles. De todos los mesoestados compatibles con el macroestado, el que maximiza la probabilidad es el que caracteriza al estado de equilibrio. Por otra parte, un ensemble aislado tiene un estado de equilibrio único. Se pueden construir muchos estados termodinámicos compatibles con el estado de equilibrio, imponiendo restricciones internas. De todos los estados termodinámicos así construidos, el estado de equilibrio es el que tiene probabilidad máxima.

Sabemos que dado un ensemble aislado, su macroestado y su estado de equilibrio son la misma cosa. Las similitudes mencionadas en el párrafo anterior sugieren relacionar el conjunto de mesoestados compatibles con el macroestado, con el conjunto de estados termodinámicos compatibles con el estado de equilibrio. Si lo anterior es válido, entonces el estado termodinámico o mesoestado que caracteriza al estado de equilibrio o macroestado es aquél que al mismo tiempo tiene probabilidad y entropía máximas, lo que sugiere una relación entre la probabilidad y la entropía. Por otra parte, la probabilidad es multiplicativa (la probabilidad de dos eventos independientes es el producto de las probabilidades de los eventos individuales), mientras que la entropía es aditiva (la entropía de dos sistemas independientes es la suma de las entropías individuales). Se puede demostrar que la única relación entre probabilidad y entropía que se maximiza para el mismo mesoestado y es compatible con la multiplicatividad de la probabilidad y la aditividad de la entropía es si la entropía es proporcional al logaritmo de la probabilidad.

Del razonamiento anterior se sigue que la entropía del estado de equilibrio del ensemble ( $S^{*}$ ) se puede calcular a partir de los números de ocupación del ensemble más probable $\left(\tilde{n}_{i}^{*}\right)$ como

$$
S^{*}=k \ln \left[\frac{N^{*}!}{\tilde{n}_{1}^{*}!\tilde{n}_{2}^{*}!\ldots \tilde{n}_{r}^{*}!} \omega_{1}^{\tilde{n}_{r}^{*}} \omega_{2}^{\tilde{n}_{1}^{*}} \ldots \omega_{r}^{\tilde{n}_{r}^{*}}\right]. 
$$ (eq:01)

$k$ es la constante de Boltzmann, que es una constante universal con unidades de Joules sobre Kelvin (unidades de entropía).

## La Entropía de Gibbs

### Entropía de Cada Sistema del Ensemble

La ecuación {eq}`eq:01` permite calcular la entropía del ensemble a partir de los números de ocupación del mesoestado más probable. Todos los sistemas del ensemble están en equilibrio y tienen el mismo macroestado. Esto significa que la entropía está bien definida y que todos los sistemas tienen el mismo valor de entropía. Haciendo uso de este hecho, así como de la aditividad de la entropía, la entropía de cada sistema del ensemble se calcula como

$$
S=\frac{S^{*}}{N^{*}}=k \frac{1}{N^{*}} \ln \left[\frac{N^{*}!}{\tilde{n}_{1}^{*}!\tilde{n}_{2}^{*}!\ldots \tilde{n}_{r}^{*}!} \omega_{1}^{\tilde{n}_{r}^{*}} \omega_{2}^{\tilde{n}_{1}^{*}} \ldots \omega_{r}^{\tilde{n}_{r}^{*}}\right].
$$

Usando la aproximación de Stirling $(\ln N!\approx N \ln N-N)$, las propiedades de la función logaritmo, y el hecho de que $\sum_{i} \tilde{n}_{i}^{*}=N^{*}$, la ecuación anterior se transforma en

$$
S=-k \sum_{i} p_{i} \ln p_{i} \omega_{i}.
$$ (eq:02)

$p_{i}=\tilde{n}_{i}^{*} / N^{*} \omega_{i}$ es la probabilidad por unidad de volumen, o densidad de probabilidad, de que el punto representativo de uno de los sistemas del ensemble se encuentre el la $i$-ésima celda. $p_{i}$ satisface $\sum_{i} p_{i} \omega_{i}=1$.

### El límite al Continuo

La definición de entropía dada por la ecuación {eq}`eq:02` es inconsistente con la naturaleza física de la entropía. Esto se debe a que su valor depende de la forma en que se construye el sistema de celdas. Esto está en desacuerdo con el hecho de que la entropía, como toda vantidad termodinámica, es una propiedad del sistema cuyo valor es independiente de la forma en que se mide o se calcula. Este problema se resuelve considerando un ensemble formado por una cantidad no numerable de sistemas (tal que sus puntos representativos forman una continuidad en el espacio $\Gamma$ ) y tomando el límite al contínuo. Con esto, la ecuación {eq}`eq:02` se convierte en

$$
S=-k \int_{\Omega} \rho(x) \ln \rho(x) d \gamma. 
$$ (eq:03)

$\Omega$ es la región formada por el conjunto de puntos representativos de microestados compatibles con el macroestado. $x$ es un punto del espacio $\Gamma . d \gamma$ es el volumen fase de una vecindad infinitesimal alrededor de $x . \rho(x) d \gamma$ es la probabilidad de que el punto representativo del ensemble se encuentre en una vecindad de volumen $d \gamma$ alrededor de $x$. La densidad de probabilidad $\rho(x)$ está normalizada:

$$
\int_{\Omega} \rho(x) d \gamma=1. 
$$ (eq:04)

La definición de entropía dada por la ecuación {eq}`eq:03` se conoce como la entropía de Gibbs.

## Ensembles Microcanónico y Canónico

La definición de entropía dada por la ecuación {eq}`eq:03` permite conocer la entropía del sistema (macroestado) a partir de la densidad de probabilidad que determina al mesoestado más probable, $(\rho(x))$. Pero así, dicha definición es poco útil, pues rara vez es posible conocer el mesoestado a partir de resultados experimentales. Sin embargo, la segunda ley de la termodinámica provee la información necesaria para conocer este mesoestado más probable a partir de las condiciones macroscópicas de los sistemas del ensemble.

La segunda ley de la termodinámica en la representación de la entropía establece que el estado de equilibrio de un sistema aislado es, de entre todos los estados termodinámicos compatibles con el macroestado, aquel que maximiza la entropía. Por otra parte, cada función de distribución que satisfaga la condición de normalización corresponde a un mesoestado compatible con las condiciones macroscópicas del sistema. Aunque esto no garantiza que el sistema está aislado. Si equiparamos los mesoestados con los estados termodinámicos, la segunda ley nos permite buscar $\rho(x)$ como la densidad de probabilidad que maximiza la ecuación {eq}`eq:03`, sujeta a la condición de normalización -ecuación {eq}`eq:04`, más las condiciones necesarias para garantizar que el ensemble es un sistema aislado.

### Ensemble Microcanónico

Por definición, el ensemble microcanónico está constituido por sistemas en equilibrio y rodeados por paredes rígidas, adiabáticas e impermeables; es decir, están aislados. Todos los sistemas de un ensemble canónico tienen valores constantes e iguales de $U, V$ y $N_{i}$.

Dada la forma en que se construye este ensemble, no es necesaria ninguna condición además de la condición de normalización {eq}`eq:04` para garantizar que el ensemble es un sistema aislado y en equilibrio. Así pues, la densidad de probabilidad de equilibrio es aquella que maximiza la entropía {eq}`eq:03`, sujeta a la condición de normalización {eq}`eq04`. Este problema se resuelve empleando cálculo variacional. Para ello, se define el Lagrangiano:

$$
\Lambda=\int_{\Omega}[\rho(x) \ln \rho(x)-\alpha \rho(x)] d \gamma,
$$

donde $\alpha$ es un multiplicador de Lagrange indeterminado. De acuerdo a la teoría del cálculo variacional, la función $\rho(x)$ que maximiza {eq}`eq:03` sujeta a la restricción {eq}`eq:04` es aquella para la cual la variación de $\Lambda$ se anula:

$$
\delta \Lambda=\int_{\Omega}[\ln \rho(x)+1-\alpha] \delta \rho(x) d \gamma=0.
$$

$\delta \rho(x)$ es la variación de $\rho(x)$, que es arbitraria. En consecuencia, para que $\delta \Delta$ se anule se requiere que el integrando de la ecuación anterior sea igual con cero:

$$
\rho(x) \ln \rho(x)-\alpha \rho(x)=0.
$$

Despejando, podemos encontrar la densidad de probabilidad del ensemble microcanónico.

$$
\rho(x)=C
$$

$C=\exp (\alpha-1)$ es una constante indeterminada. Su valor se encuentra requiriendo que $\rho(x)$ satisfaga la condición de normalización {eq}`eq:04`. Por lo tanto, la densidad de probabilidad de equilibrio del ensemble microcanónico es:

$$
\rho(x)=\frac{1}{\Gamma}. 
$$ (eq:05)

$\Gamma=\int_{\Omega} d \gamma$ es el volumen fase de la región $\Omega$.
El tamaño y forma de la región Omega están determinados por las condiciones macroscópicas de los sistemas del ensemble $\left(U, V, N_{i}\right)$. Es decir $\Gamma=\Gamma\left(U, V, N_{i}\right)$.

Finalmente, sustituyendo {eq}`eq:05` en {eq}`eq:03` se obtiene la ecuación fundamental para cada uno de los sistemas del ensemble microcanónico:

$$
S\left(U, V, N_{i}\right)=k \ln \Omega\left(U, V, N_{i}\right). 
$$ (eq:06)

### Ensemble Canónico

El ensemble canónico está constituido por sistemas con valores constantes e iguales de $V$ y $N_{i}$. Además, todos los sistemas del ensemble están en contacto térmico y en equilibrio con una fuente térmica a temperatura $T$. Como está definido, este ensemble es un sistema en equilibrio termodinámico, pero no necesariamente está aislado. La razón de esto es que todos los sistemas intercambian energía con una fuente térmica que puede ser ajena al ensemble. Para que, a pesar de esto, el ensemble sea un sistema aislado, la fuente térmica debe ser parte del ensemble mismo. Una forma de asegurar lo anterior es considerar que la fuente térmica con que cada sistema del ensemble está en contacto está formada por el resto de sistemas. De esta manera, los intercambios de calor se llevan a cabo al interior del ensemble y se garantiza que se trata de un sistema aislado.

Como se ha visto, para garantizar que el ensemble sea un sistema aislado es necesario pedir explícitamente que la energía total del ensemble permanezca constante. Esta condición se puede escribir como

$$
\int_{\Omega} \epsilon(x) \rho(x) d \gamma=\bar{\epsilon}. 
$$ (eq:07)

En la expresión anterior, $\epsilon(x)$ es la energía de un sistema cuyo punto representativo es $x$ y $\bar{\epsilon}$ es la energía promedio del ensemble (la energía total dividida por el número de sistemas del ensemble).

De acuerdo con la segunda ley de la termodinámica, la densidad de probabilidad de equilibrio del ensemble canónico es aquella que maximiza la entropía {eq}`eq:03`, sujeta a las restricciones {eq}`eq:04` y {eq}`eq:07`. La teoría del cálculo variacional establece que esta densidad de probabilidad es la que optimiza al Lagrangiano $\Lambda$ definido como

$$
\Lambda=\int_{\Omega}[\rho(x) \ln \rho(x)-(\alpha-\beta \epsilon(x)) \rho(x)], d \gamma,
$$

donde $\alpha$ y $\beta$ son multiplicadores de Lagrange. La variación de $\Lambda$ es

$$
\delta \Lambda=\int_{\Omega}[\ln \rho(x)+1-\alpha+\beta \epsilon(x)] \delta \rho(x) d \gamma.
$$

La función $\rho(x)$ que optimiza $\Lambda$ es aquella para la cual $\delta \Lambda=0$. Por otra parte, dado que $\delta \rho(x)$ es una variación arbitraria, $\delta \Lambda=0$ sólo si $\rho(x)+1-\alpha-\beta \epsilon(x)=0$. Despejando $\rho(x)$ tenemos que

$$
\rho(x)=\frac{1}{Z} e^{-\beta \epsilon(x)}. 
$$ (eq:08)

$Z=\exp (\alpha-1)$ y $\beta$ son constantes indeterminadas. El valor de $Z$, conocida como la función de partición, se determina usando la condición de normalización {eq}`eq:04`:

$$
Z=\int_{\Omega} e^{-\beta \epsilon(x)} d \gamma. 
$$ (eq:09)

En principio, debería ser posible determinar el valor de $\beta$ a partir de la restricción {eq}`eq:07`. Sin embargo, el álgebra es bastante complicada. Alternativamente, podemos sustituir la densidad de probabilidad dada por la ecuación {eq}`eq0:8` en la definición de entropía {eq}`eq:03`:

$$
S=k \beta \bar{\epsilon}+k \ln Z,
$$ (eq:10)

e imponer la relación termodinámica $1 / T=(\partial S / \partial \bar{\epsilon})_{V, N_{i}}$, para obtener

$$
\beta=\frac{1}{k T}. 
$$ (eq:11)

En resumen, la densidad de probabilidad de equilibrio del ensemble canónico está dada por la ecuación {eq}`eq:08`, con $Z$ y $\beta$ respectivamente dadas por las ecuaciones {eq}`eq:09` y {eq}`eq:11`.

Puesto que en este caso las variables independientes son $T, V$ y $N_{i}$, que corresponden a la representación de la energía libre de Helmholtz, la ecuación fundamental se obtiene a partir de la ecuación {eq}`eq:10` y la definición de $F$ como

$$
F\left(T, V, N_{i}\right)=-k T \ln Z\left(T, V, N_{i}\right). 
$$ (eq:12)

## Física Estadística del Gas Ideal

### Ensemble Canónico

Por definición, el gas ideal es un sistema cuyas partículas no interactúan entre sí y sólo tienen componente de energía cinética. Por ende, el Hamiltoniano de un gas ideal con $N$ partículas es de la forma

$$
H=\sum_{i=1}^{3 N} \frac{p_{i}^{2}}{2 m}.
$$

Sea pues un gas ideal contenido en un recipiente cúbico de lado $V^{1 / 3}$. Su función de partición se calcula como

\begin{aligned*}
Z= & \int_{-\infty}^{\infty} \ldots \int_{-\infty}^{\infty} d x_{1} \ldots d x_{3 N} \\
& \int_{0}^{V^{1 / 3}} \ldots \int_{0}^{V^{1 / 3}} e^{-\beta / 2 m\left(p_{1}^{2}+\ldots p_{3 N}^{2}\right)} d p_{1} \ldots d p_{3 N}.
\end{aligned*}

Los límites de integración de los momentos $p_{i}$ son de $-\infty$ a $\infty$ porque los sistemas del ensemble están en contacto con una fuente térmica. En consecuencia, su energía presenta fluctuaciones, pudiendo estas ser incluso de tamaño infinito. Las integrales sobre las variables $x_{i}$ se pueden separar en $3 N$ integrales de la forma $\int_{0}^{V^{1 / 3}} d x=V^{1 / 3}$. Las integrales sobre las variable $p_{i}$ también se pueden separar. En esta caso, resultan $3 N$ integrales de la forma $\int_{-\infty}^{\infty} e^{\beta p_{i}^{2} / 2 m} d p_{i}=\sqrt{x \pi m / \beta}$.

De los resultados anteriores tenemos entonces que la función de partición del gas ideal es

$$
Z=\left[V(2 \pi m k T)^{3 / 2}\right]^{N}. 
$$ (eq:13)

A partir de esta función de partición se puede encontrar la ecuación fundamental del sistema como

\begin{align*}
F(T, V, N) & =-k T \ln Z(T, V, N) \\
& =-k T N\left[\ln V+\frac{3}{2} \ln (2 \pi m k T)\right] .
\end{align*} (eq:14)

Las ecuaciones de estado resultantes de la anteror ecuación fundamental son

\begin{align*}
S &=-\left(\frac{\partial F}{\partial T}\right)_{V, N}=-\frac{F}{T}+\frac{3}{2} N k. \\
P &=-\left(\frac{\partial F}{\partial V}\right)_{T, N}=\frac{k T N}{V}. \\
\mu&=\left(\frac{\partial F}{\partial N}\right)_{T, V}=-k T\left[\ln V+\frac{3}{2} \ln (2 \pi m k T)\right]. 
\end{align*} (eq:15)


La ecuación (2.16) es una de las ecuaciones de estado del gas ideal. Por otra parte, de la ecuación (2.15) y de la definición de la energía libre de Helmholtz se sigue que
$$
\bar{\epsilon}=F+T S=\frac{3}{2} N k T. \tag{2.18}
$$
Esta ecuación es otra de las ecuaciones de estado del gas ideal. La ecuación (2.17) no corresponde a la tercera ecuación de estado del sistema. Sin embargo, este problema se estudiará posteriormente.

En conclusión, a sido posible recuperar al menos dos de las ecuaciones de estado del gas ideal, usando el formalismo del ensemble canónico. Esto en cierta medida valida las suposiciones hechas en la construcción de esta teoría. Particularmente, la hipótesis de igualdad de probabilidad a priori y la definición de entropía.

### Ensemble microcanónico

Considere un gas formado por $N$ partículas, contenido en un recipiente de volumen fijo $V$ y rodeado de paredes adiabáticas e impermeables, de tal forma que tiene una energía interna en el intervalo $[E-\delta E, E] (\delta E \ll E)$.

El hamiltoniano de este sistema es:
$$
H=\sum_{i=1}^{3 N} \frac{p_{i}^{2}}{2 m}.
$$

De aquí se sigue que la restricción en la energía del gas implica que la proyección de la región $\Omega$ en el espacio de momentos es un cascarón hiperesférico de $3 N$ dimensiones, radio externo $R=\sqrt{2 m E}$ y espesor $\delta E=\sqrt{2 m E}-\sqrt{2 m(E-\delta E)}$. Por su parte, la proyección de la región $\Omega$ en el espacio de configuración es el producto cartesiano de $N$ veces el volumen que contiene al gas.

En hiperesferas de dimensión muy grande, el volumen se concentra en su mayor parte cerca de la superficie. Luego, el volumen del cascarón se puede aproximar por el volumen de la esfera completa. El volumen de una hiperesfera de $f$ dimensiones y radio $R$ está dado por
$$
V_{f}(R)=\frac{\pi^{f / 2}}{(f / 2)!} R^{f},
$$
de donde se sigue que el volumen de la proyección de $\Omega$ en el espacio de momentos es
$$
\frac{(2 \pi m E)^{3 N / 2}}{(3 N / 2)!}.
$$
Esto, más el hecho de que el volumen de la proyección de $\Omega$ en el espacio de configuración es $V^{N}$ nos da el siguiente valor para el volumen fase ( $\Gamma$ ) de la región $\Omega$,
$$
\Gamma=\frac{\left(V(2 \pi m E)^{3 N / 2}\right)^{N}}{(3 N / 2)!} .
$$
Del resultado anterior y la fórmula para la ecuación fundamental del ensemble microcanónico {Eq}`eq06`, tenemos que la ecuación fundamental del gas ideal en condiciones de energía $E$, volumen $V$ y número de partículas $N$ constantes es
$$
S=k N\left\{\ln V\left[\frac{4 \pi m E}{3 N}\right]^{3 / 2}+\frac{3}{2}\right\}. \tag{2.19}
$$

Las ecuaciones de estado derivadas de la anterior ecuación fundamental son
$$
\begin{align*}
\frac{1}{T} & =\frac{3}{2} \frac{k N}{E}, \tag{2.20}\\
\frac{P}{T} & =\frac{k N}{V}. \tag{2.21},
\end{align*}
$$
y
$$
\frac{\mu}{T}=-k\left[\ln V+\frac{3}{2} \ln \left[\frac{4 \pi m E}{3 N}\right]\right]. 
$$
Estas ecuaciones de estado son completamente compatibles con las ecuaciones de estado derivadas con el ensemble microcanónico:{eq}`eq15`-{eq}`eq17`.

## Fluctuaciones termodinámicas

En el ensemble microcanónico, el valor promedio de cualquier cantidad física $f(x)$, se calcula como
$$
\bar{f}=\int_{\Omega} f(x) \rho(x) d \gamma,
$$
con $\rho(x)$ la densidad de probabilidad dada por la ecuación (2.8). A partir del resultado anterior y la expresión para la función de partición: ecuación (2.9), se sigue para la energía promedio del gas que
$$
\bar{\epsilon}=-\frac{\partial \ln Z}{\partial \beta}. 
$$

De manera análoga se demuestra que
$$
\overline{\Delta \epsilon^{2}}=\frac{\partial^{2} \ln Z}{\partial \beta^{2}}. 
$$

De las dos ecuaciones, y dado el caracter extensivo de la función de partición $Z$ y el caracter intensivo de $\beta=1 / k T$, se concluye que la magnitud relativa de las fluctuaciones en la energía obedece la siguiente relación
$$
\frac{\bar{\epsilon}}{\sqrt{\overline{\Delta \epsilon^{2}}}} \approx \frac{1}{\sqrt{N}}.
$$(eq:eq25)

## Paradoja de Gibbs y otros problemas

En la ecuación fundamental del gas ideal derivada con el ensemble canónico {eq}`eq13` en la representación de la energía libre de Helmholtz, como en la derivada con el ensemble microcanónico en la representación de la entropía (2.19), existen un par de problemas. En primer lugar, las unidades son incorrectas. En ambos casos, el argumento de la función logaritmo debe de ser adimensional. Este problema tiene su origen en la derivación original de la entropía de un ensemble (2.1). En dicha derivación se toma el volumen fase de una celda de la región $\Omega$ como medida del número de posiciones distintas que un punto representativo puede tomar dentro de dicha celda. Por esta razón, aparecen multiplicados los volúmenes de las celdas elevados a una potencia igual al número de ocupación de las mismas. Esto de la a la entropía del ensemble unidades de Joule soble Kelvin, por unidades de volumen fase, lo cual es incorrecto. Este problema se soluciona con argumentos cuánticos. Debido a las relaciones de incertidumbre de Heisenberg, es imposible localizar exactamente la posición de el punto relativo del sistema en el espacio fase. A lo más, se puede determinar una vecindad de volumen $h^{3 N}$, con $N$ el número de partículas del gas. Bajo estas consideraciones, el número de posiciones distintas que un punto representativo puede tomar en el interior de una celda de del espacio $\Gamma$ está dado por el volumen de la misma, dividido por $h^{3 N}$. Tomando esto en cuenta, para evitar problemas con las unidades, hay que corregir las ecuaciones fundamentales derivadas con los ensembles microcanónico y canónico de la siguiente forma, respectivamente:
\begin{aligned}
S(U, V, N) & =k \ln \frac{\Gamma}{h^{3 N}} \\
& =k N\left\{\ln V\left[\frac{4 \pi m E}{3 N h^{2}}\right]^{3 / 2}+\frac{3}{2}\right\},
\end{aligned}
y
\begin{aligned}
F(T, V, N) & =-k T \ln \frac{Z}{h^{3 N}} \\
& =-k T N\left[\ln V+\frac{3}{2} \ln \left(\frac{2 \pi m k T}{h^{2}}\right)\right].
\end{aligned}
Las fórmulas anteriores tienen las unidades correctas, pero aún presentan un problema. Tanto la entropía como la energía libre de Helmholtz son cantidades extensivas. Sin embargo, dado que en las ecuaciones anteriores aparece el logaritmo del volumen multiplicando a $N$, ellas no representan cantidades extensivas. Este problema se conoce como paradoja de Gibbs.

La paradoja de Gibbs se resuelve empleando argumentos cuánticos. En particular el hecho de que en realidad las partículas que forman un gas son indistinguibles, lo cual no se tomó en cuenta al contar el número de microestados compatibles con un mesoestado. Por tal razón, la probabilidad de un mesoestado está sobreestimada por un factor $N$ !. Después de corregirlas, las ecuaciones fundamentales obtenidas con los ensembles microcanónico y canónico quedan finalmente como
\begin{align*}
S(U, V, N) & =k \ln \frac{\Gamma}{h^{3 N} N!} \\
& =k N\left\{\ln \frac{V}{N} \left[\frac{4 \pi m E}{3 N h^{2}}\right]^{3 / 2}+\frac{5}{2}\right\}, \tag{2.26}
\end{align*}
y
\begin{align*}
F(T, V, N) & =-k T \ln \frac{Z}{h^{3 N} N!} \\
& =-k T N\left[\ln \frac{V}{N}+\frac{3}{2} \ln \left(\frac{2 \pi m k T}{h^{2}}\right)+1\right]. \tag{2.27}
\end{align*}

## Teorema de equipartición de la energía

Considere un sistema cuya dinámica está determinada por un Hamiltoniano de la forma
$$
H=K+V=\sum_{i=1}^{f} A_{i} p_{i}^{2}+\sum_{i, j=1}^{f} B_{i j} q_{i} q_{j}.
$$
$f$ es el número de grados de libertad del sistema, $p_{i}$ son los momentos generalizados, $q_{i}$ las coordenadas generalizadas, y $A_{i}$ y $B_{i j}$ son constantes arbitrarias. Tanto la componente de energía cinética como la de energía potencial de este Hamiltoniano es homogéneas de segundo orden los los momentos y en las coordenadas generalizadas, respectivamente:
\begin{align*}
& \sum_{j=1}^{f} p_{j} \frac{\partial K}{\partial p_{j}}=2 \sum_{j=1}^{f} A_{j} p_{j}^{2}=2 K,  \tag{2.28}\\
& \sum_{j=1}^{f} q_{j} \frac{\partial V}{\partial q_{j}}=2 \sum_{i, j=1}^{f} B_{i j} q_{i} q_{j}=2 V. \tag{2.29}
\end{align*}

Por otra parte, usando el ensemble canónico tenemos que
$$
\overline{p_{j} \frac{\partial K}{\partial p_{j}}}=\overline{p_{j} \frac{\partial H}{\partial p_{j}}}=\frac{1}{Z} \int e^{-\beta H} p_{j} \frac{\partial H}{\partial p_{j}} d \gamma. \tag{2.30}
$$(eq:eq30)
La integral se lleva a cabo sobre todas las coordenadas y todos los momentos generalizados, incluyendo $p_{j}$. Separando la integral sobre $p_{j}$ y llevándola a cabo por partes tenemos que
\begin{align*}
\int_{-\infty}^{\infty} e^{-\beta H} \frac{\partial H}{\partial p_{j}} p_{j} d p_{j} &=-\frac{1}{\beta} \int_{-\infty}^{\infty} \frac{\partial e^{-\beta H}}{\partial p_{j}} p_{j} d p_{j}, \\
&=-\left.\frac{e^{-\beta H} p_{j}}{\beta}\right|_{-\infty} ^{\infty}+\frac{1}{\beta} \int_{-\infty}^{\infty} e^{-\beta H} d p_{j}. 
\end{align*}(eq:eq32)
El primer término se cancela en ambos límites dada la dependencia del hamiltoniano en $p_{j}$.
Así pues, reinsertando de la integral {Eq}`eq31` en {Eq}`eq32`

$$
\overline{p_{j} \frac{\partial K}{\partial p_{j}}}=\frac{1}{\beta} \int \frac{e^{-\beta H}}{Z} d \gamma=k T. 
$$(eq:eq32)

Finalmente, de las ecuaciones {eq}`eq32` y {eq}`eq28` se sigue que
$$
\bar{K}=\frac{f}{2} k T
$$
De manera análoga se demuestra para la energía potencial que
$$
\bar{V}=\frac{f}{2} k T. 
$$
Las dos últimas ecuaciones constituyen el teorema de equipartición de la energía, el cual nos dice que si tanto la energía cinética como la energía potencial son respectivamente funciones homogéneas de segundo orden en las coordenadas y los momentos generalizados, entonces ambas se reparten equitativamente entre todos los grados de libertad.

El teorema de equipartición de la energía también puede demostrarse en ensemble microcanónico.

## El sólido cristalino clásico

Una aplicación interesante del teorema de equipartición de la energía es el sólido cristalino. El Hamiltoniano de este sistema se puede escribir en general como
$$
H=\sum_{i=1}^{3 N} \frac{p_{i}^{2}}{2 m}+V\left(q_{1} \cdots q_{3 N}\right).
$$
$N$ es el número de átomos del sólido, $p_{i}$ representa una coordenada de momento, $q_{i}$ representa una coordenada de posición y $V$ es la energía potencial elástica del sólido. Las coordenadas $q_{i}$ están referidas a las posiciones de equilibrio de las partículas, donde toman valor cero. Por convención, $V(0 \cdots 0)=0$, además de que debido a que el equilibrio mecánico se alcanza cuando $q_{i}=0(\forall i=1 \cdots 3 N)$, se cumple que $\partial V /\left.\partial q_{i}\right|_{\left\{q_{j}=0\right\}} (\forall i 1 \cdots 3 N)$.

Los átomos de un sólido paramagnético están fuertemente unidos entre sí, por lo que se alejan muy poco de su posición de equilibrio. Eso significa que $q_{j} \simeq 0,(\forall i 1 \cdots 3 N)$. En consecuencia, es factible expandir $V\left(q_{1} \cdots q_{3 N}\right)$ en serie de Taylor y cortar a segundo orden:
$$
V\left(q_{1} \cdots q_{3 N}\right) \simeq \sum_{i, j=1}^{3 N} \frac{\partial^{2} V}{\partial q_{i} \partial q_{j}} q_{i} q_{j}.
$$
Esta aproximación se llama la aproximación armónica.

Del resultado anterior vemos que si es válida la aproximación armónica, el Hamiltoniano del sólido cristalino satisface las condiciones del teorema de equipartición de la energía. En consecuencia,
$$
U=3 N k T.
$$
De donde el calor específico molar a volumen constante del sólido cristalino es
$$
c_{P}^{*}=3 R.
$$
Este resultado se conoce como Ley de Dulong y Petit. Funciona bastante bien a altas temperaturas, sin embargo en el límite de temperaturas bajas falla, pues el calor específico de los sólidos cristalinos disminuye como $T^{3}$. De hecho, la Ley de Dulong y Petit contradice la tercera ley de la termodinámica, la cual predice que el calor específico de cualquier sistema tiende a cero cuando la temperatura tiende a cero.

