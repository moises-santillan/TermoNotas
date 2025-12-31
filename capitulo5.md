# Capítulo 5: Termodinámica y Cinética del Transporte Iónico

### El Trabajo Eléctrico y la Energía Interna

En termodinámica, el cambio en la energía interna $U$ de un sistema simple está dado por la suma del calor y el trabajo. Si el sistema contiene partículas cargadas y existe un potencial eléctrico $\phi$, debemos incluir el trabajo eléctrico ($W_e$) necesario para mover una carga $q$ desde el infinito hasta su posición actual:

$$
W_e = q \cdot \phi.
$$

Si consideramos una cantidad de sustancia $N_i$ (en moles) de la especie $i$, la carga total asociada es $q_i = z_i F N_i$, donde $z_i$ es la valencia del ion y $F$ es la constante de Faraday. Por lo tanto, para un sistema abierto en presencia de un campo eléctrico, la relación fundamental de Gibbs queda de la siguiente forma:

$$
dU = TdS - PdV + \sum_i \mu_i^{quim} dN_i + \sum_i \phi d(z_i F N_i).
$$

### Potencial Electroquímico ($\tilde{\mu}_i$)

La representación termodinámica adecuada para procesos a presión y temperatura constantes es la de la energía libre de Gibbs ($G$). Realizando la transformación de Legendre ($G = U + PV - TS$), obtenemos:

$$
dG = -SdT + VdP + \sum_i \left( \mu_i^{quim} + z_i F \phi \right) dN_i.
$$

En este contexto, definimos el potencial electroquímico ($\tilde{\mu}_i$) como la derivada parcial de la energía libre de Gibbs respecto al número de moles de la especie $i$, manteniendo $T$, $P$ y el resto de especies constantes:

$$
\tilde{\mu}_i = \left( \frac{\partial G}{\partial N_i} \right)_{T, P, N_{j \neq i}} = \tilde{\mu}_i = \mu_i^{quim} + z_i F \phi.
$$

Sustituyendo la definición del potencial químico para una solución ideal ($\mu_i^{quim} = \mu_i^0 + RT \ln c_i$), llegamos a la siguiente expresión:

$$
\tilde{\mu}_i = \underbrace{\mu_i^0 + RT \ln c_i}_{†} + \underbrace{z_i F \phi}_{††}.
$$

* **† Término Químico:** Representa la energía debida al potencial estándar y a la entropía de mezcla (gradiente de concentración).
* **†† Término Eléctrico:** Representa la energía potencial de la carga en el campo eléctrico (gradiente de voltaje).


### Condición de Equilibrio y Ecuación de Nernst

El equilibrio termodinámico de una especie a través de una membrana permeable que separa 2 compartimentos (1 y 2) se alcanza cuando no hay variación neta de energía libre al mover una partícula de uno al otro; es decir, cuando el potencial electroquímico es igual en ambos compartimentos:
\begin{align*}
\tilde{\mu}_i^{(1)} &= \tilde{\mu}_i^{(2)}, \\
\mu_i^0 + RT \ln c_i^{(1)} + z_i F \phi^{(1)} &= \mu_i^0 + RT \ln c_i^{(2)} + z_i F \phi^{(2)}.
\end{align*}
Haciendo un poco de álgebra:
\begin{align*}
z_i F (\phi^{(2)} - \phi^{(1)}) &= RT \ln c_i^{(1)} - RT \ln c_i^{(2)}, \\
z_i F \Delta \phi &= RT \ln \frac{c_i^{(1)}}{c_i^{(2)}}.
\end{align*}
Finalmente, despejando $\Delta \phi$ de la última expresión obtenemos la ecuación de Nernst:
$$
\Delta \phi = \frac{RT}{z_i F} \ln \frac{c_i^{(1)}}{c_i^{(2)}}.
$$

La ecuación de Nernst representa el estado de equilibrio dinámico en el que se igualan dos fuerzas opuestas: el gradiente de concentración (fuerza química) y el gradiente de voltaje (fuerza eléctrica). Desde una perspectiva energética, el potencial de Nernst es el valor de voltaje necesario para generar una fuerza eléctrica de magnitud idéntica —pero sentido contrario— al empuje difusivo provocado por la diferencia de concentraciones. En este punto, el sistema alcanza un mínimo de energía libre donde, aunque los iones continúan cruzando la membrana individualmente, el flujo neto es nulo, manteniendo estables las concentraciones en ambos compartimentos.

### Cinética del Transporte: La Ecuación de Nernst-Planck

En sistemas fuera del equilibrio, el transporte de una especie química es impulsado por el gradiente de su potencial electroquímico. El flujo de una especie $i$ ($J_i$, medido en $mol \cdot m^{-2} \cdot s^{-1}$) es proporcional a la fuerza impulsora: el negativo del gradiente del potencial electroquímico ($-\nabla \tilde{\mu}_i$). O anterior se traduce en la siguiente relación fenomenológica:
$$
J_i = -u_i c_i \nabla \tilde{\mu}_i,
$$
donde $u_i$ es la movilidad del ion y $c_i$ su concentración local.

Calculamos el gradiente del potencial electroquímico:
$$
\nabla \tilde{\mu}_i = \nabla (\mu_i^0 + RT \ln c_i + z_i F \phi).
$$
Como $\mu_i^0$ es una constante, su gradiente es cero. Aplicando la regla de la cadena al término logarítmico ($\nabla \ln c = \frac{1}{c} \nabla c$) obtenemos:
$$
\nabla \tilde{\mu}_i = \frac{RT}{c_i} \nabla c_i + z_i F \nabla \phi.
$$
Sustituyendo en la relación fenomenológica:
$$
\begin{align*}
J_i &= -u_i c_i \left( \frac{RT}{c_i} \nabla c_i + z_i F \nabla \phi \right)
J_i &= -u_i RT \nabla c_i - u_i z_i F c_i \nabla \phi
\end{align*}
Utilizamos la relación de Einstein, que vincula la movilidad con el coeficiente de difusión: $D_i = u_i RT$. Sustituyendo esto, obtenemos la ecuación de Nernst-Planck:
$$
J_i = -D_i \left( \nabla c_i + \frac{z_i F c_i}{RT} \nabla \phi \right).
$$

La ecuación de Nernst-Planck divide el transporte iónico en dos contribuciones:
1. **Término de Difusión ($-D_i \nabla c_i$):** Movimiento debido al gradiente de concentración (Ley de Fick). Los iones se mueven hacia zonas de baja concentración para maximizar la entropía.
2. **Término de Migración Eléctrica ($-D_i \frac{z_i F c_i}{RT} \nabla \phi$):** Movimiento bajo la influencia de un campo eléctrico (Electroforesis).

Si el sistema alcanza el equilibrio, el flujo neto se anula ($J_i = 0$). En una dimensión ($x$):
$$
0 = \frac{dc_i}{dx} + \frac{z_i F c_i}{RT} \frac{d\phi}{dx}.
$$
Integrando entre dos compartimentos, recuperamos la ecuación de Nernst:
$$
\ln \frac{c_i^{(2)}}{c_i^{(1)}} = -\frac{z_i F}{RT} (\phi^{(2)} - \phi^{(1)}) \implies \Delta \phi = \frac{RT}{z_i F} \ln \frac{c_i^{(1)}}{c_i^{(2)}}.
$$

