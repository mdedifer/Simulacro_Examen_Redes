# Simulacro_Examen_Redes

https://github.com/mdedifer/Simulacro_Examen_Redes

### P1: Modelos OSI y TCP/IP
a) Diferencias:
1.	Número de capas: El modelo OSI tiene 7 capas: (Física, Enlace de datos, Red, Transporte, Sesión, Presentación y Aplicación) mientras que el modelo TCP/IP tiene 4 (Acceso a red, Internet, Transporte y Aplicación). Con esto concluimos que el TCP/IP es más sencillo, teniendo agrupadas varias capas de OSI en una sola, como pueden ser:
  -	Capa de Aplicación (TCP/IP)=Capa de Aplicación + Capa de Presentación + Capa de Sesión (OSI)
  -	Capa de Acceso a Red (TCP/IP)= Capa de Enlace de Datos + Capa Física (OSI)
2. En cuanto a la orientación, el modelo OSI es más completo y teórico, pero TCP/IP es más práctico, basado en protocolos usados en redes reales y por ello mucho más utilizado que el OSI.
3. Como he comentado antes, la capa de Aplicación en el modelo OSI está separadas de las capas de Presentación y Sesión, lo que permite una mayor especificidad en la definición de funciones.

b) Ventajas y limitaciones de cada modelo:
1. Modelo OSI:
  Ventajas:
    - Es un modelo teórico y estructurado, lo que facilita el aprendizaje y la comprensión de cómo funcionan las redes.
    - Divide las funciones de red en 7 capas bien definidas, permitiendo una mayor especificidad y modularidad.
    - Es independiente de los protocolos, lo que lo hace aplicable a diferentes tecnologías
  Limitaciones:
    - Es más complejo y menos práctico para implementaciones reales.
    - Algunos protocolos no se ajustan perfectamente a su estructura, lo que dificulta su adopción en redes modernas.
    - No está tan ampliamente utilizado como el modelo TCP/IP.
  
2. Modelo TCP/IP:
  Ventajas:
    - Es un modelo práctico, basado en protocolos reales que son ampliamente utilizados en redes modernas.
    - Es más simple, con solo 4 capas, lo que facilita su implementación.
    - Está diseñado para funcionar en redes reales, lo que lo hace más relevante en la actualidad
  Limitaciones:
    - Al agrupar varias funciones en una sola capa tiene menor detalle y especificidad.
    - No proporciona una guía teórica tan clara como el modelo OSI.
    - Está más enfocado en protocolos específicos, lo que lo hace menos flexible para tecnologías nuevas o diferentes.

### P2: Función de la Capa de Transporte
La capa de transporte se encarga de garantizar la entrega confiable de datos entre los dispositivos de red, por lo que es una capa fundamental en ambos modelos.
* *En OSI*, la entrega de datos es:
  - En orden
  - Sin errores
  - Sin duplicados
  Usa protocolo TCP: Protocolo confiable para aplicaciones que requieren entrega precisa, como correo electrónico y transferencia de archivos.
* *En TCP/IP*, la entrega de datos es:
Usa protocolos:
  - TCP, al igual que en OSI
  - UDP: Protocolo no confiable, pero rápido, utilizado en aplicaciones como streaming de video y juegos en línea.

### P3: TCP vs UDP
* *Orientación a conexión:*
  TCP: Protocolo orientado a conexión. Establece una conexión previa entre emisor y receptor antes de transmitir datos.
  UDP: Es un protocolo no orientado a conexión. No requiere establecer una conexión previa.
* *Fiabilidad y control de errores:*
  TCP: Es fiable, garantiza la entrega de datos sin errores, en orden y sin duplicados. Utiliza confirmaciones (ACK) y retransmisiones.
  UDP: No es fiable, no garantiza la entrega de datos ni el orden. No utiliza confirmaciones ni retransmisiones.
* *Velocidad de entrega:*
  TCP: Más lento debido a los mecanismos de control de errores, confirmaciones y retransmisiones. Asegura que los datos lleguen en orden.
  UDP: Más rápido porque no tiene mecanismos de control de errores ni asegura el orden de los datos.
* *Ejemplos de aplicaciones:*
  TCP: Aplicaciones que requieren alta fiabilidad, como: - HTTP/HTTPS (navegación web) - FTP (transferencia de archivos) - SMTP (correo electrónico)
  UDP: Aplicaciones que priorizan la velocidad sobre la fiabilidad, como: - Streaming de video/audio - Juegos en línea - VoIP (llamadas por Internet)


28/03/25
