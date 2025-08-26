# Simulación de marcha aleatoria en 1D

Este repositorio contiene la implementación en Python de una **marcha aleatoria en una dimensión**, 
realizada como parte de la **Tarea 1 de Física Estadística**.

## Descripción

Una partícula realiza una marcha aleatoria unidimensional: en cada paso puede moverse a la derecha o a la izquierda con igual probabilidad.  

El código permite:
- Simular $N$ pasos y obtener la posición final.
- Repetir la simulación muchas veces para construir histogramas.
- Comparar los resultados con la predicción del **Teorema Central del Límite**.
- Calcular los momentos $\langle x \rangle$ y $\langle x^2 \rangle$ para distintos $N$.
- Verificar que $\langle x^2 \rangle \propto N$ y estimar el **coeficiente de difusión** $D$.

## Requisitos

El proyecto está escrito en **Python 3** y requiere las siguientes librerías:

- `numpy`
- `matplotlib`
- `scikit-learn` (para regresión lineal)

Se pueden instalar con:

```bash
pip install numpy matplotlib scikit-learn
```

## Resultados esperados

- La distribución de posiciones finales se aproxima a una **campana de Gauss** cuando $N$ es grande.
- Se verifica que:

$$
\langle x^2 \rangle \approx N a^2
$$

- A partir de la regresión lineal, se obtiene que la pendiente $m \approx a^2$, lo que confirma la proporcionalidad.
- El coeficiente de difusión resulta ser:

$$
D = \frac{a^2}{2}
$$


