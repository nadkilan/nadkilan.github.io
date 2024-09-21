---
title:  "Entendiendo la probabilidad intuitivamente"
mathjax: true
layout: post
categories: website
---

Nuestro cerebro no está diseñado para comprender probabilidades de forma intuitiva. Incluso en situaciones simples, como lanzar una moneda, surgen dudas. Consideremos este escenario:

- "He lanzado una moneda 5 veces, y en todas ha salido cara."

Aunque esto parece improbable, tiene la misma probabilidad que cualquier otra secuencia de 5 lanzamientos. Por ejemplo, siendo "C" cara y "S" sello, las secuencias:

- C, C, C, C, C
- C, S, C, S, C

Ambas secuencias resultan igual de probables porque deben cumplirse en ese orden específico, lo que las hace igual de únicas e improbables una de la otra. No estamos contando el número de caras o sellos, sino comparando dos secuencias específicas.

**¿Por qué parece más sorprendente obtener 5 caras seguidas?** Esto se debe a la **falacia del jugador**, la creencia equivocada de que los eventos pasados afectan los futuros. Imaginemos que estamos viviendo el primer escenario y ya han salido 4 caras. Naturalmente, tendemos a pensar que "debería" salir un sello para corregir la tendencia.

En algunos juegos es útil sospechar esto, ya que podría advertirnos que nos están haciendo trampa. Sin embargo, si estamos seguros que no es el caso, debemos recordar que la moneda no tiene memoria, por lo que cada resultado es independiente del anterior. Por ello, siempre debemos esperar un 50% de probabilidad sin importar los resultados anteriores.

Ahora bien, si hacemos 1000 lanzamientos y cada uno es independiente del otro, ¿cómo es que esperamos obtener cerca de 500 caras y 500 sellos?

**Aquí es donde puede fallar nuestra intuición**. Cuando eso ocurre, podemos apoyarnos en hacer cuentas para dar sentido a la solución. 

Tomemos un ejemplo sencillo: si lanzamos una moneda dos veces, las posibles combinaciones son:

| Combinación | Número de veces que cae Cara (C) |
| ----------- | -------------------------------- |
| C, C        | 2                                |
| C, S        | 1                                |
| S, C        | 1                                |
| S, S        | 0                                |

Aquí vemos que hay más formas de obtener 1 cara que de obtener 0 o 2. Esto ocurre para cualquier número de lanzamientos; habrá más formas de obtener un número intermedio de caras y sellos. **Por eso, si hacemos 1000 lanzamientos, es más probable obtener alrededor de 500 caras y 500 sellos.**

Este enfoque también resuelve nuestro problema inicial. Con una tabla de 5 lanzamientos, encontraremos una fila para la secuencia "C, C, C, C, C" y otra para "C, S, C, S, C". Veremos que ambas combinaciones aparecen sólo una vez de 32 posibles, haciéndolas igual de probables una de la otra.

Para entender la probabilidad, suele ser necesario pensar a largo plazo o en una gran repetición de eventos. Por este motivo nuestra mente no logra entenderla de forma intuitiva, ya que se enfoca en resultados locales y de corto plazo. En vez de caer en ese error, es preferible apoyarse en hacer cuentas para encontrar el resultado correcto. Al hacer esto encontramos también sentido de los resultados, lo que nos da mayor entendimiento del tema. Intentemos resolver ahora un problema bastante famoso.

### El problema de Monty Hall

Imaginemos que estamos en un concurso donde se debe elegir entre tres puertas: detrás de una se encuentra un carro (el premio deseado) y detrás de las otras dos, cabras (premios no deseados). Después de elegir una puerta, el presentador, que sabe lo que hay detrás de cada puerta, abre una de las otras dos puertas, revelando una cabra. A continuación, se te ofrece la opción de mantener tu elección original o cambiar a la otra puerta cerrada. ¿Qué es mejor, quedarse con la puerta inicial o cambiar?

Lo primero que debemos hacer es entender el problema para ver si tiene una solución intuitiva. Si no la encontramos, siempre se puede revisar los escenarios posibles para hacer cuentas.

En el problema debemos hay dos elecciones. ¿Son estas independientes una del otra? a simple vista, en la primera escogemos entre tres puertas, y en el siguiente entre dos; no parece que dependa una de la otro. Sin embargo, la puerta que abre el presentador sí depende de nuestra elección inicial.

Supongamos que al inicio elegimos una puerta donde hay una cabra. Ahora el presentador debe abrir una puerta donde haya una cabra. No puede abrir la puerta que elegimos, por lo que debe abrir la otra con la segunda cabra. ¿Qué puerta queda restante? La que tiene el carro. En ese escenario, ganaremos si cambiamos de puerta. Es así como nuestra segunda elección depende de la primera.

Aún estando convencido de que las elecciones son dependientes y que no debo evaluarlas individualmente, ¿cómo sé cuáles son mis probabilidades? Aquí es cuando hacemos cuentas con los escenarios posibles.

Supongamos que la configuración del juego es que el carro está en la puerta 3. Hay tres escenarios posibles: escoger la puerta 1, 2 y 3. Supongamos que en los 3 escenarios vamos a cambiar de puerta.

- Si escogemos la puerta 1 (donde hay una cabra), el presentador tendrá que abrir la puerta 2. Si cambiamos de la puerta 1 a la 3, ganamos.
- Si escogemos la puerta 2 (donde hay una cabra), el presentador tendrá que abrir la puerta 1. Si cambiamos de la puerta 2 a la 3, ganamos.
- Si escogemos la puerta 3, el presentador puede abrir la puerta 1 o 2, ambas tienen cabras. Si cambiamos de la puerta 3, perdemos.

Podemos observar que ganaríamos en 2 escenarios de 3 posibles si cambiamos de puerta. Esto ocurre para cualquier configuración del juego. Ahora si no cambiamos de puerta en cada escenario, veremos que el resultado se invierte: ganaríamos solo en 1 escenario de tres posibles. Por lo tanto al cambiar de puerta tenemos una probabilidad de 2/3 o 66%, en vez de 1/2 o 50%, que podríamos pensar viendo de forma individual la segunda elección entre las dos puertas.


### Bonus

Para mejorar no solo el pensamiento estadístico sino en general el pensamiento crítico, es necesario conocer el Teorema de Bayes. Este consiste en estimar probabilidades dado un conjunto de evidencias. Esto puede aplicarse en múltiples áreas, como la medicina, el aprendizaje de máquina y la economía.

El teorema de Bayes es fundamental en este contexto y merece una explicación detallada. Sin embargo, no creo que pueda hacerlo mejor que el [video](https://www.youtube.com/watch?v=HZGCoVF3YvM) de 3Blue1Brown. Sus visualizaciones son excepcionalmente ilustrativas y hacen que el concepto sea mucho más fácil de entender. Destaco una frase importante de ese video:

> "La evidencia no debe determinar nuestras creencias, sino actualizarlas."
> — Grant Sanderson

# Referencias

Pensar rápido, pensar despacio - Daniel Kahneman

[Bayes theorem, the geometry of changing beliefs](https://www.youtube.com/watch?v=HZGCoVF3YvM)
