# 💻Arquitectura de Software

## ¿Que es?
Es el diseño de un sistema de software, que define sus **componentes**, **relaciones** e **interaccion**.

## Tipos
<details>
<summary><span style="font-size: 18px; font-weight: bold;">Arquitectura Monolítica</span></summary>

Todo el sistema funciona en un único componente
</details>

<details>
<summary><span style="font-size: 18px; font-weight: bold;">Arquitectura Cliente-Servidor</span></summary>

El sistema se divide en dos componentes, el cliente que solicita servicios a un servidor y funciona como interfaz para el usuario; y el servidor que provee estos servicios al cliente.
</details>

<details>
<summary><span style="font-size: 18px; font-weight: bold;">Arquitectura Distribuida</span></summary>

El sistema es dividido en varios componentes que se ejecutan en distintas máquinas.
</details>

<details>
<summary><span style="font-size: 18px; font-weight: bold;">Arquitectura Orientada a Servicios</span></summary>

El sistema se divide en servicios que pueden ser proporcionados por distintos proveedores, estos servicios se comunican entre sí.
</details>


## Importancia

- Garantiza que un sistema sea robusto.

- Permite la escalabilidad del sistema, podra adapdarse a las necesidades cambiantes.

- Facilita la mantenibilidad del sistema, haciendolo facil de entender y modificar.



# 🖌️Patrones de Diseño

## ¿Que son?
Son <mark style="background-color: #c7f6d4;">soluciones habituales</mark> a problemas recurrentes en el diseño de software.

▶️ No es una porcion especifica de codigo, es un concepto general para resolver un problema particular

> 📌
> Son planos ya testeados que se pueden personalizar para resolver un problema especifico.

## Clasificacion
Los patrones se clasifican por su proposito u objetivo.

1️⃣ **Patrones Creacionales** su objetivo es proporcionar mecanismos para crear objetos y clases flexibles y reutilizables.

2️⃣ **Patrones Estructurales** explican la forma en que se deben construir los objetos y las clases en estructuras mas grandes.

3️⃣ **Patrones de Comportamiento** se encargan de definir la comunicacion, interaccion y las responsabilidades entre los objetos.

## Ejemplos

### Factory Method
Es un patron de diseño creacional que nos proporciona una interfaz para crear objetos usando una superclase, que permite a sus subclases usar la misma interfaz para crear objetos diferentes.

![image](./img/factory.png)
> :bulb:
> En este caso tenemos una superclase llamada logistica, con toda la info base para realizar la logistica de envios. Esta superclase es la que nos proporciona la interfaz para crear objetos distintos como una logistica terrestre y una logistica maritima con propiedades en comun de la superclase y a la vez propias.

### Singleton
Es un patrón también creacional que nos asegura que una clase u objeto se crea una sola vez, es decir, tiene una única instancia. Esto permite que el objeto sea compartido y accedido de manera global.

⚠️ Este patrón es imposible de usar en un constructor normal, ya que al llamar al constructor, siempre se devolverá una nueva instancia.

⏫ Nos da la posibilidad de acceder a un objeto desde cualquier parte del programa, a la vez que evita que otro código sobrescriba esa instancia.
![image](./img/singleton.png)


