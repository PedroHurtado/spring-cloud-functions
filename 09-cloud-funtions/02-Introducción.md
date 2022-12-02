# Introduccion a Spring Cloud Function

Permite programación reactiva, imperativa o hibrida

Permite exponer funciones como servicios http

Permite exponer funciones como streams

Es tan sencillo como definir un metodo en una clase decorarlo con @Bean y que devuelva cualquiera de las siguiente interfaces funcionales de java.util.function

Supplier<O>

Function<I, O>

Consumer<I>

```Java
@SpringBootApplication
public class Application {

  @Bean
  public Function<Flux<String>, Flux<String>> uppercase() {
    return flux -> flux.map(value -> value.toUpperCase());
  }

  public static void main(String[] args) {
    SpringApplication.run(Application.class, args);
  }
}
```
