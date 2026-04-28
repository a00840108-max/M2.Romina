# MiniScrum Distribuido

## Objetivo

Aplicación web distribuida para gestionar tareas de un proyecto Scrum, sugiriendo automáticamente puntos Scrum usando regresión lineal basada en horas estimadas.

## Arquitectura

Navegador -> Node Gateway -> PHP API -> MySQL
Navegador -> Node Gateway -> Python ML API

## Servicios

- gateway: frontend y API Gateway.
- php-api: CRUD de tareas.
- python-ml: predicción de puntos Scrum.
- mysql: base de datos relacional.

## Endpoints principales

- GET /api/tasks
- POST /api/tasks
- PUT /api/tasks/:id/status
- POST /api/predict

## Base de datos

Tabla principal: tasks.

## Cómo ejecutar localmente

docker compose up --build

## URL desplegada

[Agregar aquí la URL de Dockploy]

## Evidencias

[Agregar capturas de:
- aplicación funcionando
- tareas guardadas
- contenedores activos
- repositorio con commits]

## Retrospectiva

Qué salió bien:

Qué fue difícil:

Qué mejoraría:

## Preguntas de reflexión

1. ¿Por qué el navegador no se conecta directamente a MySQL?
2. ¿Qué ventaja tiene separar el servicio PHP del servicio Python?
3. ¿Qué función cumple el API Gateway?
4. ¿Qué pasaría si el servicio Python deja de funcionar?
5. ¿Qué diferencia hay entre ejecutar localmente con Docker Compose y desplegar en Dockploy?
6. ¿Qué parte del sistema representa la capa de datos?
7. ¿Qué parte representa la capa de presentación?
8. ¿Qué parte representa la lógica de negocio?