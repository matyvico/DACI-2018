# Canal Corto vs Canal Largo

## Consideraciones generales para el trabajo práctico
La relación de aspecto para todos los casos es:

$$\frac{W}{L} = 5 \Rightarrow W = 5 \cdot L$$

Entonces para los distintos casos tenemos:

  - NMOS canal corto:
  $$ L = 0,6 um \wedge W = 5 \cdot L \Rightarrow W = 5 \cdot 0,6  um = 3  um $$

![NMOS canal corto, $L = 0,6 um$](./imagenes/nmos_short_L_0p6.png){width=50%}

  - NMOS canal largo:
  $$ L = 3   um \wedge W = 5 \cdot L \Rightarrow W = 5 \cdot 3    um = 15 um $$

![NMOS canal largo, $L = 3 um$](./imagenes/nmos_long_L_3.png){width=50%}

  - NMOS canal largo:
  $$ L = 6   um \wedge W = 5 \cdot L \Rightarrow W = 5 \cdot 6    um = 30 um $$

![NMOS canal largo, $L = 6 um$](./imagenes/nmos_long_L_6.png){width=50%}


## Evaluando la curva $I_{D}$ vs $V_{GS}$

1. Determinar si la función de transferencia para cada largo de canal es cuadrática o no cuadrática.

  ![$I_{D}$ vs $V_{GS}$ ambos ejes lineales](./imagenes/ID_vs_VGS/ID_vs_VGS_group.png){width=50%}

  Del análisis de la imagen se verifica, por comparación entre las curvas para cada una de las relaciones de aspecto de los trasistores, que la funcióon de transferencia de aquellos transistores con canal largo presentan un comportamiento cuadrático, mientras que aquel con canal corto presenta uno más lineal o no cuadrático.

2. Obtener los $V_{TH}$ por análisis de punto de operación y explicar que sucede en cada caso.

3. Explicar la saturación por velocidad e indicar en que caso se da.


## Evaluando la curva $\log{I_{D}}$ vs $V_{GS}$

  - Analizar corrientes sub-umbral ($V_{GS} < V_{TH}$) para canal corto y largo.

## Evaluando la curva $I_{D}$ vs $V_{DS}$ con barrido paramétrico de $V_{GS}$

  - Comparar cómo varía $\lambda$ para los distintos niveles de $I_{D}$ (cambios en la pendiente de corriente en saturación).
  - Comparar cómo varía $\lambda$ para canal corto y canal largo.
  - Comparar cómo varía $I_{D}$ para un mismo $V_{GS}$ entre canal corto y canal largo.
  - ¿En qué caso es mayor $r_o$? y ¿cómo se relaciona con $\lambda$?.


## Listar las condiciones de polarización: Apagado, Subumbral, Triodo, Saturación.


## Evaluando la curva $g_{m}/I_{D}$ vs $I_{D}$ (Comenzar con $V_{GS} = 0,5 V$)
  - ¿Es posible alcanzar el mismo $g_{m}$ con el escalamiento realizado? ($L = 0,6 um$ vs $L = 3 um$ manteniendo $W/L = 5$).
  - ¿En que otra curva puede comprobarse esta conclusión?

![](./imagenes/gmID_vs_ID/gmID_vs_ID.png){width=50%}


## Evaluando las curvas $I_{D}$ vs $V_{GS}$ y $I_{D}$ vs $V_{DS}$ (Barrido paramétrico de $V_{GS}$) para el PMOS evaluar:
  - El signo de las corrientes y tensiones respecto al NMOS.
  - Demostrar que los signos de las corrientes y tensiones del PMOS son inversos al NMOS.


# NMOS vs PMOS

Los parametros para el PMOS son:

$$ L = 3 um \wedge \frac{W}{L} = 5 \Rightarrow W = 5 \cdot 3 um = 15 um $$

# Notas
  - Armar o conseguir una hoja de ecuaciones para el MOS en cada una de las regiones, su impedancia de entrada y salida, etc. Hacer lo mismo para las configuraciones básicas utilizadas en el curso.
  - El valor de $L$ y $t_{ox}$ cumplen un rol fundamental en el comportamiento del MOS. Uno de los objetivos principales del avance de la tecnología MOS es reducír estos valores sin degradar considerablemente otros parámetros del dispositivo.

# Dudas
  - Cual es el sentido de usar una región "deep n-well" para luego poner una región "p-well" para finalmente poder fabricar un NMOS allí con todas las desventajas de área y restricciones físicas de fabricación que posee?
  - Figura 2.5 (c), porque el símbolo del PMOS no tiene las terminales D y S invertidas como el resto de los casos?
  - Porque habla en la página 20 de que los valores de $I_{D}$ y $V_{GS} - V_{TH}$ son valores bias que ambos generan cambios en el valor de $g_m$ y que a su vez los valores de las ecuaciones deducidas en las secciones anteriores no reponden a todas las variaciones reales o incorrectos.
  - $I_{D}$ vs $V_{GS}$, la determinación de la forma de la FT para cada largo de canal, debe ser matemática, por medio de la imagen?
