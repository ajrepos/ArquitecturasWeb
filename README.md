# Modelo Vista Controlador (MVC)

## ¿Qué es el MVC?

El **Modelo Vista Controlador (MVC)** es un patrón de diseño arquitectónico que separa una aplicación en tres componentes interconectados:

- **Modelo (Model)**: Representa los datos y la lógica de la aplicación. El modelo gestiona el acceso y las actualizaciones de los datos.
- **Vista (View)**: Es la interfaz gráfica con la que interactúa el usuario. Se encarga de mostrar los datos al usuario, formateados y estructurados de manera adecuada.
- **Controlador (Controller)**: Gestiona la interacción del usuario, envía la entrada del usuario al modelo y determina qué vista debe mostrarse. Actúa como intermediario entre el modelo y la vista.

---

## Ventajas del patrón MVC

- **Separación de responsabilidades**: Al dividir la aplicación en tres componentes distintos, cada uno con una función específica, es más fácil mantener y escalar la aplicación.
- **Reutilización de componentes**: Permite reutilizar tanto el código del modelo como el de las vistas para diferentes controladores o plataformas.
- **Facilita el mantenimiento**: Al separar la lógica de negocio (modelo) de la presentación (vista), los cambios en una parte no afectan directamente a las otras.

---

## Descripción de los componentes

1. **Modelo (Model)**: 
   - Es responsable de acceder a los datos, aplicando reglas de negocio.
   - Puede estar vinculado a una base de datos, una API o cualquier fuente de información.
   - Notifica a la vista cuando los datos cambian para que ésta se actualice.

2. **Vista (View)**: 
   - Es la interfaz de usuario. Se centra en cómo se muestran los datos del modelo.
   - Su trabajo es exclusivamente visual: presentar la información sin modificarla.
   - Puede ser una página web, una aplicación móvil o un sistema embebido.

3. **Controlador (Controller)**: 
   - Actúa como intermediario entre el modelo y la vista.
   - Procesa las entradas del usuario y actualiza el modelo en consecuencia.
   - Después, decide qué vista mostrar en función de los datos actualizados del modelo.

---

## Flujo de trabajo en MVC

1. El usuario interactúa con la **Vista** (ejemplo: hace clic en un botón).
2. La **Vista** pasa la solicitud al **Controlador**.
3. El **Controlador** procesa la solicitud y actualiza el **Modelo** si es necesario.
4. El **Modelo** envía datos actualizados a la **Vista**.
5. La **Vista** muestra los datos actualizados al usuario.

---

## Ejemplo visual

Imagina una tienda en línea:
- El **Modelo** contiene los productos, precios y descripciones.
- La **Vista** es la página web que muestra esos productos al usuario.
- El **Controlador** gestiona las acciones del usuario, como agregar un producto al carrito o finalizar una compra.

---

## Enlace a un video para más información

Si quieres profundizar más en el concepto, te dejo un enlace a un video de YouTube que explica el patrón MVC:

[🔗 Entendiendo el Patrón MVC - Video YouTube](https://www.youtube.com/watch?v=OnaWnh5cPgw)
