# Parcial---3

# Parcial de Patrones de Diseño: Proyecto en Java

**Integrantes:** David Santiago Diaz Jimenez
**Link del Repositorio:** https://github.com

---

## 1. Alcance del Proyecto

### Funcionalidades Incluidas (SÍ se implementará)
* **Catálogo de Productos:** Navegación por categorías (Ropa, Tecnología, Alimentos), cada una con sus propios atributos específicos.
* **Carrito de Compras y Cierre de Pedido:** Gestión de productos seleccionados y cálculo del total acumulado.
* **Módulo de Descuentos Flexibles:** Aplicación de descuentos por cantidad, temporada y cupones, con reglas para acumularlos.
* **Procesamiento de Pagos:** Simulación de flujos para tarjeta, transferencia y pago contra entrega.
* **Servicios Adicionales (Extras):** Selección de garantía extendida, empaque de regalo y envío express.
* **Sistema de Alertas de Stock:** Notificación automática a los clientes cuando un producto agotado vuelve a tener existencias.
* **Facturación:** Registro del historial de pedidos y generación de factura en formato texto.

### Funcionalidades Excluidas (NO se implementará)
* **Persistencia en Base de Datos Real:** Los datos se manejarán en memoria volátil (Colecciones de Java) durante la ejecución.
    * *Razón:* No es obligatorio según los términos del parcial y permite enfocar el desarrollo estrictamente en la lógica de los patrones de diseño y la arquitectura limpia.
* **Conexión con Pasarelas de Pago Externas:** Los pagos serán simulaciones lógicas por consola e interfaz gráfica.
    * *Razón:* El enunciado solicita explícitamente "medios de pago simulados", por lo que una integración real consume tiempo que no aporta a la rúbrica.
* **Seguridad y Autenticación Avanzada:** No habrá encriptación de credenciales ni manejo complejo de sesiones de usuario.
    * *Razón:* Añade una complejidad técnica innecesaria que se sale de los objetivos de evaluación del diseño orientado a objetos del proyecto.

---

## 2. Requisitos del Sistema

### Requisitos Funcionales (RF)
* **RF-01:** El sistema debe permitir visualizar productos filtrados por sus categorías específicas.
* **RF-02:** El sistema debe permitir agregar, editar la cantidad y eliminar ítems del carrito de compras.
* **RF-03:** El sistema debe evaluar y aplicar los descuentos correspondientes (acumulables o no) sobre el total del carrito.
* **RF-04:** El sistema debe procesar el pago solicitando los datos específicos según el medio elegido (tarjeta, transferencia o contra entrega).
* **RF-05:** El sistema debe permitir adjuntar servicios extras a un producto individual antes de consolidar la compra.
* **RF-06:** El sistema debe registrar usuarios en una lista de espera para un producto sin stock y disparar un aviso cuando este se reabastezca.
* **RF-07:** El sistema debe imprimir una factura desglosada con subtotales, descuentos aplicados, costos extras y total neto.

### Requisitos No Funcionales (RNF)
* **RNF-01 (Arquitectura desacoplada):** El núcleo de la lógica del negocio debe estar completamente aislado de las interfaces de usuario, permitiendo que la versión de consola y la gráfica compartan la misma base de código.
* **RNF-02 (Tecnología):** La aplicación debe ser desarrollada estrictamente en Java SE utilizando programación orientada a objetos.
* **RNF-03 (Calidad de Código):** Se deben aplicar patrones de diseño de al menos dos categorías diferentes de la clasificación GoF.
* **RNF-04 (Mantenibilidad):** El sistema debe permitir añadir nuevos tipos de pagos, descuentos o extras sin necesidad de modificar el código existente (Principio Abierto/Cerrado).
