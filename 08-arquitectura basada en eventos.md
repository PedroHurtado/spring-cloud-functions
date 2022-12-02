# Arquitectura basada en eventos

Desacoplar servicios y procesar solicitudes de forma asincrona. Para ello vamos a necesitar tres actores:

Publicador

    Nos va a permitir publicar un mensaje a traves del broker mediante un topic o canal

Broker

    Almacena los mensajes del publicador y sirve los datos a los suscriptor

Suscriptor


    Recibe el mensaje del broker y lo procesa. Por tanto suscriptor y publicador no se conocen y están totalmente desacoplados



Referencias

https://cloudevents.io/

https://www.redhat.com/es/topics/integration/what-is-event-driven-architecture#:~:text=La%20arquitectura%20basada%20en%20eventos%20es%20un%20modelo%20y%20una,modelo%20tradicional%20basado%20en%20solicitudes.

https://aws.amazon.com/es/blogs/aws-spanish/arquitecturas-orientadas-a-eventos-en-aws/

https://github.com/spring-cloud/spring-cloud-function/tree/main/spring-cloud-function-samples/function-sample-cloudevent

Ejemplo con spring cloud

https://github.com/spring-cloud/spring-cloud-function/tree/main/spring-cloud-function-samples/function-sample-cloudevent