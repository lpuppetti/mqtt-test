# mqtt-imp

Implementacion basica de prueba del protocolo MQTT.

Pasos para ejecutar:

-Clonar proyecto.

-Instalar mosquitto mqtt broker.

-Desde la consola ejecutar $ mvn exec:java@publish (posicionado en el directorio mqrrt-imp). Esto inicia la clase publisher, solicitara que se ingrese un topico(EJ: prueba/sensor1) y comenzara a publicar mensajes.

NOTA: Se puede ejecutar mas de una instacia de la clase Publiser abriendo varias consolas e insgresando otro topico(EJ: prueba/sensor2)

-Abrir nueva consola y ejecutar $ mvn exec:java@suscribe. Esto inicia la clase Susbriber, solicitara que se ingrese un topico de los ingresados anteriormente y comenzara a mostrar los mensajes recibidos.

NOTA: Si se ejecutaron mas de una instancia de Publisher se puede conectar a un especifica a travez del topico(EJ: prueba/sensor1) o a
varias con el comodin #(EJ: prueba/#).

