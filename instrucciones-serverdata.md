# Prueba Técnica: Aplicación Todo List con React

## Objetivo
Desarrollar una aplicación de gestión de tareas (Todo List) utilizando React y json-server como backend simulado. La aplicación debe permitir visualizar, crear, actualizar el estado y eliminar tareas.

## Requisitos Técnicos
- Proyecto base en React.js (proporcionado)
- json-server (ya configurado)
- Gestión de estados 
- Manejo de peticiones HTTP
- CSS para estilos

## Estructura Inicial del Proyecto
El proyecto base ya incluye:
- Configuración de json-server
- Archivo db.json con la siguiente estructura de datos:
```json
{
  "todos": [
    {
      "text": "Junta de trabajo",
      "status": "in progress",
      "id": "d207"
    },
    {
      "text": "Contestar correos",
      "status": "done",
      "id": "4595"
    },
    {
      "text": "Llamar a proveedores",
      "status": "in progress",
      "id": "cc19"
    }
  ]
}
```

## Requerimientos Funcionales

### 1. Visualización de Tareas
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

### 4. Gestión de Datos
Implementar las siguientes operaciones con json-server:

#### Endpoints
- GET    /todos - Obtener todas las tareas
- POST   /todos - Crear nueva tarea
- PUT    /todos/:id - Actualizar estado de tarea
- DELETE /todos/:id - Eliminar tarea

## Requerimientos Técnicos Específicos

### 1. Estructura de Datos
Cada tarea (todo) debe tener la siguiente estructura:
```json
{
  "text": "Texto de la tarea",
  "status": "in progress" // o "done"
}
```

### 2. Manejo de Estado
- Usar useState para gestionar el estado local
- Usar useEffect para cargar los datos iniciales

### 3. Peticiones HTTP
- Implementar todas las operaciones CRUD usando fetch
- Manejar adecuadamente los errores de las peticiones

## Instrucciones para Ejecutar el Proyecto

1. Instalar dependencias:
```bash
npm install
```

2. Iniciar json-server:
```bash
npm run start:server
```

3. En otra terminal, iniciar la aplicación React:
```bash
npm run dev
```