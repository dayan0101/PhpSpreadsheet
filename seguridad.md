# Seguridad

Las APIs son cada vez más vulnerables a los ataques de seguridad. Pero lo cierto es la que mayoría de amenazas se pueden prevenir y evitar. Por eso en nuestra plataforma empleamos protocolos de seguridad que nos permiten evitar la mayoría de amenazas.

## Conexiones seguras HTTPS

En **ePayco** se fuerzan todos los servicios a HTTPS empleando TLS, incluyendo nuestro sitio web público y nuestro dashboard. Regularmente, se auditan los detalles de nuestras implementaciones, incluyendo los certificados autorizando su uso y el cifrado que soporta. Se usa HSTS para asegurar que los navegadores interactúen con ePayco sólo por HTTPS.

## Encriptado de data sensible y comunicaciones

Todas los datos de las tarjetas de créditos son encriptadas  y se genera un token card para cada una de ellas, el cuál se emplea para futuras transacciones. Las llaves para desencriptar son guardadas en máquinas separadas. Nadie en ePayco puede obtener los datos sensibles. En ePayco la infraestructura para almacenamiento, desencriptar y enviar los datos de tarjetas de créditos corren en ambientes separados y no se comparten las mismas con nadie ni en servicios primarios \(API, página web y otros\).

## Validación de parámetros

 En la API de nuestra plataforma adicional a los protocolos de comunicación y encriptado de dato, hacemos validación de todos los datos **entrantes verificando su formato, su validez y garantizar que no pueda causar daño al sistema.** Empleamos un serializador JSON para codificar correctamente los datos enviados por el cliente y evitar la ejecución de código incluido dentro de la información introducida por el cliente.

