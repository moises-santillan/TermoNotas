# Capítulo 3: Física Estadística Cuántica

## La matriz de densidad

Desde el punto de vista de la mecánica cuántica, un sistema termodinámico nunca está completamente aislado. Incluso un sistema rodeado por paredes adiabáticas, rígidas e impermeables interactúa con las paredes mismas. En tal sentido, siempre es posible escribir el operador Hamiltoniano de un sistema termodinámico de la siguiente forma,

$$
\hat{H}_{o}\left(x_{i}\right)+\hat{H}_{i}\left(x_{i}, q_{j}\right)
$$

$\hat{H}_{o}$ es el Hamiltoniano que da cuenta de la dinámica interna del sistema mientras que $\hat{H}_{i}$ representa la interacción del sistema con el medio. las variables $x_{i}$ son las coordenadas generalizadas de los elementos que componen el sistema, en tanto que las variables $q_{j}$ son las coordenadas generalizadas asociadas al medio.

Bajo la suposición de que $\hat{H}_{i}$ se puede tratar como una perturbación, la función de onda del sistema $\left(\Psi\left(x_{i}, q_{j}\right)\right)$ se puede escribir como una combinación lineal de las eigenfunciones de $\hat{H}_{o}\left(\phi_{n}\left(x_{i}\right)\right)$ :

$$
\Psi\left(x_{i}, q_{j}\right)=\sum_{n} a_{n}\left(q_{j}\right) \phi_{n}\left(x_{i}\right)
$$

En virtud de lo anterior, dado un operador $\hat{f}\left(x_{i}\right)$ asociado a un observable del sistema, su valor esperado queda como

$$
\bar{f}=\int \Psi^{*}\left(x_{i}, q_{j}\right) \hat{f}\left(x_{i}\right) \Psi\left(x_{i}, q_{j}\right) d x_{i} d q_{j}=\sum_{n, m} f_{n m} w_{m n}
$$

donde

$$
f_{n m}=\int \phi_{n}^{*}\left(x_{i}\right) \hat{f}\left(x_{i}\right) \phi_{m}\left(x_{i}\right) d x_{i}
$$

mientras que

$$
w_{n m}=\int a_{m}\left(q_{j}\right) a_{n}^{*}\left(q_{j}\right)
$$

$w_{n m}$ recibe el nombre de matriz de densidad. Los valores de las entradas de esta matriz están determinados por las interacciones del sistema con el medio. Dado que la traza de una matriz es un invariante, el valor esperado del operador $\hat{f}$ también se puede escribir como

$$
\bar{f}=\operatorname{tr}(\underline{\underline{f} \underline{\underline{w}}})
$$

Sin pérdida de generalidad podemos suponer que $\Psi\left(x_{i}, q_{j}\right)$ está normalizada y que las funciones $\phi_{n}\left(x_{i}\right)$ forman un conjunto ortonormal. De acuerdo con esto, la probabilidad $p_{n}$ de que al hacer una medición el estado del sistema sea $\phi_{n}$ está dada por

$$
p_{n}=\int a_{n}^{*}\left(q_{j}\right) a_{n}\left(q_{j}\right) d q_{j}=w_{n n}
$$

En otras palabras, el conjunto de estados accesibles al sistema está determinado por su dinámica interna, en tanto que la probabilidad de que el sistema esté en un estado u otro depende de el tipo de interacción con el medio.

## Ensemble cuántico

Un ensemble estadístico cuántico está conformado por un conjunto muy grande de copias del sistema bajo estudio, todas ellas gobernadas por el mismo Hamiltoniano $\left(\hat{H}_{o}\left(x_{i}\right)\right)$, sujetos a las mismas condiciones externas $\left(\hat{H}_{i}\left(x_{i}, q_{j}\right)\right)$ y en equilibrio termodinámico. Esto significa que todos los miembros del ensemble tienen el mismo conjunto de estados cuánticos accesibles ( $\phi_{n}\left(x_{i}\right)$ ), así como la misma probabilidad $p_{n}$ de que, al hacer una medición, el sistema se encuentre en el estado $\phi_{n}$.

## Definición de Entropía

### Microestado del ensemble

El microestado del ensemble está determinado por el conjunto de microestados de cada uno de los sistemas del ensemble. De hecho, la función de estado del ensemble puede construirse como el producto de las funciones de estado de cada uno de los sistemas que lo componen. En este caso, no hay que preocuparse por la indistinguibilidad puesto que, al ser macroscópicos, los sistemas que conforman el ensemble son todos indistinguibles entre sí.

### Hipótesis de igualdad de probabilidad a priori

Todos los microestados del ensemble compatibles con las restricciones termodinámicas son igualmente probables.

### Mesoestado cuántico

Tomemos un ensemble con $N^{*}$ sistemas, construido de acuerdo a la definición de la sección anterior. El mesoestado del ensemble está determinado por el conjunto $\left\{\tilde{n}_{i}\right\}$, donde $\tilde{n}_{i}$ es el número de sistemas del ensemble cuyo estado es $\phi_{i}$.

### Probabilidad de un mesoestado

Dada la hipótesis de igualdad de probabilidad a priori, la probabilidad de un mesoestado es proporcional al número de microestados compatibles con él, i.e.

$$
\frac{N^{*}!}{\tilde{n}_{1}!\tilde{n}_{2}!\cdots}
$$

### Entropía

De todos los mesoestados compatibles con las restricciones termodinámicas, el que posee la probabilidad máxima es el que caracteriza el estado macroscópico de equilibrio del ensemble.

Por otra parte, si el ensemble es un sistema termodinámico aislado, su estado de equilibrio es aquel que posee la entropía máxima.

La anterior similitud, junto con el hecho de que la entropía es aditiva, en tanto que la probabilidad es multiplicativa nos conduce, mediante un razonamiento heurístico, a definir la entropía del ensemble ( $S^{*}$ ) como proporcional al logaritmo del mesoestado más probable:

$$
\begin{equation*}
S^{*}=k_{B} \ln \frac{N^{*}!}{\tilde{n}_{1}^{*}!\tilde{n}_{2}^{*}!\cdots} \tag{3.1}
\end{equation*}
$$

donde $\left\{\tilde{n}_{i}^{*}\right\}$ es el conjunto que caracteriza al mesoestado más probable.

Dado que todos los sistemas del ensemble son idénticos, la entropía ( $S$ ) de cada uno de ellos se puede calcular como

$$
\begin{equation*}
S=\frac{S^{*}}{N} \tag{3.2}
\end{equation*}
$$

A partir de las ecuaciones (3.1) y (3.2) y haciendo uso de la aproximación de Stirling $(\ln N!=N \ln N-N)$, se llega a la siguiente expreción para la entropía de cada sistema del ensemble:

$$
\begin{equation*}
S=-k_{B} \sum_{n} p_{n} \ln p_{n} \tag{3.3}
\end{equation*}
$$

donde $p_{n}=\frac{\tilde{n}_{n}^{*}}{N^{*}}$ y la sumatoria se lleva a cabo sobre todos los estados accesibles a cada uno de los sistemas del ensemble. De la definición, $p_{n}$ se puede identificar con la probabilidad calculada a partir de la densidad de probabilidad. Sin embargo, cualquier intento de calcularla a partir de primeros principios es imposible en la práctica, dado que, al tratar con sistemas macroscópicos, el número de grados de libertad es del orden de $10^{24}$.

## Ensembles microcanónico y canónico

Como se menciona en la sección anterior, es prácticamente imposible calcular la entropía de un sistema a partir de la definición (3.3) si se quiere encontrar las probabilidades $p_{n}$ resolviendo la ecuación de Scrödinger del sistema y sus alrededores.

Es posible resolver este problema usando la segunda ley de la termodinámica. Si podemos asegurar que el ensemble es un sistema termodinámico aislado en equilibrio, entonces la distribución de probabilidades $\left\{p_{n}\right\}$ será aquella que maximize la entropía. En otras palabras, en lugar de calcular las probabilidades $p_{n}$ (estado mesoscópico) a partir de la dinámica microscópica, éstas se calculan a partir de las condiciones macroscópicas y de la segunda ley de la termodinámica. A continuación un par de ejemplos.

### Ensemble microcanónico

Por definición, el ensemble canónico está formado por un conjunto muy grande de sistemas termodinámicos, todos ellos gobernados por el mismo hamiltoniano, en equilibrio termodinámico y sujetos a las restricciones macroscópicas de energía $(E)$, volumen $(V)$ y número de partículas $(N)$ constantes. Es decir, todos los sistemas del ensemble microcanónico están termodinámicamente aislados.

Dado lo anterior, el único requisito adicional para garantizar que el ensemble es un sistema termodinámico aislado y en equilibrio es que el número de sistemas permanezca constante. Esto es equivalente a pedir que:

$$
\begin{equation*}
\sum_{n} p_{n}=1 \tag{3.4}
\end{equation*}
$$

En otras palabras, la distribución de probabilidades del ensemble microcanónico es aquella que maximiza la entropía (3.3), sujeta a la condición de normalización (3.4). Usando la técnica de los multiplicadores de Lagrange se encuentra que:

$$
\begin{equation*}
p_{n}=\frac{1}{W} \tag{3.5}
\end{equation*}
$$

donde $W$ es el número total de estados microscópicos accesibles al sistema.
De las ecuaciones (3.3) y (3.5) se deduce la siguiente expresión para la entropía en el ensemble microcanónico:

$$
\begin{equation*}
S=k_{B} \ln W \tag{3.6}
\end{equation*}
$$

### Ensemble canónico

Por definición, el ensemble microcanónico está formado por un conjunto muy grande de sistemas termodinámicos, todos ellos gobernados por el mismo hamiltoniano, en equilibrio termodinámico y sujetos a las restricciones macroscópicas de temperatura $(T)$, volumen $(V)$ y número de partículas $(N)$ constantes. Los
sistemas del ensemble canónico no están termodinámicamente aislados, sino que se encuentran en contacto con una fuente térmica a temperatura $T$.

Dado lo anterior, los requisito necesarios para garantizar que el ensemble es un sistema termodinámico aislado y en equilibrio son que el número de sistemas y la energía total del ensemble permanezcan constantes. La primera condición es equivalente a pedir que:

$$
\begin{equation*}
\sum_{n} p_{n}=1 . \tag{3.7}
\end{equation*}
$$

La condición de energía total del ensemble constante se puede expresar como:

$$
\begin{equation*}
\sum_{n} E_{n} p_{n}=\bar{E} \tag{3.8}
\end{equation*}
$$

donde $E_{n}$ es la energía del sistema cuando su estado cuántico es $\phi_{n}$.
En otras palabras, la distribución de probabilidades del ensemble microcanónico es aquella que maximiza la entropía (3.3), sujeta a las condiciones de normalización (3.7) y de energía constante (3.8). Usando la técnica de los multiplicadores de Lagrange así como la relación entre entropía y temperatura ( $1 / T=\partial S / \partial \bar{E}$ ) se encuentra que:

$$
\begin{equation*}
p_{n}=\frac{\exp \left(-E_{n} / k_{B} T\right)}{Z} \tag{3.9}
\end{equation*}
$$

donde $Z$ es la función de partición definida por:

$$
\begin{equation*}
Z=\sum_{n} \exp \left(-E_{n} / k_{B} T\right) \tag{3.10}
\end{equation*}
$$

A partir de la ecuación (3.9) y la definición de energía libre de Helmholtz, la ecuación fundamental en el ensemble canónico queda como:

$$
\begin{equation*}
F=-k_{B} T \ln Z \tag{3.11}
\end{equation*}
$$

## El sólido paramagnético

Considere un sistema formado por $N$ dipolos magnéticos fijos en el espacio los cuales, en la presencia de un campo magnético externo $\vec{B}$, pueden alinearse paralela o antiparalelamente a $\vec{B}$. La energía de interacción entre un dipolo magnético y $\vec{B}$ está dada por $-\vec{\mu} \cdot \vec{B}$, donde $\vec{\mu}$ es el momento magnético del dipolo.

### Ensemble microcanónico

Para poder emplear en ensemble microcanónico necesitamos pedir que el sistema de $N$ dipolos se mantenga a energía constante $E$. No es necesario pedir que el volumen permanezca constante pues, al estar los dipolos fijos en el espacio, esta condición se satisface automáticamente. Tampoco es necesario hacer explícita la constancia de $N$, pues está implícita en la definición del sistema.

La energía del sistema está dada por:

$$
\begin{equation*}
E=\mu B((N-n)-n)=\mu B(N-2 n) \tag{3.12}
\end{equation*}
$$

donde $n$ es el número de dipolos paralelos a $\vec{B}, B=|\vec{B}|$ y $\mu=|\mu|$. El número, $W$, de microestados del sistema compatibles con la restricción de energía constante es igual al número de formas en que los $N$ dipolos se pueden arreglar estando $n$ de ellos paralelos a $\vec{B}$ y $(N-n)$ antiparalelos; es decir:

$$
\begin{equation*}
W=\frac{N!}{n!(N-n)!} \tag{3.13}
\end{equation*}
$$

A partir de las ecuaciones (3.6), la entropía del sistema se puede calcular, usando la aproximación de Stirling, como:

$$
\begin{equation*}
S=k_{B} \ln W \simeq k_{B}\left[N \ln \frac{N}{N-n}-n \ln \frac{n}{N-n}\right] \tag{3.14}
\end{equation*}
$$

A partir de la relación $1 / T=\partial S / \partial E$, así como de las ecuaciones (3.12) y (3.14) se obtiene la siguiente relación entre la energía del sistema y su temperatura:

$$
\begin{equation*}
E=-N \mu B \tanh \frac{\mu B}{k_{B} T} \tag{3.15}
\end{equation*}
$$

### Ensemble canónico

En el ensemble canónico el sistema está en equilibrio con una fuente de temperatura $T$ y su energía fluctúa alrededor del valor medio. Así, lad $2^{N}$ combinaciones de bipolos paralelos y antiparalelos a $\vec{B}$ son microestados compatibles con las restricciones macroscópicas de los sistemas del ensemble.

De la ecuación (3.11), la función de partición del sistema se calcula como:

$$
\begin{equation*}
Z=\sum_{n_{1}, n_{2} \cdots n_{N}=-1,1} \exp \left(\frac{\left(n_{1}+n_{2} \cdots+n_{N}\right) \mu B}{k_{B} T}\right)=\left(\mathrm{e}^{\mu B / k_{B} T}+\mathrm{e}^{-\mu B / k_{B} T}\right)^{N} . \tag{3.16}
\end{equation*}
$$

Finalmente, la energía promedio del sistema resulta ser:

$$
\begin{equation*}
\bar{E}=-\frac{1}{Z} \frac{\partial Z}{\partial \beta}=-N \mu B \tanh \frac{\mu B}{k_{B} T} \tag{3.17}
\end{equation*}
$$

$\operatorname{con} \beta=1 / k_{B} T$.

### Ensemble gran canónico

Por definición, este ensemble está formado por sistemas gobernados por el mismo Hamiltoniano, que se encuentran en equilibrio termodinámico con una fuente de temperatura $T$ y una fuente de potencial químico $\mu$, y están sujetos a la restricción de volumen $V$ constante.

Por como está constituido, para garantizar que el ensemble gran canónico es un sistema termodinámico aislado, es necesario pedir explícitamente que el número de sistemas del ensemble, la energía y el número de partículas del mismo sean constantes. Es decir:

$$
\begin{gather*}
\sum_{n} p_{n}=1  \tag{3.18}\\
\sum_{n} E_{n} p_{n}=\bar{E} \tag{3.19}
\end{gather*}
$$

y

$$
\begin{equation*}
\sum_{n} N_{n} p_{n}=\bar{N} \tag{3.20}
\end{equation*}
$$

donde $E_{n}, N_{n}$ y $p_{n}$ son respectivamente la energía, el número de partículas y la probabilidad asociadas al estado $\phi_{n}$, accesible al sistema dadas las restricciones macroscópicas.

En otras palabras, la distribución de probabilidades $\left\{p_{n}\right\}$ del ensemble microcanónico es aquella que maximiza la entropía (3.3), sujeta a las restricciones (3.18)-(3.20). Usando la técnica de los multiplicadores de Lagrange, así como las relaciones $1 / T=\partial S / \partial \bar{E}$ y $\mu / T=-\partial S / \partial \bar{N}$ se obtiene que:

$$
\begin{equation*}
p_{n}=\frac{\mathrm{e}^{-\beta\left(E_{n}-\mu N_{n}\right)}}{\mathcal{Z}} \tag{3.21}
\end{equation*}
$$

con $\mathcal{Z}$ la gran función de partición, definida como:

$$
\begin{equation*}
\mathcal{Z}=\sum_{n} \mathrm{e}^{-\beta\left(E_{n}-\mu N_{n}\right)} \tag{3.22}
\end{equation*}
$$

El potencial termodinámico asociado con el ensemble gran canónico es el llamado gran potencial termodinámico, el cual está definido por:

$$
\begin{equation*}
\Omega(T, V, \mu)=U(T, V, \mu)-T S(T, V, \mu)-\mu N(T, V, \mu) \tag{3.23}
\end{equation*}
$$

De las ecuaciones (3.3), (3.21)-(3.23), se deduce que:

$$
\begin{equation*}
\Omega(T, V, \mu)=k_{B} T \ln \mathcal{Z}(T, V, \mu) \tag{3.24}
\end{equation*}
$$

Finalmente, de las ecuaciones (3.19)-(3.22) se sigue que:

$$
\begin{equation*}
\bar{E}=-\frac{\partial \ln \mathcal{Z}}{\partial \beta} \tag{3.25}
\end{equation*}
$$

y

$$
\begin{equation*}
\bar{N}=k_{B} T \frac{\partial \ln \mathcal{Z}}{\partial \mu} \tag{3.26}
\end{equation*}
$$

## Estadísticas de Bose-Einstein y Fermi-Dirac

### Ecuación de onda del gas ideal cuántico

Considere un gas formado por $N$ partículas ideénticas e indestinguibles que no interactúan entre sí. Todas las partículas del gas obedecen el mismo Hamiltoniano, $H^{(1)}(x)$. Sean $\psi_{n}(x)$ y $\varepsilon_{n}$ las eigenfunciones y los eigenvalores de $H^{(1)}(x)$, respectvamente. Es decir, $H^{(1)} \psi_{n}=\varepsilon_{n} \psi_{n}$. Puesto que las partículas del gas no interactúan entre sí (el gas es ideal), el Hamiltoniano del gas es:

$$
\begin{equation*}
H\left(x_{1}, x_{2} \cdots x_{N}\right)=H^{(1)}\left(x_{1}\right)+H^{(1)}\left(x_{2}\right) \cdots+H^{(1)}\left(x_{n}\right) \tag{3.27}
\end{equation*}
$$

Por otra parte, la energía total del gas (el eigenvalor de $H\left(x_{1}, x_{2} \cdots x_{N}\right)$ ) resulta ser:

$$
\begin{equation*}
E_{n_{1}, n_{2}, \cdots n_{N}}=\varepsilon_{n_{1}}+\varepsilon_{n_{2}} \cdots+\varepsilon_{n_{N}}, \tag{3.28}
\end{equation*}
$$

donde el ídices $n_{i}(i=1,2 \cdots N)$ determina el estado $\psi_{n_{i}}$ de la $i$-ésima partícula del gas. Sólo falta construir la función de estado del gas, $\Psi_{n_{1}, n_{2}, \cdots n_{N}}\left(x_{1}, x_{2} \cdots x_{N}\right)$, a partir de las funciones de estado individuales $\psi_{n_{i}}\left(x_{i}\right)$. Por ser solución de la ecuación de Scrödinger, esta funcón debe satisfacer que:

$$
\begin{equation*}
H\left(x_{1}, x_{2} \cdots x_{N}\right) \Psi_{n_{1}, n_{2}, \cdots n_{N}}=E_{n_{1}, n_{2}, \cdots n_{N}} \Psi_{n_{1}, n_{2}, \cdots n_{N}} \tag{3.29}
\end{equation*}
$$

Como las partículas del gas son indistinguibles, la función de estado del gas debe contener la misma información cuando se intercambian cualesquiera dos partículas. Dado que es $|\Psi|$, y no $\Psi$, quien tiene significado físico, se debe cumplir que

$$
\begin{equation*}
\Psi_{n_{1}, n_{2}, \cdots n_{N}}\left(\cdots x_{i} \cdots x_{j} \cdots\right)= \pm \Psi_{n_{1}, n_{2}, \cdots n_{N}}\left(\cdots x_{j} \cdots x_{i} \cdots\right) \tag{3.30}
\end{equation*}
$$

Es decir, la indistinguibilidad entre partículas implica que la función de estado del gas sólo puede ser simétrica (en cuyo caso diremos que el gas está formado por bosones) o antisimétrica (las partículas) del gas son fermiones.

Se puede demostrar que la únuca posibilidad de construir la función de estado de un gas de fermiones a partir de las funciones de ondas individuales es:

$$
\begin{equation*}
\Psi_{n_{1}, n_{2}, \cdots n_{N}}\left(x_{1}, x_{2} \cdots x_{N}\right)=\frac{N_{1}!N_{2}!\cdots}{N!} \sum_{\sigma} \psi_{n_{\sigma_{1}}}\left(x_{1}\right) \psi_{n_{\sigma_{2}}}\left(x_{2}\right) \cdots \psi_{n_{\sigma_{N}}}\left(x_{N}\right), \tag{3.31}
\end{equation*}
$$

donde la suma se lleva a cabo sobre todas las posibles permutaciones $\sigma$ de $\{1,2 \cdots N\}$ y $N_{\nu}=\sum_{i=1}^{N} \delta_{n_{i}, \nu}$, es el número de partículas del gas cuyo estado es $\psi_{\nu}$. En adelante, llamaremos a $N_{\nu}$ el número de ocupación del estado $\psi_{\nu}$. En el caso de un gas de bosones, el número de ocupación de cualquier estado puede variar entre cero y el número de partículas del gas, $N$. Para un gas de fermiones, la función de estado es:

$$
\begin{equation*}
\Psi_{n_{1}, n_{2}, \cdots n_{N}}\left(x_{1}, x_{2} \cdots x_{N}\right)=\frac{1}{N!} \sum_{\sigma} \epsilon^{\sigma_{1}, \sigma_{2} \cdots \sigma_{N}} \psi_{n_{\sigma_{1}}}\left(x_{1}\right) \psi_{n_{\sigma_{2}}}\left(x_{2}\right) \cdots \psi_{n_{\sigma_{N}}}\left(x_{N}\right), \tag{3.32}
\end{equation*}
$$

$\operatorname{con} \epsilon^{\sigma_{1}, \sigma_{2} \cdots \sigma_{N}}$ el tensor antisimétrico de Levi-Civita. Dada la antisimetría de la función de estado de un gas de fermiones, se sigue que no es posible tener dos partículas en el mismo estado cuántico ( $n_{i} \neq n_{j}, \forall i \neq j$ ). Este es el llamado principio de Pauli. Una consequencia del principio de Pauli es que el número de ocupación de cualquier estado de una partícula sólo puede ser cero o uno.

### Representación de los números de ocupación

De las ecuaciones (3.31) y (3.32) se sigue que, si conocemos el conjunto de funciones de estado de una partícula $\left\{\psi_{n}\right\}$, basta con conocer los números de ocupación $\left\{N_{n}\right\}$ para reconstruir la función de estado del gas, tanto si se trata de fermiones como de bosones. Lo anterior, sugiere introducir una representación cuántica en la que los números de ocupación son también los números cuánticos del sistema. En esta nueva representación, la función de estado del gas se escribe como:

$$
\begin{equation*}
\Psi=\mid N_{1}, N_{2}, \cdots> \tag{3.33}
\end{equation*}
$$

### Números de ocupacion promedio

En la representación de los números de ocupación, la gran función de partición para un gas de bosones se calcula como:

$$
\begin{equation*}
\mathcal{Z}=\sum_{N_{1}, N_{2}, \cdots=0}^{\infty} \exp \left(-\beta\left[N_{1} \varepsilon_{1}+N_{2} \varepsilon_{2} \cdots-\mu N_{1}-\mu N_{2} \cdots\right]\right)=\prod_{\nu}\left(1-\mathrm{e}^{-\beta\left(\varepsilon_{\nu}-\mu\right)}\right)^{-1} \tag{3.34}
\end{equation*}
$$

El índice $\nu=1,2 \cdots$ identifica los diferentes estados de una partícula. Por otra parte, la gran función de partición de un gas de fermiones resulta ser:

$$
\begin{equation*}
\mathcal{Z}=\sum_{N_{1}, N_{2}, \cdots=0,1} \exp \left(-\beta\left[N_{1} \varepsilon_{1}+N_{2} \varepsilon_{2} \cdots-\mu N_{1}-\mu N_{2} \cdots\right]\right)=\prod_{\nu}\left(1+\mathrm{e}^{-\beta\left(\varepsilon_{\nu}-\mu\right)}\right) \tag{3.35}
\end{equation*}
$$

Las ecuaciones (3.34) y (3.35) se pueden resumir en una sola de la siguiente forma:

$$
\begin{equation*}
\mathcal{Z}=\prod_{\nu}\left(1 \pm \mathrm{e}^{-\beta\left(\varepsilon_{\nu}-\mu\right)}\right)^{ \pm 1} \tag{3.36}
\end{equation*}
$$

donde los signo $+\mathrm{y}-$ se usan cuando el gas está respectivamente compuesto por fermiones o bosones.
De las ecuaciones (3.26) y (3.36), el número de partículas promedio del gas es:

$$
\begin{equation*}
\bar{N}=\sum_{\nu} \frac{1}{\mathrm{e}^{\beta\left(\varepsilon_{\nu}-\mu\right)} \pm 1}, \tag{3.37}
\end{equation*}
$$

donde, una vez más, el signo + corresponde a fermiones, en tanto que el signo - corresponde a bosones.
Sea $\bar{n}_{\nu}$ el número de ocupación promedio del estado $\psi_{\nu}$. Dado que $N=\sum_{\nu} n_{\nu}$,

$$
\begin{equation*}
\bar{N}=\sum_{\nu} \bar{n}_{\nu} \tag{3.38}
\end{equation*}
$$

De las ecuaciones (3.37) y (3.38) se sigue que los números de ocupación promedio de los direfentes estados de una partícula de un gas ideal cuántico están dados, en términos de la energía $\varepsilon_{\nu}$ de cada estado, por:

$$
\begin{equation*}
\bar{n}_{\nu}=\frac{1}{\mathrm{e}^{\beta\left(\varepsilon_{\nu}-\mu\right)} \pm 1} \tag{3.39}
\end{equation*}
$$

En el caso de un gas de fermiones, en el límite cuando la temperatura tiende a cero ( $\operatorname{lím} \beta \rightarrow \infty$ ), $\bar{n}_{\nu}$ tiende a la función escalón, que vale uno si $\varepsilon_{\nu}<\mu$ y vale cero en caso contrario. En el caso de un gas de bosones, como $\bar{n}_{\nu} \geq 0$, las energías $\varepsilon_{\nu}$ deben ser tales que $\varepsilon_{\nu} \geq \mu$. De hecho, para bosones, $\operatorname{lím}_{\varepsilon_{\nu} \rightarrow \mu} \bar{n}_{\nu}=\infty$.

Puesto que el número de ocupación promedio del estado $\psi_{\nu}$ sólo depende de la energía $\varepsilon_{\nu}$ del mismo, se suele escribir $\bar{n}(\varepsilon)$ en vez de $\bar{n}_{\nu}$. Con esta nueva notación, tenemos que:

$$
\begin{equation*}
\bar{n}(\varepsilon)=\frac{1}{\mathrm{e}^{\beta(\varepsilon-\mu)} \pm 1} \tag{3.40}
\end{equation*}
$$

## Función de densidad de estados

Considere una partícula de masa $m$, libre en en interior de un recipiente cúbico de lado $L$ y volumen $L=V^{3}$. La ecuación de Schrödinger de dicho sistema es:

$$
\begin{equation*}
-\frac{\hbar^{2}}{2 m} \nabla^{2} \psi(x, y, z)=\varepsilon \psi(x, y, z) \tag{3.41}
\end{equation*}
$$

Usando las ecuaciones de frontera:

$$
\begin{array}{ll}
\psi(0, y, z)=\psi(L, y, z)=0, & \forall x, y, \\
\psi(x, 0, z)=\psi(x, L, z)=0, & \forall x, z, \\
\mathrm{y} & \\
\psi(x, y, 0)=\psi(x, y, L)=0, & \forall y, z,
\end{array}
$$

la solución de la ecuación de Schrödinger queda como:

$$
\begin{equation*}
\psi(x, y, z)=C \sin \left(\frac{\kappa_{x} \pi}{L} x\right) \sin \left(\frac{\kappa_{y} \pi}{L} y\right) \sin \left(\frac{\kappa_{z} \pi}{L} z\right) \tag{3.42}
\end{equation*}
$$

donde $C$ es una constante de normalización y $\kappa_{x}, \kappa_{y}$ y $\kappa_{z}$ están obligados a obedecer la siguiente relación:

$$
\begin{equation*}
\kappa_{x}^{2}+\kappa_{y}^{2}+\kappa_{z}^{2}=\frac{2 m \varepsilon L^{2}}{\pi^{2} \hbar^{2}} \tag{3.43}
\end{equation*}
$$

A partir de la ecuación (3.43), podemos representar gráficamente los estados accesibles a la partícula libre como los vertices de una malla cúbica de lado uno, localizada en el octante $\kappa_{x}, \kappa_{y}, \kappa_{z}>0$ del espacio $\left(\kappa_{x}, \kappa_{y}, \kappa_{z}\right)$. Si la energía es lo suficientemente grande, entonces podemos aproximar el número de estados con energía menor o igual que $\varepsilon(\Gamma(\varepsilon))$ como la octava parte del volumen de una esfera de radio $\left(2 m \varepsilon V^{2 / 3} / \pi^{2} \hbar^{2}\right)^{1 / 2}$, es decir:

$$
\begin{equation*}
\Gamma(\varepsilon)=\frac{V}{6 \pi^{2}}\left(\frac{2 m \varepsilon}{\hbar^{2}}\right)^{3 / 2} \tag{3.44}
\end{equation*}
$$

De la ecuación (3.44), la función de densidad de estados $(\mathcal{D}(\varepsilon) d \varepsilon)$, que nos da el número de estados de la partícula con energías en el intervalo $[\varepsilon, \varepsilon+d \varepsilon]$, se calcula como $\mathcal{D}(\varepsilon)=d \Gamma(\varepsilon) / d \varepsilon$, i.e.,

$$
\begin{equation*}
\mathcal{D}(\varepsilon) d \varepsilon=\frac{\gamma V}{4 \pi^{2}}\left(\frac{2 m}{\hbar^{2}}\right)^{3 / 2} \varepsilon^{1 / 2} d \varepsilon \tag{3.45}
\end{equation*}
$$

donde $\gamma$ es una constante que toma en cuenta la posibilidad de degeneración debida a números cuánticos como el espín.

Con el número de ocupación promedio (3.40) y la función de densidad de estados (3.45), se puede calcular el valor promedio de cualquier función de la energía $(F(\varepsilon))$ como:

$$
\begin{equation*}
\bar{F}=\int_{0}^{\infty} F(\varepsilon) \bar{n}(\varepsilon) \mathcal{D}(\varepsilon) d \varepsilon \tag{3.46}
\end{equation*}
$$

## El límite clásico

Considere el límite en que, independientemente de si se trata de un gas de fermiones o bosones, el número de ocupación promedio es bastante menor que la unidad. Para que este sea el caso se necesita que $\exp \left((\varepsilon-\mu) / k_{B} T\right) \gg 1$, con lo que la expresión para calcular los números de ocupación promedio se puede aproximar como:

$$
\begin{equation*}
\bar{n}(\varepsilon)=\lambda e^{-\varepsilon / k_{B} T} \tag{3.47}
\end{equation*}
$$

$\operatorname{con} \lambda=\exp \left(\mu / k_{B} T\right)$. Note que la expresión en la ecuación (3.47) es la misma independientemente de si estamos hablando de fermiones o de bosones. Es decir, en el límite en el que los números de ocupación son muy pequeños, la estadística se vuelve indiferente al tipo de partículas. La ecuación (3.47) define la llamada estadística de Boltzmann.

El número promedio de partículas de un gas se puede calcular como:

$$
\begin{equation*}
\bar{N}=\int_{0}^{\infty} \bar{n}(\varepsilon) \mathcal{D}(\varepsilon) d \varepsilon \tag{3.48}
\end{equation*}
$$

Sustituyendo las ecuaciones (3.45) y (3.47) en (3.48), obtenemos para el número promedio de partículas de un gas de Boltzmann lo siguiente (por simplicidad consideramos $\gamma=1$ en la presente sección):

$$
\bar{N}=\frac{\pi \lambda V}{2}\left(\frac{2 m k_{B} T}{\pi^{2} \hbar^{2}}\right)^{3 / 2} \int_{0}^{\infty} x^{2} e^{-x^{2}} d x
$$

$\operatorname{con} x^{2}=\varepsilon / k T$. Como la integral definida vale $\pi^{1 / 2} / 4, \bar{N}$ resulta estar dado por:

$$
\begin{equation*}
\bar{N}=V \lambda\left(\frac{m k T}{2 \pi \hbar^{2}}\right)^{3 / 2} \tag{3.49}
\end{equation*}
$$

Despejando $\lambda$ de (3.49) y sustituyendo en (3.47), obtenemos la siguiente expresión para el número de ocupación promedio en la estadística de Boltzmann:

$$
\begin{equation*}
\bar{n}(\varepsilon)=\frac{N}{V}\left(\frac{2 \pi \hbar^{2}}{m k_{B} T}\right)^{3 / 2} e^{-\varepsilon / k_{B} T} \tag{3.50}
\end{equation*}
$$

La energía promedio del gas de Boltzmann es:

$$
\begin{equation*}
\bar{\varepsilon}=\int_{0}^{\infty} \varepsilon \bar{n}(\varepsilon) \mathcal{D}(\varepsilon) d \varepsilon=\frac{3}{2} \bar{N} k_{B} T \tag{3.51}
\end{equation*}
$$

la cual coincide con la correspondiente expresión del gas ideal clásico. Esto confirma que la estadística de Boltzmann corresponde al gas ideal clásico y explica por qué en tal caso es innecesario hacer la distinción entre fermiones y bosones.

## La energía de Fermi

Sabemos que para fermiones el número de ocupación promedio tiende a la función escalón, que vale uno para energías menores que $\mu$ y cero para energías mayores, en el límite cuando la temperatura tiende a cero. Esto implica que en el límite de temperatura cero, el número promedio de partículas de un gas de fermiones se puede calcular como:

$$
\begin{equation*}
\bar{N}=\int_{0}^{\infty} \bar{n}(\varepsilon) \mathcal{D}(\varepsilon) d \varepsilon=\int_{0}^{\varepsilon_{F}} \mathcal{D}(\varepsilon) d \varepsilon \tag{3.52}
\end{equation*}
$$

donde $\varepsilon_{F}=\mu$ se conoce como la energía de Fermi. Después de realizar la integral y despejar $\varepsilon_{F}$ se tiene que:

$$
\begin{equation*}
\varepsilon_{F}=\frac{\hbar^{2}}{2 m}\left(\frac{6 \pi^{2} \bar{N}}{\gamma V}\right)^{2 / 3} \tag{3.53}
\end{equation*}
$$

## Gas de electrones

El incremento en la energía total en un gas formado por $N$ electrones cuando se calienta desde el cero absoluto hasta una temperatura $T$ está dado por:

$$
\begin{equation*}
\Delta \bar{E}=\int_{0}^{\infty} \varepsilon \mathcal{D}(\varepsilon) \bar{n}(\varepsilon) d \varepsilon-\int_{0}^{\varepsilon_{F}} \varepsilon \mathcal{D}(\varepsilon) d \varepsilon \tag{3.54}
\end{equation*}
$$

con

$$
\bar{n}(\varepsilon)=\frac{1}{e^{\beta(\varepsilon-\mu)}+1}
$$

Consideremos ahora la identidad

$$
N=\int_{0}^{\infty} \mathcal{D}(\varepsilon) \bar{n}(\varepsilon) d \varepsilon=\int_{0}^{\varepsilon_{F}} \mathcal{D}(\varepsilon) d \varepsilon
$$

y multipliquémosla por $\varepsilon_{F}$ para obtener

$$
\begin{equation*}
\left(\int_{0}^{\varepsilon_{F}}+\int_{\varepsilon_{F}}^{\infty}\right) \varepsilon_{F} \mathcal{D}(\varepsilon) \bar{n}(\varepsilon) d \varepsilon=\int_{0}^{\varepsilon_{F}} \varepsilon_{F} \mathcal{D}(\varepsilon) d \varepsilon \tag{3.55}
\end{equation*}
$$

Usando (3.55) podemos reescribir (3.54) como

$$
\begin{equation*}
\Delta \bar{E}=\int_{\varepsilon_{F}}^{\infty}\left(\varepsilon-\varepsilon_{F}\right) \mathcal{D}(\varepsilon) \bar{n}(\varepsilon) d \varepsilon+\int_{0}^{\varepsilon_{F}}\left(\varepsilon_{F}-\varepsilon\right) \mathcal{D}(\varepsilon)[1-\bar{n}(\varepsilon)] d \varepsilon \tag{3.56}
\end{equation*}
$$

El primer término en la ecuación (3.56) denota la energía necesaria para llevar electrones en orbitales con energía $\varepsilon_{F}$ a orbitales con energías mayores, en tanto que el segundo término representa la energía necesaria para llevar electrones desde orbitales inferiores hasta el nivel $\varepsilon_{F}$.

Puesto que en la ecuación (3.56) el único término dependiente de la temperatura es $\bar{n}(\varepsilon)$, la capacidad calorífica del gas de electrones se puede calcular como:

$$
\begin{equation*}
C_{\mathrm{el}}=\frac{d U}{d T}=\int_{0}^{\infty} \mathcal{D}(\varepsilon)\left(\varepsilon-\varepsilon_{F}\right) \frac{d \bar{n}(\varepsilon)}{d T} d \varepsilon \tag{3.57}
\end{equation*}
$$

La temperatura de interés en metales es bastante pequeña $\left(k_{B} T / \varepsilon_{F}<0,01\right)$. Lo anterior implica que la derivada de $\operatorname{overlinen}(\varepsilon)$ es muy grande para valores de $\varepsilon$ cercanos a $\varepsilon_{F}$ y despreciable para cualquier otro valor. Por tanto, podemos aproximar $\mathcal{D}(\varepsilon) \simeq \mathcal{D}\left(\varepsilon_{F}\right)$ :

$$
\begin{equation*}
C_{\mathrm{el}} \simeq \mathcal{D}\left(\varepsilon_{F}\right) \int_{0}^{\infty}\left(\varepsilon-\varepsilon_{F}\right) \frac{d \bar{n}}{d T} d \varepsilon \tag{3.58}
\end{equation*}
$$

A bajas temperaturas $\left(T \ll \varepsilon_{F} / k_{B}\right)$, el potencial qímico de un gas de electrones es prácticamente constante e igual a $\varepsilon_{F}$. En consecuencia:

$$
\begin{equation*}
\frac{d \bar{n}}{d t} \simeq \frac{\varepsilon-\varepsilon_{F}}{k_{B} T^{2}} \cdot \frac{e^{\left(\varepsilon-\varepsilon_{F}\right) / k_{B} T}}{\left[e^{\left(\varepsilon-\varepsilon_{F}\right) / k_{B} T}+1\right]^{2}} \tag{3.59}
\end{equation*}
$$

Sustituyendo (3.59) en (3.58) y haciendo el cambio de variable $x=\left(\varepsilon-\varepsilon_{F}\right) / k_{B} T$ se sigue que

$$
\begin{equation*}
C_{\mathrm{el}} \simeq k_{B}^{2} T \mathcal{D}\left(\varepsilon_{F}\right) \int_{-\varepsilon_{F} / k_{B} T}^{\infty} x^{2} \frac{e^{x}}{\left(e^{x}+1\right)^{2}} d x \tag{3.60}
\end{equation*}
$$

Aproximando $-\varepsilon_{F} / k_{B} T \simeq-\infty$ y usando que $\mathcal{D}\left(\varepsilon_{F}\right)=3 N / 2 \varepsilon_{F}$ y

$$
\int_{-\infty}^{\infty} x^{2} \frac{e^{x}}{\left(e^{x}+1\right)^{2}} d x=\frac{\pi^{2}}{3}
$$

la ecuación (3.60) queda como

$$
\begin{equation*}
C_{\mathrm{el}} \simeq \frac{1}{2} \pi^{2} N k_{B} \cdot \frac{k_{B} T}{\varepsilon_{F}} \tag{3.61}
\end{equation*}
$$

### Radiación de cuerpo negro

Considere un gas de fotones en equilibrio a temperature $T$, en el interior de un recipiente de volumen $V$. La energía de un fotón está en función de la frecuencia angular $(\omega)$ del mismo: $\varepsilon=\hbar \omega$. Por otra parte, el potencial químico de un gas de fotones es cero: $\mu=0$. Con esto, el número de ocupación promedio del gas de fotones se puede escribir como:

$$
\begin{equation*}
\bar{n}(\omega)=\frac{1}{e^{\hbar \omega} / k_{B} T}-1 \tag{3.62}
\end{equation*}
$$

Por otra parte, tomando en cuenta que para una misma frecuencia existen dos polarizaciones independientes, es posible derivar (resolviendo la ecuación de onda $\nabla^{2} \psi=\ddot{\psi} / c^{2}$ ) la siguiente función de densidad de estados para fotones:

$$
\begin{equation*}
\mathcal{D}(\omega) d \omega=\frac{V}{\pi^{2} c^{3}} \omega^{2} d \omega \tag{3.63}
\end{equation*}
$$

donde $c$ es la velocidad de la luz.
La energía por unidad de volumen de los fotones cuya frecuencia se encuentra en el intervalo $[\omega, \omega+d \omega]$, también conocida como densidad de energía espectral, está dada por:

$$
\begin{equation*}
u_{\omega} d \omega=\frac{\bar{n}(\omega) \hbar \omega \mathcal{D}(\omega)}{V} d \omega=\frac{\hbar}{\pi^{2} c^{3}} \frac{\omega^{3}}{e^{\hbar \omega / k_{B} T}-1} d \omega \tag{3.64}
\end{equation*}
$$

La densidad de energía del gas de fotones se calcula como

$$
\begin{equation*}
u=\int_{0}^{\infty} u_{\omega} d \omega=\left(\frac{\pi^{2} k_{B}^{4}}{60 \hbar^{3} c^{2}}\right) T^{4} \tag{3.65}
\end{equation*}
$$

Esta es la llamada ley de radiación de Stefan-Boltzmann. El coeficiente de $T^{4}$ es la constante $\sigma$ de StefanBoltzmann.

Un pequeño orificio en la pared del recipiente que contiene al gas de fotones es una muy buena aproximación de un cuerpo negro. La intensidad de la radiación que escapa por el orificio $(I)$ está relacionada con la densidad de energía del gas por $I=c u / 4$, i.e.,

$$
\begin{equation*}
I=\left(\frac{\pi^{2} k_{B}^{4}}{15 \hbar^{3} c^{3}}\right) T^{4} \tag{3.66}
\end{equation*}
$$

## Capacidad Calorífica del sólido cristalino

Un sólido cristalino compuesto por $N$ átomos arreglados en una red periódica posee $3 N$ modos normales de oscilación. Esto significa que cualquier oscilación del sólido puede expresarse como una combinación lineal de oscilaciones con las $3 N$ frecuencias normales y diferentes amplitudes. Desde el punto de vista de la mecánica cuántica, la energía de una oscilación determinada está cuantizada y sólo puede tomar valores que sean múltiplos de $\hbar \omega$, con $\omega$ la frecuencia angular de la oscilación. Puesto que la energía de oscilación es proporcional al cuadrado de la intensidad, resulta que la intensidad también está cuantizada. De lo anterior se desprende que cualquier oscilación de un sólido cristalino se puede interpretar como un gas ideal de cuasipartículas cuánticas llamadas fononoes. Pueden existir fonones de $3 N$ frecuencias distintas y el número de fonones de una determinada frecuencias depende de la intensidad del correspondiente modo normal de oscilación.

Por otra parte, los fonones son bosones con una degeneración igual a 3 y potencial químico nulo. Puede haber 3 fonones independientes de una frecuencia dada, 2 de ellos correspondientes a las 2 polarizaciones independientes de ondas transversales y otro más correspondiente a ondas longitudinales. Los fonones se desplazan con la velocidad de las ondas transversales o longitudinales correspondientes. Finalmente, puesto que el número de modos normales de oscilación es finito, existe una cota superior $\omega_{\text {max }}$ para la frecuencia de los fonones.

De lo establecido en los párrafos anteriores y de la ecuación 3.46 se sigue que la energía promedio de un gas de fonones en equilibrio se puede calcular como:

$$
\begin{equation*}
\bar{E}=\int_{0}^{\omega_{\max }} \frac{\hbar \omega}{e^{\beta \hbar \omega}-1} \mathcal{D}(\omega) d \omega \tag{3.67}
\end{equation*}
$$

### Aproximación de Einstein

En uno de sus celebrados artículos de 1905, Einstein estudió la capacidad calorífica del sólido cristalino. Para ello supuso que todos los modos normales de oscilación se pueden caracterizar mediante una única
frecuencia omega. Esto equivale a suponer que $\mathcal{D}(\omega)=3 N \delta\left(\omega-\omega_{E}\right)$, con lo que la ecuación (3.67) se convierte en:

$$
\begin{equation*}
\bar{E}=\frac{3 N \hbar \omega_{E}}{e^{\beta \hbar \omega_{E}}-1} \tag{3.68}
\end{equation*}
$$

Al derivar la ecuación (3.68) con respecto a $T=1 / k_{B} \beta$ se obtiene la siguiente expresión para la capacidad calorífica de un sólido cristalino en la aproximación de Einstein:

$$
\begin{equation*}
C_{V}=3 N k_{B}\left(\frac{\Theta_{E}}{T}\right)^{2} \frac{\exp \left(\Theta_{E} / T\right)}{\left[\exp \left(\theta_{E} / T\right)-1\right]^{2}} \tag{3.69}
\end{equation*}
$$

$\operatorname{con} \Theta_{E}=\hbar \omega_{E} / k_{B}$. De la ecuación (3.69) se desprende que el calor específico molar está dado por:

$$
\begin{equation*}
c_{V}^{*}=3 R\left(\frac{\Theta_{E}}{T}\right)^{2} \frac{\exp \left(\Theta_{E} / T\right)}{\left[\exp \left(\theta_{E} / T\right)-1\right]^{2}} \tag{3.70}
\end{equation*}
$$

donde se ha tomado en cuenta que el número de moles $(n)$ y el número de partículas $(N)$ satisfacen la eelación $n R=N k_{B}$.

De la ecuación (3.70) es fácil comprobar que $\lim _{T \rightarrow \infty}=3 R$, lo cual esta de acuerdo con el resultado clásico. Similarmente, en la región de muy bajas temperaturas $c_{V}^{*} \propto \exp \left(-\Theta_{E} / T\right)$, lo cual significa que el calor específico del sólido cristalino debido a las oscilaciones elásticas decáe exponencialmente conforme la temperatura se aproxima al cero absoluto. Este último resultado esá de acuerdo con la tercera ley de la termodinámica (que exige que $\operatorname{lím}_{T \rightarrow 0} c_{X}^{*}=0$ ), pero contradice los resultados experimentales de acuerdo con los cuales $c_{V}^{*}$ decáe como $T^{3}$ en la región de muy bajas temperaturas.

### Aproximación de Debye

Para mejorar el modelo de Einstein Debye supuso que la función de densidad de estados es de la forma

$$
\mathcal{D}= \begin{cases}\frac{3 V}{2 \pi^{2} v_{s}^{3}} \omega^{2}, & \omega \leq \omega_{D}  \tag{3.71}\\ 0 & \omega>\omega_{D}\end{cases}
$$

En la expresión anterior $V$ es el volumen del sólido, $v_{s}$ es un promedio apropiado de la velacidad de las ondas elásticas longitudinales y transversales, el factor 3 da cuenta de las tres polarizaciones (dos longitudinales y una transversal) independientes de las óndas elásticas y $\omega_{D}$ es la frecuencia máxima posible para las ondas elásticas en el sólido. El valor de la frecuencia de Debye $\omega_{D}$ se determina de la siguiente restricción:

$$
3 N=\int_{0}^{\omega_{D}} \mathcal{D}(\omega) d \omega=\frac{V}{2 \pi^{2} v_{s}^{3}} \omega_{D}^{3}
$$

de donde imediatamente se sigue que

$$
\begin{equation*}
\omega_{D}=\left(\frac{6 \pi^{2} N v_{s}^{3}}{V}\right)^{1 / 3} \tag{3.72}
\end{equation*}
$$

A partir de la ecuación (3.72) la función de densidad de estados se puede escribir como

$$
\begin{equation*}
\mathcal{D}\left(\omega<\omega_{D}\right)=9 N \frac{\omega^{2}}{\omega_{D}^{3}} \tag{3.73}
\end{equation*}
$$

La energía elástica promedio de un sólido cristalino a temperatura $T$ se calcula a partir de las ecuaciones (3.67), (3.72) y (3.73) quedando como

$$
\begin{equation*}
\bar{E}=\frac{9 N\left(k_{B} T\right)^{4}}{\left(\hbar \omega_{D}\right)^{3}} \int_{0}^{x_{D}} \frac{x^{3}}{e^{x}-1} d x \tag{3.74}
\end{equation*}
$$

En esta ecuación $x_{D}=\hbar \omega_{D} / k_{B} T=\Theta_{D} / T$, con $\Theta_{D}=\hbar \omega_{D} / k_{B}$.

En la región de muy bajas temperaturas $x_{D} \gg 1$, por lo que podemos aproximar

$$
\begin{equation*}
\bar{E}=\frac{9 N\left(k_{B} T\right)^{4}}{\left(\hbar \omega_{D}\right)^{3}} \int_{0}^{\infty} \frac{x^{3}}{e^{x}-1} d x=\frac{3 \pi^{4} N k_{B} T^{4}}{5 \Theta_{D}^{3}} \tag{3.75}
\end{equation*}
$$

De la ecuación anterior, el calor específico debido a las oscilaciones elásticas en el límite de bajas temperaturas resulta, en esta aproximación, estar dado por

$$
\begin{equation*}
c_{V}^{*}=\frac{12 \pi^{4} N k_{B}}{5}\left(\frac{T}{\Theta_{D}}\right)^{3} \tag{3.76}
\end{equation*}
$$

