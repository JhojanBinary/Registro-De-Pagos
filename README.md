# Registro-De-Pagos
Registro de pagos con TypeScript, React y Tailwind CSS: 
[https://soft-gumption-9c61d2.netlify.app/]

![image](https://github.com/JhojanBinary/Registro-De-Pagos/assets/102551448/af0ef789-9e1f-4c1c-84af-861904833361)


![image](https://github.com/JhojanBinary/Registro-De-Pagos/assets/102551448/5e1f1fef-7f66-4d78-9da3-9bcea8cc84b7)
![image](https://github.com/JhojanBinary/Registro-De-Pagos/assets/102551448/4e23dafa-9ee3-4851-b706-6fffc8db8e9b)
![image](https://github.com/JhojanBinary/Registro-De-Pagos/assets/102551448/5029362a-e196-480c-a4dc-fa86868c1cb1)
![image](https://github.com/JhojanBinary/Registro-De-Pagos/assets/102551448/ab8bf758-230f-48c4-9791-10f1d4aca262)
![image](https://github.com/JhojanBinary/Registro-De-Pagos/assets/102551448/990c56e3-9d29-4f95-97a9-21958d7b6641)


En este proyecto se ha desarrollado una aplicación web interactiva y eficiente para la gestión de pedidos en un entorno de restaurante. A continuación, se detallan las tecnologías utilizadas:

-React
En este proyecto, React se ha empleado para desarrollar componentes reutilizables que facilitan la gestión del estado y la interacción con los elementos de la interfaz de usuario. Los componentes como MenuItem, OrderContents, y OrdersTotals permiten manejar de manera eficiente la adición, visualización y eliminación de elementos en un pedido.

#
React: Gestión de Propinas
Componente TipPorcentageForm
El componente TipPorcentageForm permite a los usuarios seleccionar el porcentaje de propina que desean añadir al total de su pedido. Este formulario presenta opciones de propina predeterminadas (0%, 10%, 20%, 50%) que los usuarios pueden seleccionar. Cuando el usuario selecciona una opción, se actualiza el estado de la propina en la aplicación.

Cálculo de Propinas y Totales
En la aplicación, los cálculos de los totales y la propina se manejan utilizando React y el hook useMemo. Este hook se utiliza para memorizar el subtotal, el monto de la propina y el total general, de modo que estos valores solo se recalculen cuando el pedido o el porcentaje de propina cambien. Esto optimiza el rendimiento de la aplicación al evitar cálculos innecesarios.

Subtotal: Se calcula sumando el precio total de cada elemento del pedido (precio unitario multiplicado por la cantidad).
Monto de la Propina: Se calcula aplicando el porcentaje de propina seleccionado al subtotal.
Total General: Es la suma del subtotal y el monto de la propina.
Interfaz de Usuario
La interfaz de usuario se actualiza dinámicamente para reflejar los cambios en el pedido y la propina:

Formulario de Selección de Propina: Los usuarios pueden elegir la propina mediante un formulario interactivo que muestra las opciones disponibles. Al seleccionar una opción, la propina se actualiza inmediatamente en el estado de la aplicación.

Visualización de Totales: La sección de totales muestra el subtotal, el monto de la propina y el total general. Estos valores se recalculan y se muestran en tiempo real conforme los usuarios añaden o eliminan elementos del pedido y ajustan el porcentaje de propina.

Botón de Confirmación de Pedido: El botón para confirmar el pedido se activa solo si hay elementos en el pedido. Cuando el usuario hace clic en este botón, se guarda el pedido y se reinician los valores del pedido y la propina.


#

-TypeScript
El uso de TypeScript en este proyecto asegura que el código sea más robusto y fácil de mantener, al proporcionar verificaciones de tipo en tiempo de desarrollo. Esto es particularmente útil para la definición de tipos personalizados como MenuItems y OrderItem, garantizando que los datos manejados en los componentes sean siempre del tipo esperado.

-Tailwind CSS
En este proyecto, Tailwind CSS ha sido clave para crear un diseño moderno y responsivo, con clases utilitarias que permiten aplicar estilos directamente en los componentes de React. Esto incluye la personalización de botones, formularios y la disposición general de los elementos en la interfaz.

CSS
Además de Tailwind CSS, se ha utilizado CSS para añadir transiciones y efectos adicionales a la interfaz de usuario, mejorando la experiencia del usuario. Por ejemplo, se han definido clases como .img-secondary y .order__selected para añadir efectos de transición y hover, haciendo que la interfaz sea más dinámica y atractiva visualmente.

En conjunto, estas tecnologías han permitido desarrollar una aplicación de pedidos intuitiva y eficiente, con una interfaz de usuario moderna y una lógica de gestión de pedidos clara y robusta. La integración de React con TypeScript y Tailwind CSS ha facilitado la creación de una solución completa que mejora la experiencia tanto para los usuarios finales como para los desarrolladores.
