# Canal Corto vs Canal Largo

## Consideraciones generales para el trabajo práctico
En el siguiente trabajo práctico se realiza la comparación de las curvas básicas y relaciones de las magnitudes típicas para tres transistores MOS con diferente longitud de canal $L$ e igual relación de aspecto $W/L$.

La relación de aspecto para todos los casos es:

$$\frac{W}{L} = 5 \Rightarrow W = 5 \cdot L$$

Entonces para los distintos casos tenemos:

  - NMOS canal corto:
  $$ L = 0,6 \mu m \wedge W = 5 \cdot L \Rightarrow W = 5 \cdot 0,6 \mu m = 3 \mu m $$

![NMOS canal corto, $L = 0,6 \mu m$](./imagenes/MOS/nmos_short_L_0p6.png){width=50%}

  - NMOS canal largo:
  $$ L = 3 \mu m \wedge W = 5 \cdot L \Rightarrow W = 5 \cdot 3 \mu m = 15 \mu m $$

![NMOS canal largo, $L = 3 \mu m$](./imagenes/MOS/nmos_long_L_3.png){width=50%}

  - NMOS canal largo:
  $$ L = 6 \mu m \wedge W = 5 \cdot L \Rightarrow W = 5 \cdot 6 \mu m = 30 \mu m $$

![NMOS canal largo, $L = 6 \mu m$](./imagenes/MOS/nmos_long_L_6.png){width=50%}

Resumiendo, tenemos:

| Transistor      | $W/L$ | $L [\mu m]$ | $W [\mu m]$ |
| --------------- | ----- | ----------- | ----------- |
| `NMOS_short_L`  | $5$   | $0,6$       | $3$         |
| `NMOS_long_L_3` | $5$   | $3$         | $15$        |
| `NMOS_long_L_6` | $5$   | $6$         | $30$        |

## Evaluando la curva $I_{D}$ vs $V_{GS}$

1. Determinar si la función de transferencia para cada largo de canal es cuadrática o no cuadrática.

  ![$I_{D}$ vs $V_{GS}$](./imagenes/ID_vs_VGS/ID_vs_VGS_group.png){width=50%}

  Del análisis de la imagen se verifica, por comparación entre las curvas para cada una de las relaciones de aspecto de los trasistores, que la funcióon de transferencia de aquellos transistores con canal largo presentan un comportamiento cuadrático, mientras que aquel con canal corto presenta uno más lineal o no cuadrático.

2. Obtener los $V_{TH}$ por análisis de punto de operación y explicar que sucede en cada caso.

3. Explicar la saturación por velocidad e indicar en que caso se da.


## Evaluando la curva $\log{I_{D}}$ vs $V_{GS}$

  - Analizar corrientes sub-umbral ($V_{GS} < V_{TH}$) para canal corto y largo.

  ![$log{(I_{D})}$ vs $V_{GS}$](./imagenes/ID_vs_VGS/ID-log_vs_VGS_group.png){width=50%}

  Para tensiones $V_{GS} < V_{TH}$ (región de inversión débil del canal) se puede observar lo siguiente:

  - Hay presencia de $I_{D}$, el MOS permanece en conducción en esta región.
  - La variación de las curvas sigue un comportamiento lineal, al ser la escala del eje $y$ el logaritmo de la corriente de `Drain` se puede concluir que la corriente sub-umbral sigue un comportamiento exponencial respecto a $V_{GS}$.
  - Existe un leve desplazamiento hacia la izquierda en la respuesta del MOS de canal corto, mientras que las respuestas de aquellos de canal largo son coincidentes. Esto muestra como para un MOS con canal corto se alcanza conducción sub-umbral para tensiones $V_{GS}$ levemente inferiores frente a aquellos con canal largo.

## Evaluando la curva $I_{D}$ vs $V_{DS}$ con barrido paramétrico de $V_{GS}$

Este análisis muestra la curva fundamental del dispositivo. Se analizan las magnitudes que definen directamente la función de transferencia del transistor MOS. Además, el análisis de la familia de curvas en función de la tensión presente entre `Gate` y `Source` muestra diversos comportamientos básicos de la física del MOS que permiten incorporar fenomenos de segundo orden a su modelado.

  - Comparar cómo varía $\lambda$ para los distintos niveles de $I_{D}$ (cambios en la pendiente de corriente en saturación).

  ![$I_{D}$ vs $V_{DS}$ canal corto $L = 0,6 \mu m$](./imagenes/ID_vs_VDS_swp_VGS/ID_vs_VDS_short.png){width=50%}

  ![$I_{D}$ vs $V_{DS}$ canal largo $L = 3 \mu m$](./imagenes/ID_vs_VDS_swp_VGS/ID_vs_VDS_long_3.png){width=50%}

  ![$I_{D}$ vs $V_{DS}$ canal largo $L = 6 \mu m$](./imagenes/ID_vs_VDS_swp_VGS/ID_vs_VDS_long_6.png){width=50%}

  - Comparar cómo varía $\lambda$ para canal corto y canal largo.

  Se puede verificar que para aquellos transistores MOS con canal corto se tiene una mayor pendiente (mayor $\lambda$) que para aquellos que poseen canal largo. De esto se desprende que un transistor de canal largo tiene menor variación de $I_{D}$ que uno de canal corto para un mismo cambio de $V_{DS}$.

  - Comparar cómo varía $I_{D}$ para un mismo $V_{GS}$ entre canal corto y canal largo.

  ![$I_{D}$ vs $V_{DS}$ para $V_{GS} = 0 V$](./imagenes/ID_vs_VDS_swp_VGS/ID_vs_VDS_para_VGS_0V.png){width=50%}

  ![$I_{D}$ vs $V_{DS}$ para $V_{GS} = 1,66 V$](./imagenes/ID_vs_VDS_swp_VGS/ID_vs_VDS_para_VGS_1p66V.png){width=50%}

  ![$I_{D}$ vs $V_{DS}$ para $V_{GS} = 3,33 V$](./imagenes/ID_vs_VDS_swp_VGS/ID_vs_VDS_para_VGS_3p33V.png){width=50%}

  ![$I_{D}$ vs $V_{DS}$ para $V_{GS} = 5 V$](./imagenes/ID_vs_VDS_swp_VGS/ID_vs_VDS_para_VGS_5V.png){width=50%}

  - ¿En qué caso es mayor $r_o$? y ¿cómo se relaciona con $\lambda$?.


## Listar las condiciones de polarización: Apagado, Subumbral, Triodo, Saturación.


## Evaluando la curva $g_{m}/I_{D}$ vs $I_{D}$ (Comenzar con $V_{GS} = 0,5 V$)
  - ¿Es posible alcanzar el mismo $g_{m}$ con el escalamiento realizado? ($L = 0,6 \mu m$ vs $L = 3 \mu m$ manteniendo $W/L = 5$).
  - ¿En que otra curva puede comprobarse esta conclusión?

  ![$g_{m}/I_{D}$ vs $I_{D}$](./imagenes/gmID_vs_ID/gmID_vs_ID.png){width=50%}


## Evaluando las curvas $I_{D}$ vs $V_{GS}$ y $I_{D}$ vs $V_{DS}$ (Barrido paramétrico de $V_{GS}$) para el PMOS evaluar:
  - El signo de las corrientes y tensiones respecto al NMOS.
  - Demostrar que los signos de las corrientes y tensiones del PMOS son inversos al NMOS.


# NMOS vs PMOS

Los parametros para el PMOS son:

$$ L = 3 \mu m \wedge \frac{W}{L} = 5 \Rightarrow W = 5 \cdot 3 \mu m = 15 \mu m $$

![PMOS canal largo, $L = 3 \mu m$](./imagenes/MOS/pmos_long_L_3.png){width=50%}
