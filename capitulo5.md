# Capítulo 5: Termodinámica y Cinética del Transporte Iónico

En este capítulo, estudiaremos cómo las fuerzas químicas y eléctricas se integran para gobernar el movimiento de partículas cargadas a través de interfaces, un proceso fundamental tanto en la fisiología celular como en la electroquímica industrial.

## El Trabajo Eléctrico y la Energía Interna

Para comprender el transporte iónico, debemos reconocer que los iones no solo están sujetos a gradientes de concentración, sino también a campos eléctricos. En termodinámica, el cambio en la energía interna $U$ de un sistema depende del calor y de todas las formas de trabajo realizado. Si el sistema contiene partículas cargadas, debemos incluir el **trabajo eléctrico** ($W_e$) necesario para traer una carga $q$ desde un punto de referencia (infinito) hasta un potencial eléctrico $\phi$:

$$
W_e = q \cdot \phi.
$$

Dado que trabajamos con sustancias químicas, expresamos la carga en términos de moles ($N_i$). La carga total de una especie $i$ es el producto del número de moles por su valencia ($z_i$) y la constante de Faraday ($F$), que representa la carga de un mol de electrones ($F \approx 96,485$ C/mol): 

$$q_i = z_i F N_i.$$

Al integrar este trabajo en la relación fundamental de Gibbs para un sistema abierto, obtenemos la expresión de la energía interna que incluye la contribución de la energía potencial eléctrica:

$$
dU = TdS - PdV + \sum_i \mu_i^{quim} dN_i + \sum_i \phi d(z_i F N_i).
$$

Aquí, el término $\sum \phi d(z_i F N_i)$ representa la energía necesaria para añadir iones a un sistema que ya posee un potencial eléctrico determinado.

## Potencial Electroquímico ($\tilde{\mu}_i$)

Para la mayoría de los sistemas biológicos y químicos, el control experimental se ejerce sobre la presión ($P$) y la temperatura ($T$). Por ello, utilizamos la energía libre de Gibbs ($G$). Al aplicar la transformación de Legendre ($G = U + PV - TS$) a la ecuación anterior, la diferencial se convierte en:

$$
dG = -SdT + VdP + \sum_i \left( \mu_i^{quim} + z_i F \phi \right) dN_i.
$$

El término entre paréntesis representa la energía total aportada por un mol de la especie $i$, considerando tanto sus propiedades químicas como su interacción con el campo eléctrico. Definimos formalmente este valor como el potencial electroquímico ($\tilde{\mu}_i$):

$$
\tilde{\mu}_i = \left( \frac{\partial G}{\partial N_i} \right)_{T, P, N_{j \neq i}} = \tilde{\mu}_i = \mu_i^{quim} + z_i F \phi.
$$

Sustituyendo la definición del potencial químico para una solución ideal ($\mu_i^{quim} = \mu_i^0 + RT \ln c_i$), obtenemos la ecuación fundamental del transporte iónico:

$$
\tilde{\mu}_i = \underbrace{\mu_i^0 + RT \ln c_i}_{†} + \underbrace{z_i F \phi}_{††}.
$$

* **† Término Químico:** Refleja la estabilidad intrínseca de la molécula ($\mu_i^0$) y la tendencia estadística a difundirse debido al desorden térmico ($\ln c_i$).
* **†† Término Eléctrico:** Refleja la energía potencial debida a la interacción de la carga del ion con el entorno eléctrico local.

## Condición de Equilibrio y Ecuación de Nernst

El equilibrio termodinámico entre dos compartimentos (1 y 2) separados por una membrana se define como el estado donde no existe una fuerza impulsora neta; es decir, mover un ion del lado 1 al lado 2 no produce un cambio en la energía libre del sistema. Esto ocurre cuando los potenciales electroquímicos se igualan:

\begin{align*}
\tilde{\mu}_i^{(1)} &= \tilde{\mu}_i^{(2)}, \\
\mu_i^0 + RT \ln c_i^{(1)} + z_i F \phi^{(1)} &= \mu_i^0 + RT \ln c_i^{(2)} + z_i F \phi^{(2)}.
\end{align*}

Sustituyendo los términos correspondientes y asumiendo que el potencial estándar $\mu_i^0$ es el mismo en ambos lados de la membrana:

\begin{align*}
z_i F (\phi^{(2)} - \phi^{(1)}) &= RT \ln c_i^{(1)} - RT \ln c_i^{(2)}, \\
z_i F \Delta \phi &= RT \ln \frac{c_i^{(1)}}{c_i^{(2)}}.
\end{align*}

Para hallar la diferencia de potencial eléctrico ($\Delta \phi = \phi^{(2)} - \phi^{(1)}$) necesaria para mantener esta diferencia de concentraciones en equilibrio, reordenamos los términos:

$$z_i F (\phi^{(2)} - \phi^{(1)}) = RT \ln c_i^{(1)} - RT \ln c_i^{(2)}.$$

Utilizando la propiedad de los logaritmos ($\ln A - \ln B = \ln \frac{A}{B}$):

$$z_i F \Delta \phi = RT \ln \frac{c_i^{(1)}}{c_i^{(2)}}.$$

Finalmente, despejando el potencial, llegamos a la ecuación de Nernst:

$$
\Delta \phi = \frac{RT}{z_i F} \ln \frac{c_i^{(1)}}{c_i^{(2)}}.
$$

**Interpretación Física:** El potencial de Nernst es el voltaje específico que debe existir a través de una membrana para que un ion esté en equilibrio pese a tener concentraciones desiguales en ambos lados. En este estado, el flujo neto es cero porque la fuerza eléctrica empuja a los iones con la misma intensidad, pero en sentido opuesto, que la fuerza difusiva (gradiente químico).

## Cinética del Transporte: La Ecuación de Nernst-Planck

Cuando los potenciales electroquímicos no son iguales ($\tilde{\mu}_i^{(1)} \neq \tilde{\mu}_i^{(2)}$), el sistema se encuentra fuera del equilibrio y se genera un flujo neto ($J_i$). Según la termodinámica de procesos irreversibles, el flujo es proporcional a la fuerza impulsora, la cual se define como el negativo del gradiente del potencial electroquímico ($-\nabla \tilde{\mu}_i$). La relación fenomenológica es:

$$
J_i = -u_i c_i \nabla \tilde{\mu}_i,
$$

donde $u_i$ es la movilidad del ion y $c_i$ es la concentración local. Procedemos a derivar el gradiente de $\tilde{\mu}_i$:

$$\nabla \tilde{\mu}_i = \nabla (\mu_i^0 + RT \ln c_i + z_i F \phi).$$

Considerando que $\mu_i^0$ es constante en el espacio ($\nabla \mu_i^0 = 0$) y aplicando la regla de la cadena para el término logarítmico ($\nabla \ln c = \frac{1}{c} \nabla c$):

$$\nabla \tilde{\mu}_i = \frac{RT}{c_i} \nabla c_i + z_i F \nabla \phi.$$

Al sustituir este gradiente en la relación fenomenológica inicial:

\begin{align*}
J_i &= -u_i c_i \left( \frac{RT}{c_i} \nabla c_i + z_i F \nabla \phi \right)
 &= -u_i RT \nabla c_i - u_i z_i F c_i \nabla \phi
\end{align*}

Finalmente, aplicamos la relación de Einstein, que vincula la movilidad iónica con el coeficiente de difusión macroscópico ($D_i = u_i RT$). Obtenemos así la ecuación de Nernst-Planck:

$$
J_i = -D_i \left( \nabla c_i + \frac{z_i F c_i}{RT} \nabla \phi \right).
$$

**Análisis de los términos:**
1.  **Difusión:** Representa el flujo provocado por el movimiento aleatorio térmico (Ley de Fick). Los iones tienden a desplazarse de zonas de mayor a menor concentración para maximizar la entropía del sistema.
2.  **Migración Eléctrica:** Representa el flujo provocado por la fuerza electrostática sobre las partículas cargadas. Los cationes migran hacia potenciales negativos y los aniones hacia potenciales positivos.

Esta ecuación es la piedra angular para modelar procesos como el potencial de acción neuronal o la electrodiálisis, permitiendo predecir cómo varían las concentraciones y el voltaje en sistemas dinámicos fuera del equilibrio.

### Recuperación de la Ecuación de Nernst

La ecuación de Nernst-Planck describe el flujo iónico como una respuesta dinámica a gradientes químicos y eléctricos. Sin embargo, en el equilibrio termodinámico no hay transporte neto de materia ($J_i = 0$), a pesar de que el movimiento térmico individual de los iones persiste. 

Para demostrar cómo la cinética converge hacia la termodinámica clásica, consideremos el transporte en una sola dimensión ($x$) a través del espesor de una membrana. Si igualamos el flujo a cero en la ecuación de Nernst-Planck:

$$0 = -D_i \left( \frac{dc_i}{dx} + \frac{z_i F c_i}{RT} \frac{d\phi}{dx} \right).$$

Dado que el coeficiente de difusión $D_i$ es una propiedad física del sistema distinta de cero, la expresión dentro del paréntesis debe anularse necesariamente para satisfacer la igualdad. Reordenando los términos para separar las variables de concentración ($c_i$) y de potencial eléctrico ($\phi$), obtenemos:

$$\frac{dc_i}{dx} = -\frac{z_i F c_i}{RT} \frac{d\phi}{dx}.$$

Dividiendo ambos lados por $c_i$ y eliminando $dx$, eliminamos la dependencia espacial explícita, transformando la ecuación en una relación de diferenciales exactas:

$$\frac{dc_i}{c_i} = -\frac{z_i F}{RT} d\phi.$$

Para encontrar la diferencia de potencial entre dos compartimentos, integramos la ecuación desde el compartimento 1 (estado inicial) hasta el compartimento 2 (estado final):

$$\int_{c_i^{(1)}}^{c_i^{(2)}} \frac{1}{c_i} dc_i = -\frac{z_i F}{RT} \int_{\phi^{(1)}}^{\phi^{(2)}} d\phi.$$

Al resolver las integrales, obtenemos:

\begin{align*}
\ln c_i^{(2)} - \ln c_i^{(1)} &= -\frac{z_i F}{RT} (\phi^{(2)} - \phi^{(1)}), \\
\ln \frac{c_i^{(2)}}{c_i^{(1)}} &= -\frac{z_i F}{RT} \Delta \phi$$. \\
\end{align*}

Finalmente, despejando $\Delta \phi$ e invirtiendo el argumento del logaritmo para eliminar el signo negativo recuperamos la ecuación de Nernst:

$$\Delta \phi = \frac{RT}{z_i F} \ln \frac{c_i^{(1)}}{c_i^{(2)}}.$$

Esto demuestra que el equilibrio de Nernst es el caso límite de la ecuación de Nernst-Planck cuando las fuerzas impulsoras se cancelan exactamente. Físicamente, esto significa que el potencial eléctrico de la membrana se ajusta hasta compensar la tendencia del ion a difundirse a favor de su gradiente, logrando que el potencial electroquímico sea uniforme ($\nabla \tilde{\mu}_i = 0$) y, por ende, el flujo neto sea nulo.
