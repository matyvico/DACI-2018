# Trabajo Práctico 2

## Actividad 1
  Encontrar el valor que debe tener $W_{0,1}$ para obtener $I_{REF} \pm 1\%$

  ![Actividad 1](./imagenes/esquematicos/actividad_1.png){height=25%}

  De la simulacion de la corriente por $M_{1}$, sobre el circuito anterior, para una variacion de $W_{0,1}$ entre $1 \mu m$ y $50 \mu m$ se obtiene el siguiente resultado:

  ![$I_{ref} = 200 \mu m$ vs $I_{D1}$ para un barrido de $W_{0,1}$](./imagenes/actividad_1/I_ref_vs_ID_copia_swp_WNMOS.png)

  Para el punto de cruce de las curvas anteriores se obtiene el valor de $W_{0,1}$ que permitira copiar la corriente de la fuente de corriente de referencia:

  ![Zoom de la imagen anterior para el punto de cruce de las curvas de corriente](./imagenes/actividad_1/I_ref_vs_ID_copia_swp_WNMOS_cruce.png)

  De la imagen se observa que en el punto de cruce se tiene que $W_{0,1} \approx 5,33 \mu m$, se redondea el valor anterior a $W_{0,1} = 5,35 \mu m$.

  Para el nuevo valor de $W_{0,1}$ se tiene la siguiente copia de corriente:

  ![Copia de corriente para $W_{0,1} = 5,35 \mu m$](./imagenes/actividad_1/ID_copia_WNMOS_5p35.png)
  ![Error en la copia de corriente para $W_{0,1} = 5,35 \mu m$](./imagenes/actividad_1/ID_copia_WNMOS_5p35_error.png)

  El error entre la corriente de referencia $I_{REF}$ y la copia de corriente viene dada por el no cumplimiento de cualquiera de las siguientes condiciones:

  - $\frac{W_{0}}{L_{0}} = \frac{W_{1}}{L_{1}}$
  - $V_{GS0} = V_{GS1}$
  - $M_{0}$ y $M_{1}$ en saturación
  - $V_{DS0} = V_{DS1} \Rightarrow L_{0} = L_{1}$ y mientras menor sea el valor de $L$, menor será la dependencia con $\lambda$ y $V_{DS}$ (modulación de ancho de canal), menor será la pendiente de $I_{D}$ respecto de $V_{DS}$ y más estable será el valor de la corriente por $M_{1}$


## Actividad 2
  ![Actividad 2](./imagenes/esquematicos/actividad_2.png){height=25%}

  Para generar una corriente similar por las 3 ramas, es preciso que todas las tensiones $V_{GS}$ sean similares. Para lograr lo anterior se modifica el valor de $W$. Para encontrar el valor óptimo se realiza un barrido paramétrico de la variable $wmos$. Los valores encontrados son:

  - $W_{M1} = 3,1352 \um m \approx 3,135 \mu m$
  - $W_{M2} = 5,35429 \um m \approx 5,354 \um m$
  - $W_{M3} = 13,72 \um m \approx 13,72 \um m$


## Actividad 3
![Actividad 3](./imagenes/esquematicos/actividad_3.png){height=25%}

## Actividad 4
![Actividad 4](./imagenes/esquematicos/actividad_4.png){height=25%}

## Actividad 5
![Actividad 5](./imagenes/esquematicos/actividad_5.png){height=25%}

## Actividad 6
![Actividad 6](./imagenes/esquematicos/actividad_6.png){height=25%}


- : $$ \wedge \cdot \Rightarrow $$

$$ y = mx +b $$ {#eq:description}

... and then referenced like this:

lalala {@eq:description} lalala

