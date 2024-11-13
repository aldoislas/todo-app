# Ejercicio de Prueba Técnica: Todo List con React

## Objetivo

Crear una aplicación de gestión de tareas (Todos) en React con las siguientes funcionalidades: visualización, cambio de estado, adición y eliminación de tareas.

## Instrucciones

### 1. Visualización de Tareas

Importa todosData en tu componente principal.

- Mostrar una lista de todas las tareas
- Cada tarea debe mostrar:
  - Texto de la tarea
  - Estado actual (in progress/done)
  - Botón de eliminación

### 2. Estados de las Tareas

- Cada tarea debe tener dos posibles estados:
  - "in progress"
  - "done"
- El texto de las tareas debe mostrarse:
  - En color rojo cuando está "in progress"
  - En color verde cuando está "done"
- El estado actual debe ser visible mediante una etiqueta (badge)

### 3. Interactividad

- Al hacer clic en una tarea, debe alternar su estado entre "in progress" y "done"
- Debe haber un botón para eliminar cada tarea
- Debe existir un formulario para agregar nuevas tareas