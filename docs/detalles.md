# Normalización en la Computación Cuántica

Un estado normalizado en computación cuántica es un estado cuántico cuyas amplitudes cumplen una condición matemática que garantiza que la suma de las probabilidades de todos los resultados posibles sea igual a 1 (es decir, al 100 %).

## Estado cuántico

En computación clásica, un bit puede valer `0` o `1`.

En computación cuántica, un qubit puede encontrarse en una combinación de los estados $|0\rangle$ y $|1\rangle$.

$$|\psi\rangle = \alpha|0\rangle + \beta|1\rangle$$

- $|\psi\rangle$ : *estado del qubit.*
- $\alpha$ : *amplitud asociada al resultado `0`.*
- $\beta$ : *amplitud asociada al resultado `1`.*

Las amplitudes pueden ser números reales o complejos.

## Estado Cuántico Normalizado

Las amplitudes tienen que cumplir esta condición:

$$|\alpha|^2 + |\beta|^2 = 1$$

Porque al medir el cúbit, obtendremos uno de los resultados posibles: `0` o `1`. La probabilidad de cada resultado se calcula elevando al cuadrado el módulo de su amplitud.

$$P(0)=|\alpha|^2$$

$$P(1)=|\beta|^2$$

Y como las probabilidades de todos los resultados posibles deben sumar el 100 %, los módulos al cuadrado deben sumar 1:

$$P(0)+P(1)=1$$

### Estado normalizado

$$|\psi\rangle=\frac{1}{\sqrt2}|0\rangle+ \frac{1}{\sqrt2}|1\rangle$$

#### Calculamos las probabilidades

$$P(0)=\left|\frac{1}{\sqrt2}\right|^2=\frac12$$

$$P(1)=\left|\frac{1}{\sqrt2}\right|^2=\frac12$$

#### Suma

$$1/2+1/2=1$$

* 50 % de probabilidad para cada estado. Está normalizado.

### Estado no normalizado

$$|\psi\rangle=|0\rangle+|1\rangle$$

#### Las amplitudes valen 1 y 1:

$$P(0)=1,\qquad P(1)=1$$

#### Suma

$$1+1=2$$

* 200% en total. No está normalizado.

## Álgebra lineal

En álgebra lineal, un estado cuántico se representa mediante un vector. Normalizarlo significa hacer que su norma sea igual a 1.

Esto se extiende también a sistemas de varios cúbits. En ese caso, sumamos los módulos al cuadrado de todas las amplitudes del estado, y el resultado debe ser 1.
