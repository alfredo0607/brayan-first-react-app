# 📝 Ejercicio Práctico: Creación y Validación de un Formulario en React

## 🎯 Objetivo

Desarrollar un componente funcional en React que permita gestionar los datos de un formulario utilizando el hook `useState` para controlar los campos y condicionales tradicionales (`if`) para validar la información antes de permitir su envío.

## 📋 Requisitos de la Aplicación

Crear un componente funcional llamado `FormularioBasico` que cumpla con los siguientes requerimientos:

### 1. Campos del formulario

El formulario debe contener los siguientes campos de entrada:

- **Nombre:** Campo de texto (`text`).
- **Correo Electrónico:** Campo de texto (`email`).
- **Contraseña:** Campo de contraseña (`password`).

### 2. Manejo de estado con useState

Utilizar el hook `useState` de React para:

- Almacenar el valor de cada campo del formulario.
- Mantener los inputs controlados mediante las propiedades `value` y `onChange`.
- Gestionar los mensajes de error.
- Gestionar los mensajes de confirmación o éxito.

### 3. Validaciones obligatorias

Al hacer clic en el botón de envío, se debe ejecutar una función que:

1. Prevenga el comportamiento predeterminado del formulario utilizando `event.preventDefault()`.
2. Valide los campos en el siguiente orden:

**Nombre**
- No puede estar vacío.
- Se recomienda utilizar `.trim()` para eliminar espacios en blanco al inicio y al final.
- Si está vacío, debe mostrar un mensaje de error y detener el proceso de validación.

**Correo electrónico**
- Debe contener obligatoriamente el carácter `@`.
- Debe contener un punto (`.`).
- Si no cumple estas condiciones, debe mostrar un mensaje de error.

**Contraseña**
- Debe tener una longitud mínima de 6 caracteres.
- Si tiene menos de 6 caracteres, debe mostrar un mensaje de error.

> **Importante:** Las validaciones deben implementarse utilizando condicionales tradicionales (`if`). No utilizar librerías externas de validación.

### 4. Retroalimentación visual

La aplicación debe proporcionar información al usuario sobre el resultado del proceso:

**Cuando ocurre un error:**
- Mostrar el mensaje de error correspondiente en pantalla.
- Impedir que el formulario continúe con el proceso de registro.
- No permitir que se muestre un mensaje de éxito mientras exista un error.

**Cuando todas las validaciones son exitosas:**
- Mostrar un mensaje de confirmación, por ejemplo: `¡Registro exitoso!`.
- Limpiar todos los campos del formulario.
- Restablecer los estados correspondientes para permitir un nuevo registro.

## ⚙️ Restricciones técnicas

- Utilizar componentes funcionales de React.
- Utilizar el hook `useState` para el manejo de estados.
- Utilizar eventos `onChange` para controlar los inputs.
- Utilizar el evento `onSubmit` para gestionar el envío del formulario.
- Utilizar condicionales `if` para realizar las validaciones.
- No utilizar librerías externas para manejar formularios o validaciones.
- No utilizar `alert()` para mostrar mensajes; toda la retroalimentación debe visualizarse dentro de la interfaz.

## ✅ Criterios de evaluación

| Criterio | Descripción |
|---|---|
| Estructura | El componente está correctamente construido. |
| useState | Los estados se utilizan correctamente. |
| Inputs controlados | Los campos reflejan correctamente los valores almacenados. |
| Validaciones | Se cumplen todas las reglas solicitadas. |
| Condicionales | Se utilizan correctamente los bloques `if`. |
| Eventos | Se implementan correctamente `onChange` y `onSubmit`. |
| Retroalimentación | Los mensajes de error y éxito se muestran en pantalla. |
| Limpieza | Los campos se reinician después de un registro exitoso. |

## 🚀 Entregables

El estudiante debe entregar:

1. El código fuente del componente `FormularioBasico`.
2. La aplicación funcionando en el navegador.
3. Un repositorio de GitHub con el código desarrollado.

## 💡 Recomendaciones

- Mantener el código organizado y legible.
- Utilizar nombres de variables descriptivos.
- Separar la lógica de validación de la estructura visual cuando sea conveniente.
- Probar diferentes escenarios para verificar que todas las validaciones funcionen correctamente.

**¡Éxitos con el desarrollo!**