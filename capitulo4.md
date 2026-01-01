# Capítulo 4. Termodinámica de Reacciones Químicas

## Introducción: El Criterio de Espontaneidad de Gibbs

En el estudio de las transformaciones químicas, el objetivo central es determinar la dirección del cambio y el punto de equilibrio. Bajo condiciones habituales de laboratorio, presión ($P$) y temperatura ($T$) constantes, la función de estado que gobierna el sistema es la energía libre de Gibbs ($G$).

El segundo principio de la termodinámica dicta que, para estos procesos, el sistema evolucionará espontáneamente hacia un mínimo de energía libre ($dG < 0$).

## El Potencial Químico y la Relación Fundamental

Para sistemas donde la composición cambia (por entrada/salida de materia o por reacciones internas), la diferencial de Gibbs debe incluir términos que den cuenta de la variación en el número de moléculas $N_i$. La Relación Fundamental de Gibbs se expresa como:

$$
d G = -S d T + V d P + \sum_{i} \mu_{i} d N_{i},
$$

donde $\mu_i$ es el potencial químico de la especie $i$, definido formalmente como:

$$
\mu_i = \left( \frac{\partial G}{\partial N_i} \right)_{T, P, N_{j \neq i}}.
$$

A $P$ y $T$ constantes ($dT=0, dP=0$), el cambio en la energía libre depende exclusivamente de la composición química:

$$
d G = \sum_{i} \mu_{i} d N_{i}.
$$

Conceptualmente, $\mu_i$ representa la "presión química" o la tendencia de una especie a reaccionar o difundirse.

## Estequiometría y Grado de Avance ($\xi$)

En una reacción química, las variaciones en $N_i$ no son independientes, sino que están vinculadas por la estequiometría.

Para un sistema con múltiples reacciones $j$, el cambio en el número de moléculas de la especie $i$ es:

$$
d N_{i} = \sum_{j} \gamma_{i j} d \xi_{j},
$$

donde $\xi$ es el grado de avance de la reacción $j$ (una variable que cuantifica el progreso de la reacción) y $\gamma_{i j}$ es el coeficiente estequiométrico (positivo para productos, negativo para reactivos) de la especie química $i$ en la reacción $j$. Al sustituir esto en la diferencial de Gibbs obtenemos:

$$
d G = \sum_{j} \left( \sum_{i} \mu_{i} \gamma_{i j} \right) d \xi_{j} = \sum_{j} A_{j} d \xi_{j}.
$$

Aquí, $\Delta G_{j} = \sum_{i} \mu_{i} \gamma_{i j}$ se denomina la afinidad química de la reacción $j$.

## Reacciones Químicas Acopladas

En sistemas complejos, como las rutas metabólicas, las reacciones suelen estar acopladas. En estos casos, el avance del sistema se define por una coordenada única $\xi$. Con esto, la variación total es:

$$
\Delta G = \frac{d G}{d \xi} = \sum_{j} \Delta G_{j}.
$$

Un principio fundamental que se depende de la relación anterior es que una reacción con $\Delta G$ positivo (no espontánea) puede ocurrir si se acopla a otra con un $\Delta G$ lo suficientemente negativo como para que el balance total sea negativo.

El potencial químico depende de la concentración $c_i$ (normalizada con respecto una concentración de referencia) como:

$$
\mu_{i} = \mu_{i}^{0} + R T \ln c_{i},
$$

donde $\mu_i^0$ es el potencial químico de la especie $i$ en el estado de referencia. Con esto,  podemos expresar el cambio molar de energía libre de Gibbs como:

$$
\Delta G = \Delta G^{0} + R T \ln \prod_{i} c_{i}^{\gamma_{i}},
$$

donde $\Delta G^{0} = \sum \mu_{i}^{0} \gamma_{i}$ es el cambio de energía libre estándar.

## Equilibrio Químico

El equilibrio químico se alcanza cuando la energía libre de Gibbs es mínima para las condiciones dadas, lo que implica que la afinidad química desaparece:

$$
\Delta G = 0.
$$

A partir de esta condición, se deriva la relación fundamental con las concentraciones de equilibrio ($\bar{c}_i$):

$$
\Delta G^{0} = -R T \ln \prod_{i} \bar{c}_{i}^{\gamma_{i}}.
$$

## Cinética Química y su Vínculo Termodinámico

Mientras que la termodinámica define la dirección, la cinética define la velocidad. Para una reacción reversible:

$$
\sum \alpha_i A_i \underset{k^{-}}{\stackrel{k^{+}}{\rightleftharpoons}} \sum \beta_j B_j,
$$

la velocidad neta ($v$) es la diferencia entre la velocidad directa e inversa:

$$
v = k^{+} \prod a_{i}^{\alpha_{i}} - k^{-} \prod b_{j}^{\beta_{j}}.
$$

### Conexión en el Equilibrio

En el equilibrio químico ($v = 0$), las velocidades se igualan:

$$
k^{+} \prod \bar{a}_{i}^{\alpha_{i}} = k^{-} \prod \bar{b}_{j}^{\beta_{j}}.
$$

Esto define la constante de asociación $K_A$ como el cociente de las constantes de reacción:

$$
K_{A} = \frac{k^{+}}{k^{-}} = \frac{\prod \bar{b}_{j}^{\beta_{j}}}{\prod \bar{a}_{k}^{\alpha_{k}}} = \prod_{i} \bar{c}_{i}^{\gamma_{i}}.
$$

Finalmente, vinculamos la cinética con la termodinámica estándar:

$$
\Delta G^{0} = -R T \ln K_{A} \implies K_A = \exp\left( -\frac{\Delta G^0}{RT} \right).
$$

En definitiva, la descripción termodinámica de las reacciones químicas proporciona un marco unificado que conecta la estabilidad molecular con la dinámica de transformación de la materia. La convergencia final entre la constante de equilibrio y las constantes de velocidad demuestra que la cinética y la termodinámica no son disciplinas independientes, sino dos caras de una misma moneda: mientras la primera dicta la escala temporal del cambio, la segunda impone los límites energéticos infranqueables que definen el estado final de equilibrio del universo químico.

