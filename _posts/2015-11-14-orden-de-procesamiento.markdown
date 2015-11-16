---
layout:     post
title:      "Orden de procesamiento sugerido"
subtitle:   "Los principales plugins que emulan el comportamiento de los channel strip"
author:     "Jorge"
header-img: "none"
---


### Orden de procesamiento sugerido

El lugar donde va cada instancia de procesamiento altera el resultado sobre la señal y por lo tanto como funciona el plugin, como hemos visto en las distintas emulaciones hay variantes para este orden; en ese sentido debemos buscar que el plugin funcione de manera óptima y así obtener mejores resultados en la mezcla. Este orden "estandard", se puede alterar ante situaciones específicas de mezcla.

1. **Ganancia:** El nivel de la señal debe ser el óptimo al entrar al plugin, para que el mismo pueda funcionar en el rango de operación en el que fue diseñado, recordemos ademas que en el sistema digital nosotros debemos crear el headroom para las señales. Se recomienda apuntar a -20 dB RMS para todas las señales del tipo constantes y -6 dBFS para las señales peak.
2. **Filtrado:** Las bajas frecuencias tienden a acumularse en la mayoría de las señales de la mezcla, este exceso produce enmascaramiento entre los distintos elementos además de falta de separación en el estéreo; por si esto fuera poco los compresores actúan sobre el nivel de la señal y si la misma tiene ruidos de baja frecuencia, la compresión se activa en falso. Se sugiere usar en prácticamente todos los canales un filtro pasa altos o HPF, para atenuar toda la energía sobrante de bajas frecuencias.
3. **Dinámica:** Tanto la compresión como la expansión se suelen aplicar después del filtrado y antes de la ecualización, ya que de lo contrario las ecualizaciones aditivas activarian la compresión contrarrestando su efecto en gran medida. 
4. **Ecualización:** Se suele usar después de la sección de dinámica, para que los cambios frecuenciales se puedan escuchar por completo; se recomienda en general usar técnicas de EQ sustractivas para limpiar las zonas problemáticas y usar EQ aditiva en última instancia para embellecer el sonido, de esta manera evitamos el enmascaramiento y ganamos headroom para la mezcla.
5. **Nivel de salida:** Para mantener la estructura de ganancia, se recomienda siempre revisar el nivel de salida de la señal y en especial si hemos generado EQ aditiva, de esta manera podemos atenuar la señal para mantener el headroom de la mezcla.