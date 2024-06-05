# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.



#
Controlador de consumo y propinas.
Informe:

#
React
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

TypeScript
El uso de TypeScript en este proyecto asegura que el código sea más robusto y fácil de mantener, al proporcionar verificaciones de tipo en tiempo de desarrollo. Esto es particularmente útil para la definición de tipos personalizados como MenuItems y OrderItem, garantizando que los datos manejados en los componentes sean siempre del tipo esperado.

Tailwind CSS
Framework de CSS altamente configurable que se utiliza para diseñar interfaces de usuario de manera rápida y eficiente. En este proyecto, Tailwind CSS ha sido clave para crear un diseño moderno y responsivo, con clases utilitarias que permiten aplicar estilos directamente en los componentes de React. Esto incluye la personalización de botones, formularios y la disposición general de los elementos en la interfaz.

CSS
Además de Tailwind CSS, se ha utilizado CSS para añadir transiciones y efectos adicionales a la interfaz de usuario, mejorando la experiencia del usuario. Por ejemplo, se han definido clases como .img-secondary y .order__selected para añadir efectos de transición y hover, haciendo que la interfaz sea más dinámica y atractiva visualmente.

En conjunto, estas tecnologías han permitido desarrollar una aplicación de pedidos intuitiva y eficiente, con una interfaz de usuario moderna y una lógica de gestión de pedidos clara y robusta. La integración de React con TypeScript y Tailwind CSS ha facilitado la creación de una solución completa que mejora la experiencia tanto para los usuarios finales como para los desarrolladores.
#

![image](https://github.com/JhojanBinary/Registro-De-Pagos/assets/102551448/a4254584-2519-4935-a878-d13d8a24e5dd)

![image](https://github.com/JhojanBinary/Registro-De-Pagos/assets/102551448/c7eefeeb-56b3-49c2-9ed6-f5c855af499e)
![image](https://github.com/JhojanBinary/Registro-De-Pagos/assets/102551448/5db9cb51-4132-47b9-99fc-e8d5ffaf105c)
![image](https://github.com/JhojanBinary/Registro-De-Pagos/assets/102551448/999bd831-89ac-4d23-b1b0-233839634462)

![image](https://github.com/JhojanBinary/Registro-De-Pagos/assets/102551448/3d821e5a-824d-42ca-b3de-1aa8a30960ad)


![image](https://github.com/JhojanBinary/Registro-De-Pagos/assets/102551448/0fc37cea-2050-4edc-bc9a-239ca5df33e3)

![image](https://github.com/JhojanBinary/Registro-De-Pagos/assets/102551448/e7be7d4e-9f25-4f3e-b23c-4063f088102b)

![image](https://github.com/JhojanBinary/Registro-De-Pagos/assets/102551448/1931bf7a-bcf0-4d3e-8413-2e8678ea20c2)


Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default {
  // other rules...
  parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
  },
}
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list
