# Circuit Breakers

Al tener dependencias entre servicios y realizar llamadas sincronas entre ellos uno de los servicios puede fallar o tener una latencia muy alta. Si no utilizamos este patrón podemos provocar un comsumo de recursos muy alto.

Para ello debemos de marcar el servicio sobrecargado o caido como no disponible

Referencias.

https://spring.io/projects/spring-cloud-circuitbreaker

https://microservices.io/patterns/reliability/circuit-breaker.html