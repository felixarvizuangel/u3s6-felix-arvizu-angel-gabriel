# Proyecto Django — Felix Arvizu Angel Gabriel

## Demo en vivo (produccion)
https://u3s6-felix-arvizu-angel-gabriel.onrender.com

## Semana 6 — Autenticacion, sesiones y seguridad
Registro/login/logout propios; cada usuario ve y edita solo
sus propios servicios (probado con usuario_a y usuario_b).

## Prueba de aislamiento
Registre usuario_a y usuario_b desde /registro/ y cree 2 servicios con cada uno.
Con sesion de usuario_b, /servicios/ solo muestra sus 2 servicios, nunca los de usuario_a.
Con usuario_b escribi a mano /servicios/<id>/editar/ con el id de un servicio de usuario_a
y respondio 404 (Not Found), gracias al filtro propietario=request.user en views.py.
