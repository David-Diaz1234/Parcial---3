# Parcial---3
# Proyecto: Tienda en Línea 

**Integrantes:** David Santiago Diaz Jimenez
**Link del Repositorio:** https://github.com

---

## 1. Alcance del Proyecto

### Lo que SÍ tendrá el sistema:
* **Catálogo:** Una lista simple de productos divididos en categorías básicas (Ropa y Tecnología).
* **Carrito:** Opción para agregar productos y calcular el total acumulado.
* **Descuentos (Área de cambio 1):** Poder aplicar un descuento fijo al total (como un Cupón del 10% o Descuento de Temporada).
* **Métodos de Pago (Área de cambio 2):** Opción de elegir pagar con Tarjeta o Efectivo (simulado con mensajes simples en pantalla).
* **Extras (Área de cambio 3):** Opción de agregar "Empaque de Regalo" o "Garantía" a un producto incrementando su costo.

### Lo que NO tendrá el sistema:
* **Sin Base de Datos Real:** Todos los productos y el carrito se guardan en listas de Java (ArrayList) en la memoria mientras el programa esté corriendo.
* **Sin Conexión Externa:** No realiza cobros con tarjetas reales ni se conecta a pasarelas de pago en internet.

---

## 2. Requisitos del Sistema

### Requisitos Funcionales (Lo que hace la aplicación)
* **RF-01:** El sistema debe mostrar la lista de productos disponibles en pantalla.
* **RF-02:** El sistema debe permitir al usuario añadir productos a su carrito de compras.
* **RF-03:** El sistema debe calcular el precio total aplicando el descuento seleccionado.
* **RF-04:** El sistema debe permitir sumarle extras opcionales (como empaque de regalo) a un producto.
* **RF-05:** El sistema debe mostrar una factura final en texto con el resumen de la compra.

### Requisitos No Funcionales (Cómo está construida)
* **RNF-01:** La aplicación debe estar desarrollada completamente en lenguaje Java.
* **RNF-02:** El sistema debe funcionar mediante una interfaz por consola y una interfaz gráfica sencilla compartiendo el mismo núcleo lógico.
