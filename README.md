# Modelo Vista Controlador (MVC)

## Introducción

El **Modelo Vista Controlador (MVC)** es un patrón de diseño de software ampliamente utilizado en el desarrollo de aplicaciones. Divide una aplicación en tres componentes principales:

- **Modelo (Model)**: Gestiona los datos y la lógica de la aplicación.
- **Vista (View)**: Presenta los datos al usuario, generalmente a través de una interfaz gráfica.
- **Controlador (Controller)**: Actúa como un intermediario entre el modelo y la vista, procesando la lógica de negocio y las solicitudes del usuario.

Este patrón facilita la separación de preocupaciones, lo que hace que el código sea más modular, mantenible y escalable.

---

## Componentes del MVC

### 1. **Modelo (Model)**
El modelo es la capa encargada de la gestión de datos. Es responsable de manejar la lógica de la aplicación relacionada con los datos, como consultar bases de datos, aplicar reglas de negocio y responder a las peticiones del controlador.

```plaintext
class Producto:
    def __init__(self, nombre, precio):
        self.nombre = nombre
        self.precio = precio

    def obtener_precio_con_descuento(self, porcentaje_descuento):
        return self.precio - (self.precio * porcentaje_descuento / 100)
