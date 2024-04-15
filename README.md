# Simulador de Tarjeta de Crédito en Java 🛒💳🏦

## Características
**Consulta de saldo**: Muestra el saldo actual disponible en la tarjeta.

**Lanzamiento de compra**: Permite realizar una compra si hay suficiente saldo disponible. 
Si la compra se realiza con éxito, se registra en la lista de compras.

## Uso
- Crea una instancia de TarjetaDeCredito proporcionando un límite de crédito inicial.
- Utiliza el método lanzarCompra(Compra compra) para intentar realizar una compra. 
- Si el saldo es suficiente, la compra se registra y el saldo se actualiza.
- Consulta el saldo actual y la lista de compras utilizando los métodos getSaldo() y getListaDeCompras().


## Instrucciones de Uso
Para ejecutar esta simulación, sigue estos pasos:

1. Asegúrate de tener Java instalado en tu sistema.
2. Descarga o clona este repositorio en tu máquina local.
3. Abre una terminal y navega hasta la carpeta que contiene el archivo `Principal.java`.
4. Compila el código con el comando `javac Principal.java`.
5. Ejecuta el programa con `java Principal`.

## Ejemplo de Uso
 Java

public static void main(String[] args) {
    // Crear una tarjeta de crédito con un límite de 1000
    TarjetaDeCredito miTarjeta = new TarjetaDeCredito(1000);

    // Intentar lanzar una compra de 200
    Compra compra1 = new Compra("Tienda A", 200);
    boolean exito = miTarjeta.lanzarCompra(compra1);

    if (exito) {
        System.out.println("Compra realizada con éxito. Saldo restante: " + miTarjeta.getSaldo());
    } else {
        System.out.println("Saldo insuficiente para la compra.");
    }
}


Requisitos
Java 8 o superior.
