# Introdução

## Teoria do raio
O método do raio tem duas vantagens. Ele proporciona a compreensão do fenômeno de propagação de ondas em modelos geofísicos razoavelmente complicados, descrevendo o campo de ondas total como a soma de diferentes tipos de ondas geradas no problema a em consideração. Isto proporciona um algoritmo numérico efetivo e que não consome tanto tempo quando comparado aos métodos de diferenças finitas e elementos finitos.

Por outro lado, o método do raio sofre com o chamado problema das cáusticas, oque significa precisamente que se os raios associados com o problema da propagação da onda sob investigação tocam uma superfície 3D (ou uma curva em 2D), o espalhamento geométrico desaparece e a amplitude do raio se torna singular neste limite, enquanto o campo de ondas real se mantém finito e suave.

Esta superfície é chamada de envelope do campo de ondas, ou superfície de cáustica. Assim, o método do raio não descreve corretamente o campo de ondas na vizinhança das cáusticas. Infelizmente, nos modelos geofísicos de meios elásticos o comportamento dos raios é complicado e eles normalmente formam cáusticas de diferentes estruturas geométricas. Então, o método do raio encontra sérios problemas com as cáusticas em aplicações geofísicas.

## Gaussian beam
On the other hand, the Gaussian beam method gives rise to a numerical algorithm for the calculations of the high frequency wave field independently of the position of an observation point. Briefly, it can be explained as follows. To calculate the wave field at an observation point M, we have to cover the vicinity of M by a fan of rays distributed in this vicinity more or less uniformly.

For each ray we have to derive a Gaussian beam propagating along the ray and then to sum the contribution of each Gaussian beam to the point M over all rays from the fan. As every Gaussiam beam has no singularity on caustics, the numerical algorithm does not depend on the position of M with respect to a caustic and on the geometrical structure of the caustic. The Gaussian beam method, as a new approach for the computation of wave fields in high frequency approximation, was suggested by M.M. Popov in his theoretical papers - See Popov (1981,1982).

## Paraxial ray theory
The main idea of the paraxial ray theory [...] can be formulated as follows. If we consider a narrow ray tube surrounding a fixed central ray of the tube, we may linearize Euler's equation for the rays from the tube because they are close to the central one. This results in a significant simplification of Euler's equation, and therefore of the whole ray theory built on them.

These equations are known in classical mechanics as equations in variations. Of course, that theory remains valid only in the vicinity of the central ray. In fact, the paraxial ray theory was used and developed by specialists in optical resonators for lasers in the 1960s. In particular, the ray centered coordinates, broadly used in (1969) in studies on self oscilations in opened resonators. In geophysics the paraxial approach was firstly used by Popov and Psencik (1978), see also Popov (1977), for the dynamic ray tracing problem.
