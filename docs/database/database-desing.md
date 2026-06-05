Tablas

Equipo
--
id PK
nombre
descripcion
coordinador_id FK -> usuario.id

usuario
--
id PK
nombre
apellido
correo
password
activo
rol
equido_id FK -> 

Evento
--
id PK
titulo
descripcion
mensaje_organizador
fecha_inicio
fecha_fin
tipo_evento
ubicacion
enlace_virtual
estado

equipo_id FK -> equipo.id
creador_id -> usuario.id

Invitacion
---
id PK
estado
obligatoriedad
fecha_respuesta
comentario_respuesta

usuario_id -> usuario.id
evento_id -> evento.id

