# Sistema de Gestión de Inventario

## Programación Básica – Examen Parcial Práctico

Este proyecto para el examen consiste en un programa de sistema de gestión de inventario para una tienda.  
El sistema permite representar productos electrónicos y productos de alimentos, mostrando su información y calculando el impuesto correspondiente según el tipo de producto.

## Conceptos de Programación Orientada a Objetos utilizados

El proyecto utiliza los siguientes conceptos fundamentales:

- Encapsulación
- Herencia
- Polimorfismo
- Uso de clases y objetos

## Estructura del Programa

### Clase Base: productos

Esta clase representa un producto general y contiene los atributos comunes a todos los productos:

- nombre
- codigo
- precio
- cantidad

También incluye:

- Constructor para inicializar los datos del producto
- Propiedades públicas para acceder a los atributos
- Método `MostrarProducto()` para mostrar la información del producto
- Método virtual `CalcularImpuesto()` que será sobrescrito por las clases derivadas

### Clase productoElectronico

Esta clase hereda de la clase `productos`.

Atributo adicional:

- GarantiaMeses

El método `CalcularImpuesto()` calcula el impuesto del producto electrónico aplicando el **18% (ITBIS)** al precio.

### Clase productoAlimento

Esta clase también hereda de la clase `productos`.

Atributo adicional:

- FechaVencimiento

El método `CalcularImpuesto()` calcula el impuesto aplicando **8%** al precio del producto.

## Funcionamiento del Programa

En el método `Main()` se crean dos objetos:

- Un producto electrónico (Laptop)
- Un producto de alimento (Arroz)

El programa muestra:

- Información del producto
- Garantía o fecha de vencimiento
- Impuesto calculado

## Ejemplo de salida

Producto Electronico  
Producto: Laptop  
Codigo: 1001  
Precio: 45000  
Cantidad: 5  
Garantia: 12 meses  
Impuesto: 8100  

Producto Alimento  
Producto: Arroz  
Codigo: 2001  
Precio: 2000  
Cantidad: 10  
Fecha vencimiento: 12/12/2026  
Impuesto: 160  

## Autor

Estudiante: Ancell Araujo Valdez  
Asignatura: Programación Básica  
Profesor: Ing. Gamalier Reyes del Carmen
