# Lista de tareas CRUD

Una aplicación simple de lista de tareas con funcionalidades CRUD (Crear, Leer, Actualizar, Eliminar) desarrollada en HTML, CSS y JavaScript puro.
Desarrollada por Franklin Javier Carpio, matrícula: 2023-0948.

## Características

- Crear nuevas tareas
- Marcar tareas como completadas
- Editar tareas existentes
- Eliminar tareas
- Almacenamiento local en el navegador (localStorage)
- Interfaz de usuario intuitiva y responsiva

## Estructura del proyecto

El proyecto sigue la metodología Git Flow con las siguientes ramas:

* `main`: Código estable en producción
* `develop`: Código de desarrollo integrado
* `qa`: Código listo para pruebas de calidad
* `feature/project-structure`: Estructura inicial del proyecto
* `feature/data-model`: Modelo de datos para tareas
* `feature/create-task`: Funcionalidad para crear tareas
* `feature/update-delete-tasks`: Funcionalidad para actualizar y eliminar tareas
* `feature/improve-ui`: Mejoras en la interfaz de usuario
* `hotfix/fix-todo-app`: Corrección de problemas en la funcionalidad principal

## Tecnologías utilizadas

- HTML5
- CSS3
- JavaScript (ES6+)
- localStorage para persistencia de datos

## Modelo de datos

Las tareas se almacenan en formato JSON con la siguiente estructura:

```javascript
{
  id: Number, // Identificador único (timestamp)
  text: String, // Texto de la tarea
  completed: Boolean // Estado de completado
}
```

## Solución de problemas comunes

### Problema: Los botones no funcionan al hacer clic
- **Solución**: Asegúrate de que los eventos `onclick` estén correctamente asociados a los botones. El botón principal de agregar tareas debe tener `onclick="addOrUpdateTask()"`.

### Problema: Las tareas no se muestran
- **Solución**: Verifica que el elemento `<ul id="taskList">` exista en el HTML para mostrar las tareas creadas.

## Historial de actualizaciones

### Versión 1.1.0 (Actual)
- Corregido problema con el botón de agregar tareas
- Añadido elemento faltante para la lista de tareas
- Mejorada la documentación

### Versión 1.0.0
- Lanzamiento inicial con funcionalidades CRUD básicas
- Interfaz de usuario mejorada
- Persistencia de datos con localStorage

## Cómo contribuir

1. Haz un fork del repositorio
2. Crea una rama para tu característica (`git checkout -b feature/amazing-feature`)
3. Haz commit de tus cambios (`git commit -m 'Add some amazing feature'`)
4. Sube tu rama (`git push origin feature/amazing-feature`)
5. Abre un Pull Request