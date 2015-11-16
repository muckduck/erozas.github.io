---
layout:     post
title:      "Plugins de emulación de channel strips"
subtitle:   "Los principales plugins que emulan el comportamiento de los channel strip"
author:     "Jorge"
header-img: "none"
---

### Plugins de emulación

Hay una serie de fabricantes que ha emulado canales de consola clásicos o legendarios, para usarlos dentro del secuenciador de una manera muy similar a como se usarian en la mezcla; entre los desarrolladores destacados de este tipo de plugins están: Waves y Universal Audio. 

Entre los canales que se han emulado tenemos los de EMI, SSL, Neve y API, de estos modelos el de SSL-4000 es el más extendido; entre los parámetros que se emularon están:

* Distorsión armónica: Los armónicos que generan todos los dispositivos no lineales, entre ellos las consolas.
* Distorsión de fase: Los cambios en la fase de la señal que producen principalmente los dispositivos que alteran la frecuencia, filtros y ecualizadores.
* Comportamiento de ruido: En algunas emulaciones se incluyen los ruidos de la fuente de alimentación y el ruido del tipo hiss.
* Comportamiento de los ecualizadores: Tanto las pendientes de los filtros, como los anchos de banda de las curvas de ecualización.
* Comportamiento de los compresores: En terminos de la razón, ataque, release, circuito de reducción de ganancia, etc.

#### EMI REDD 37 y 51 (Waves)

Es un plugin que emula un canal de las consolas REDD 37 y 51, dentro del plugin podemos elegir cual de ambos canales queremos usar; la diferencia principal entre ambos canales radica en que la consola REDD 37 usaba preamplificadores Telefunken V72 y la consola REDD 51 usa preamplificadores más modernos de la propia firma, llamados REDD47; veamos el procesamiento que ofrece esta emulación.

* Amp type: Nos permite seleccionar que consola se emula si la REDD 37 o REDD 51.
* Ganancia: Con este potenciómetro podemos hacer la estructura de ganancia de la señal o agregar distorsión a la señal, aumentando el nivel.
* Bass lift: Activa una curva del tipo shelving con 9 dB de ganancia, pensado para compensar el uso de micrófonos en figura de ocho; además se incorpora un pad para atenuar la señal.
* Ecualización: Emplea dos curvas de ecualización del tipo shelving, para bajos y agudos, en la curva de agudos podemos cambiar a una curva shelving al producir realces.
* Drive: Genera armónicos a la señal, valores altos van a generar un sonido distorsionado.
* Analog: Controla el nivel del ruido de fuente (hum) y del tipo hiss que se suma a la señal.
* Output: Controla el nivel de salida de la señal, para volver a la estrucutra de ganancia obtenida, esto puede ser usado para atenuar la señal si es que se decide usar mucha ganancia de entrada por el color, de tal manera de mantener el headroom.

#### EMI TG12345 (Waves)

Es un plugin que emula un canal de la consola de EMI TG12345, que es la consola reemplazante a la serie REDD de estado sólido; por lo que tiene un sonido más limpio y una sección de ecualización más completa en conjunto con un compresor, veamos el procesamiento que ofrece:

* Input: Con este potenciómetro podemos ajustar la estructura de ganancia de la señal o agregar distorsión a la señal, aumentando el nivel.
* Dynamics: Activa el compresor o limitador del canal, el mismo tiene un ataque fijo de 1 (ms) y un release variable con la perilla recovery. La función hold permite establecer una reducción de ganancia constante o continua en la compresión. Finalmente el botón SC-HP activa un filtro pasa altos en la señal que llega al circuito de detección, para comprimir menos bajas frecuencias.
* EQ: El canal dispone de dos curvas shelving en los extremos un una curva peaking en los medios, llamada presence. La curva de agudos puede transformarse en peaking si hacemos un realce y es shelving cuando cortamos, la curva de bajos es del tipo shelving.
* Ruoting: Nos permite escoger el orden de los procesos dentro del canal ya que el mismo modifica los resultados que vamos a obtener; podemos escoger entre EQ-DYN-PRES, DYN-EQ-PRES o EQ-PRES-DYN.
* Drive: Genera armónicos a la señal, valores altos van a generar un sonido distorsionado.
* Noise: Controla el nivel del ruido de fuente (hum) y del tipo hiss que se suma a la señal.
* Output: Controla el nivel de salida de la señal, para volver a la estrucutra de ganancia obtenida, esto puede ser usado para atenuar la señal si es que se decide usar mucha ganancia de entrada por el color, de tal manera de mantener el headroom.

#### API Vision (Universal audio)

Es un plugin que emula un canal de la consola moderna de API de producción actual llamada Vision, el canal consiste de varios módulos que contienen el procesamiento necesario para mezcla: filtros, ecualización y dinámica. Veamos los procesos

* Gain 212L: Con este potenciómetro podemos ajustar la ganancia de entrada de la señal, para establecer el headroom necesario, además podemos usarlo para agregar distorsión a la señal; también disponemos de un atenuador de 20 dB y un inversor de polaridad.
* Filtrado 215L: Consiste en un filtro pasa altos HPF y un filtro pasa bajos o LPF, de frecuencias variables, el botón Dyn-Sc envía los filtros hacia el circuito de Side chain de la sección dinámica, para obtener compresiones acotadas en frecuencia.
* Gate/Expander 235L: Incorpora un expansor o compuerta seleccionables con umbral, depth y release variables; podemos elegir entre tiempos de ataque fijos.  
* Compresor/Limitador 225L: Incorpora un compresor o limitador con umbral, razón y release variables; el ataque y knee puede ser seleccionado entre algunas opciones fijas.
* EQ 550L: Ecualizador del tipo 550B con cuatro bandas de ecualización de frecuencias y ganancias seleccionables, las curvas de los extremos pueden ser shelving o peaking y la de los medios son peaking; el botón Pre-Dyn coloca la sección de EQ antes del compresor. El botón SC mueve la sección de EQ hacia el circuito de side chain de la sección dinámica.
* Output: Controla el nivel de salida de la señal, esto puede ser usado para atenuar la señal si es que se decide usar mucha ganancia de entrada por el color, de tal manera de mantener el headroom.

#### Neve 88RS (Universal audio)

Es un plugin que emula un canal de la consola moderna emblema de AMS/NEVE de producción actual 88RS, el canal  contiene el procesamiento necesario para mezcla: filtros, ecualización y dinámica. Veamos los procesos:

* Gain/Preamp: En esta sección tenemos la posibilidad de ajustar la ganancia del canal para mezclar o la ganancia del micrófono al grabar, seleccionando el tipo de fuente adecuado; además se incluye un atenuador de 20 dB y un inversor de polaridad.
* Filtrado: Consiste en un filtro pasa altos HPF y un filtro pasa bajos o LPF, de frecuencias variables continuamente.
* Gate/Expander: Incorpora un expansor o compuerta seleccionables con umbral, range, histeresis y release variables continuamente; el ataque se puede variar entre rápido y lento. 
* Compresor/Limitador: Incorpora un compresor o limitador con umbral, razón, ganancia de salida y release variables continuamente, el ataque se puede variar entre rápido o lento. El botón SC-EQ envía la sección de ecualización al circuito de Side chain del compresor/compuerta, para obtener compresión selectiva en frecuencia.
* EQ: Ecualizador de cuatro bandas de ecualización, las dos bandas de los extremos (HF y LF) pueden ser shelving o peaking y las dos bandas de medios son peaking paramétricas. Cuando las bandas de los extremos son peaking se puede escoger que el ancho de banda sea más selectivo con el botón Hi-Q. Con el botón P-Dyn se puede colocar la sección de ecualización antes o después de la sección dinámica.
* Output: Controla el nivel de salida de la señal, esto puede ser usado para atenuar la señal si es que se decide usar mucha ganancia de entrada por el color, de tal manera de mantener el headroom.

#### SSL 4000 (Waves)

Es un plugin que emula un canal de la consola más famosa y usada de SSL la serie G/E-4000, si bien nos vamos a centrar en el plugin del desarrollador Waves, también hay versiones similares de Universal audio, SSL Duende, Native instruments y T racks. El canal contiene el procesamiento necesario para mezcla: filtros, ecualización y dinámica; la principal diferencia entre las versiones E y G radica en el diseño del ecualizador y en las opciones de ruteo de la señal; veamos los procesos en ambos canales:

##### E-4000
* Gain: En esta sección tenemos la posibilidad de ajustar la ganancia de entrada del canal para mezclar, también hay un inversor de polaridad; esta parte del canal se situa abajo a la derecha.
* Filtrado: Consiste en un filtro pasa altos HPF y un filtro pasa bajos o LPF, de frecuencias variables continuamente; al colocar el botón Split se hace que el filtrado vaya antes que la sección de dinámica.
* EQ: Ecualizador de cuatro bandas de ecualización, las dos bandas de los extremos (HF y LF) pueden ser shelving o peaking y las dos bandas de medios son peaking paramétricas. Al apretar el botón Bell las bandas de los extremos se transforman a peaking; con el botón EQ TO DYN SC se puede hacer que la ecualización salga del camino de la señal y vaya al circuito de side chain de la sección dinámica; con el botón EQ TO By pass se desactiva por completo la sección de EQ.
* Compresor/Limitador: Incorpora un compresor o limitador con umbral, razón y release variables continuamente, el ataque se puede variar entre rápido o lento, con el botón Dyn to CH OUT hacemos que la sección de dinámica vaya después de la ecualización.
* Gate/Expander: Incorpora un expansor o compuerta seleccionables con umbral, range y release variables continuamente, el ataque se puede variar entre rápido o lento; con el botón gate transformamos el expansor en compuerta de ruido. 
* Analog: Con este interruptor activamos o desactivamos el ruido de fuente(hum) y del tipo hiss emulado del canal.
* Output: Provee un fader para controlar el nivel de salida de la señal y mantener el headroom en todo momento.

##### G-4000

* Gain: En esta sección tenemos la posibilidad de ajustar la ganancia de entrada del canal para mezclar, también hay un inversor de polaridad; esta parte del canal se situa abajo a la derecha.
* Filtrado: Consiste en un filtro pasa altos HPF y un filtro pasa bajos o LPF, de frecuencias variables continuamente; al colocar el botón Split se hace que el filtrado vaya antes que la sección de dinámica.
* EQ: Ecualizador de cuatro bandas de ecualización, las dos bandas de los extremos (HF y LF) son shelving  y las dos bandas de medios son peaking paramétricas; en las banda HMF de medios al apretar el botón HMF x 3 se multiplica el valor de la frecuencia seleccionada por tres, en la banda LMF al apretar el botón LMF % 3 se divide el valor de la frecuencia entre tres. Con el botón EQ TO FLT DYN SC se puede hacer que la sección de filtrado salga del camino de la señal y vaya al circuito de side chain de la sección dinámica; con el botón EQ TO By pass se desactiva por completo la sección de EQ.
* Compresor/Limitador: Incorpora un compresor o limitador con umbral, razón y release variables continuamente, el ataque se puede variar entre rápido o lento, con el botón Dyn to CH OUT hacemos que la sección de dinámica vaya después de la ecualización, con el botón DYN TO BYPASS desactivamos por completo esta sección.
* Gate/Expander: Incorpora un expansor o compuerta seleccionables con umbral, range y release variables continuamente, el ataque se puede variar entre rápido o lento; con el botón gate transformamos el expansor en compuerta de ruido. 
* Analog: Con este interruptor activamos o desactivamos el ruido de fuente(hum) y del tipo hiss emulado del canal.
* Output: Provee un fader para controlar el nivel de salida de la señal y mantener el headroom en todo momento.

#### Channel strips digitales

En la mayoría de los secuenciadores modernos profesionales los desarrolladores incluyen un plugin llamado channel strip, que agrupa el procesamiento necesario para mezclar al igual que las emulaciones que hemos abordado; sin embargo la forma de implementar el  procesamiento en este caso es más bien transparente, por lo que podriamos colocar a estos plugins dentro de lo que consideramos de precisión. Veamos el procesamiento típico de estos plugins

* Gain o input: En esta sección tenemos la posibilidad de ajustar la ganancia de entrada del canal para mezclar, también suele haber un inversor de polaridad.
* Filtrado: Por lo general consiste en un filtro pasa altos y pasa bajos modificables, tanto en la frecuencia de corte como la pendiente.
* EQ: En general vamos a encontrar un ecualizador del tipo paramétrico de entre cuatro a seis bandas de ecualización, además podemos cambiar algunas de estas bandas a shelving conforme lo necesitemos. 
* Compresor/Limitador: Incorpora un compresor con todos los parámetros ajustables por el usuario: umbral, razón, ataque, release e incluso la forma del knee; en algunos casos podemos ecualizar la señal que ingresa al circuito de side chain , para lograr resultados dependientes de la frecuencia.
* Gate/Expander: Se incorpora un expansor o compuerta con todos los parámetros seleccionables por el usiario: umbral, razón, range, ataque, release y hold. 
* Orden de procesos: En algunos casos podemos alterar el orden en el que se disponen las instancias de procesamiento, por ejemplo: EQ-DYN-FILT o FILT-DYN-EQ.
* Output: En esta parte se controla el nivel de salida de la señal, para mantener el headroom de la señal en todo momento.