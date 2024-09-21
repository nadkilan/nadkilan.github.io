---
title:  "El valor del riesgo"
mathjax: true
layout: post
categories: website
---


Supongamos que estamos en un concurso, y nos dan a elegir entre dos opciones:

1. Ganar $85 seguros.
2. 90% de probabilidad de ganar $100 y 10% de no ganar nada.

¿Qué elección deberíamos escoger? lo más razonable parece asegurar la ganancia en vez de arriesgarse, ¿pero y si en realidad lo más sensato fuera buscar el riesgo?

Aunque este problema está sujeto a la subjetividad, ya que no todos valoramos de la misma manera las ganancias y las pérdidas, explicaré por qué la segunda opción es más rentable, presentando algunos argumentos (o excusas, si se quiere ver) para justificar esa elección.

### Resolviendo el problema

Imaginemos que jugamos el juego 10 veces con la misma elección. ¿Con cuál elección ganaríamos más dinero?

Con la primera elección, ganaríamos $85 las diez veces, dando un total de $850.
Con la segunda, la probabilidad nos dice que ganaremos 9 de cada 10 veces, por lo que deberíamos ganar un total de $900. Dividiendo este total sobre los 10 juegos, obtenemos que nuestra ganancia es equivalente a si hubiéramos ganado $90 por juego.

Claramente estamos jugando con probabilidades, así que es posible que perdamos una, dos o incluso tres veces. Pero la probabilidad apunta a que ganaremos 9 de cada 10 juegos, y esa probabilidad se hace más confiable a mayor número de juegos.

Si jugamos este juego 1000 veces escogiendo la opción dos, donde hay un riesgo, **siempre** vamos a ganar más que escogiendo 1000 veces la opción segura. Nuevamente si dividimos el total ganado sobre el número de juegos, obtendremos que en promedio es como si hubiéramos ganado $90 por juego contrario a los $85 ganados por la opción segura.

Podemos decir que el **valor esperado** de la elección dos es de $90, que calculamos fácilmente multiplicando la probabilidad (0.9) por el valor de ganancia ($100). Es en este sentido que la elección dos otorga un mayor beneficio que la primera.

La primer pregunta que surge es: ¿Qué importa si eso se cumple para 1000 juegos? Yo voy a jugarlo una sola vez, y si pierdo, no gano nada. En realidad, le doy toda la razón a ese argumento. Existen varios motivos por los que, naturalmente, nuestra mente siente una **aversión a la pérdida** y nos dice que la opción segura es la más sensata.

Conocer esos motivos nos da un mayor entendimiento de cómo funcionamos en la toma de decisiones, por lo que recomiendo leerlos. De momento quiero exponer algunos argumentos (o excusas) para tratar de ver el asunto de forma diferente.

### La vida como un juego

Ya sabemos que la opción 2 es mejor que la 1 jugando muchos juegos, nuestro problema es que no parece que podamos repetir el juego. Sin embargo, imaginemos que se presenta otra oportunidad similar al día siguiente. Hay una elección entre tomar un riesgo con un valor esperado más alto que la elección de la opción segura.

En este caso, ¿pensaríamos lo mismo del día anterior? creo que podríamos identificar que, en efecto, tanto el juego de ayer como el de hoy pueden verse como una repetición de escenarios, tal y como hicimos al comienzo. Del mismo modo, en la medida que encontremos oportunidades similares, podemos enmarcarlas como un grupo de escenarios repetidos, donde elegir el riesgo resulta más rentable que la opción segura.

Lo cierto es que la vida está llena de decisiones por tomar y podemos estar seguros de encontrar numerosos escenarios donde debemos elegir entre arriesgarnos o no, solo es cuestión de identificarlos y enmarcarlos como un gran juego, en vez de verlo cada escenario individualmente.

Esto es muy importante, ya que estamos hablando de toma de decisiones en general, no solo en escenarios financieros. Veamos un ejemplo más cotidiano:

Supongamos que quieres hablarle a la persona que te gusta. Debes elegir entre hacerlo o no. ¿Cómo podemos modelar este escenario para decidir correctamente?

1. No le hablamos y no ganamos nada.
2. Si le hablamos y nos ignora, no ganamos nada.
3. Si le hablamos y nos responde, ganamos algo.

Podemos ver fácilmente que la opción 3 es la única que puede arrojarnos un valor positivo, aún si tuviera una baja probabilidad de que ocurra, su valor esperado sigue siendo mayor que 0. Algunos pueden argumentar que en la opción dos se perdería, en forma de pasar vergüenza, pero el único resultado real es que no ocurrió nada, lo mismo a si no hubiéramos hecho nada; ¿Por qué nos daría vergüenza intentar ganar?

Este es un ejemplo sencillo de toma de decisiones de la cotidianidad. Podemos observar que, aunque inexacto, puede darnos algo de racionalidad sobre por qué puede ser mejor actuar. Asignemos valores de pérdida y ganancia al ejemplo:

1. 90% de probabilidad que nos ignore. Perdemos 1 punto por la vergüenza de ese resultado (no le damos mucha importancia a la vergüenza, por lo menos intentamos).
2. 10% de probabilidad de que nos responda. Ganamos 10 puntos de felicidad.

Calcular el valor esperado de este escenario sería calcular el valor esperado de la posible ganancia y restar el de la posible pérdida, entonces es:

$$ (0.1\times10) - (0.9\times1) = 1 - 0.9 = 0.1 $$

Como podemos observar, obtenemos un valor esperado positivo, lo que indica que en promedio ganamos al hablarle.

> ADVERTENCIA: En este ejemplo, debemos ser cautelosos con la idea de la repetición de escenarios. No queremos escribirle 100 veces a una persona para evaluar la probabilidad. Recordemos que cada escenario debe ser independiente del otro. Este escenario es dependiente ya que escribirle una vez puede afectar la probabilidad de que responda al escribirle una segunda vez.

Ciertamente, no hace falta hacer estos cálculos y estimaciones para cada decisión que tomemos. Sin embargo, es una forma de motivarnos y convencernos que está bien tomar riesgos en la vida; si los identificamos y analizamos racionalmente (esto es, sin ser presa de emociones como el miedo o el arrepentimiento), sabremos que a lo largo de nuestra vida saldremos más beneficiados que al no arriesgarnos.

Si esta razón no es lo suficientemente convincente, existe otra que puede resultar o bien reveladora o totalmente inútil, según la personalidad de cada uno.

### Apología de un ludópata

Para las personas más curiosas y amantes de la ciencia: ¿No es increíble el universo? desde el electrón hasta las estrellas, todo se rige por procesos tan complejos, todo interactúa de forma tan perfecta para que todo exista. Al lanzar una moneda, ocurre toda una sinfonía de procesos, como la fuerza en que se lanzó, el ángulo, el viento, etc. Para nosotros es azar, pero para el universo es una tocar cada nota de la sinfonía.

Si un amigo nos ofrece una apuesta de lanzamiento de moneda, donde ganamos $10 si cae una cara y perdemos $10 si cae la otra, es normal que esa apuesta no nos anime mucho. Sin embargo, ante la poca cantidad que podríamos perder, podríamos aceptar solo para ver qué ocurre. Podemos decir entonces: "No estoy apostando, estoy pagando para ver cómo el universo decide un resultado".

Quiero aclarar que no promociono ningún tipo de apuesta. En cambio estoy planteando una forma de disminuir nuestro miedo a perder, o a redefinir lo que es una pérdida para nosotros. ¿Qué pasa si perdemos poco? ¿acaso no estaríamos dando un poco de emoción (de forma muy mesurada) a nuestra vida, al mismo tiempo que decidimos participar de un juego junto a nuestro amigo?

A diferencia de los casinos, donde la casa siempre gana, acá tenemos un valor esperado de 0. No estamos abandonando nuestra racionalidad, estamos ejercitando nuestra capacidad para aceptar una pérdida de forma divertida o contemplativa.

Claramente es posible "contemplar al universo decidir un resultado" de forma gratuita (en internet por ejemplo). Pero si nos fascina el universo, por qué no participar de forma más activa en él? Cuanto más lo hagamos, más oportunidades tendremos de jugar y nuestra vida será más como un juego, en vez de un campo minado de cosas que debemos evitar.

### Conclusión

El valor esperado resulta útil para tomar decisiones bajo incertidumbre. Como vimos en el primer ejemplo, en promedio es más rentable tomar la elección de riesgo que la elección segura. Bajo este concepto, podemos identificar que ciertos escenarios pueden ser evaluados de una forma similar, lo que puede motivarnos a no tener tanta aversión a la pérdida. Sin embargo, debemos considerar algunos aspectos importantes.

En primer lugar, recordemos que los escenarios deben ser independientes, repetitivos y no simbolizar una gran pérdida. En segundo lugar, las evaluaciones de ganancias y pérdidas son **subjetivas**, así que uno mismo es quien debe estimar esos valores bajo sus criterios.
Por último, si bien enfrentar el miedo a perder puede enriquecer nuestra vida en algunos aspectos, debemos ser conscientes de cuándo el riesgo se convierte en imprudencia, especialmente en situaciones donde las pérdidas son significativas o donde el escenario es verdaderamente único.

Cuando logremos identificar y estimar correctamente los escenarios que se nos presenta en la vida, es cuando podremos tomar las mejores decisiones, en las cuales tendremos que enfrentar nuestras emociones como el miedo o el arrepentimiento. En palabras de Mark Twain:

> Dentro de veinte años estarás más decepcionado por las cosas que no hiciste que por las que hiciste.

# Referencias

Pensar rápido, pensar despacio - Daniel Kahneman
