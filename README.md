# ASO2024TPs
TP 3
PUNTO 1

a- Después de ejecutar varias veces cada archivo, noté que CONHILOS.PY toma alrededor de 4.07 segundos desde el inicio de la compilación hasta que finaliza, mientras que SINHILOS.PY tarda aproximadamente 5.17 segundos. Al observar estos resultados, se puede ver una diferencia clara en los tiempos de ejecución entre ambos programas, siendo CONHILOS.PY notablemente más rápido que SINHILOS.PY. Aunque el tiempo total de ejecución es similar en cada repetición, varía unos milisegundos entre cada ejecución. Esta diferencia de velocidad se debe a que en CONHILOS.PY, mientras una tarea está en espera, otras pueden seguir ejecutándose.

b- Al comparar mis tiempos de ejecución con los de un compañero, noté que son similares, variando solo en milisegundos y sin grandes diferencias.

c- Al ejecutar el programa con las líneas 11, 12, 19 y 20 comentadas, observé que el valor final siempre es 0 y el tiempo de ejecución es de aproximadamente 0.015 segundos. Sin embargo, al descomentar esas líneas, el valor final ya no es 0 y el tiempo de ejecución aumenta a aproximadamente 2.01 segundos, con pequeñas variaciones. Esta diferencia se debe a que los dos bucles for que estaban comentados no realizaban ninguna acción relevante, pero incrementaban el tiempo de ejecución del programa.

Tambien agregar que ambos hilos utilizan la misma variable global llamada acumulador (zona critica), entonces ejecutando normalmente deberia dar 0, pero al ser una race condition puede llegar a suceder el caso de que el resultado no de lo correcto, debido a esto mismo, a que no hay ningun tipo de control sobre los hilos
