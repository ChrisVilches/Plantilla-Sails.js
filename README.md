# Plantilla para Sails.js v0.12.13

## Instalacion

```
npm install
sails lift
```

Quizas hay que tener Sails.js instalado globalmente (usar `npm install -g sails`)

## Poblar base de datos

Primero agregar guitarras usando

```
POST http://localhost:1337/guitar
{ "brand": "Fender" }
```
	
Luego de agregar algunas guitarras, elegir una ID a suscribirse. Luego cuando se agreguen comentarios a esa guitarra (usando la URL `http://localhost:1337/guitar/1/messages` y un JSON `{ "text": "mensaje" }`), la pagina deberia recibir un mensaje por consola automaticamente (utiliza Socket.io).

Si se escoge una ID, solo se reciben notificaciones de esa ID.

Esta plantilla puede servir para crear REST y con Socket (opcional).
