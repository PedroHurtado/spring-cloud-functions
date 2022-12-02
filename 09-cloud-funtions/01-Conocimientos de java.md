# Conocimientos de Java

## Interface funcional.

Es aquella interface que solo posee un metodo abstracto y por tanto puede ser instanciada mediante una expresión lambda

```Java
     public interface Operation<T>{
        T apply(T a, T b)
     }

     Operation<int> sum  =  (a,b)->a+b;
     Operation<int> multiply= (a,b)->a*b;
     Operation<int> subtract= (a,b)->a-b;
     Operation<int> divide=  (a,b)->a/b;


     sum.apply(5,3); //8
     multiply.apply(5,3); //15
     subtract.apply(5,5); //0
     divice.apply(4,2); //2


```

## Callback

Consiste en pasar una funcion como parametro a otra funcion, en java no son funciones puras sino interfaces funcionales

```Java
 var result = persons.stream().filter(byAge)
        .collect(Collectors.toList());
```

Evitar el uso de collect

## Clousure

Una clausura o closure es una función que guarda referencias del estado adyacente (ámbito léxico). En otras palabras, una clausura permite acceder al ámbito de una función exterior desde una función interior

```Java
     public Operation<Integer> sum(Integer a, Integer b){
        return ()->a+b
     }

     sum(5,3).apply()
```

## Reactor Project

Mono<T> 
    Retorna una stream reactivo de un solo elemento
Flux<T>
    Retorna una stream reactivo de n  elementos

Referencia

https://projectreactor.io/



