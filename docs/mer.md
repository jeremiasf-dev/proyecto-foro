# Esquema lógico del foro

# CATEGORIA
        id PK
        nombre
        descripcion

# SUBCATEGORIA
        id PK
        nombre
        descripcion
        aporte FK -> APORTES

# USUARIO
	id PK 
	nickname 
	email
	contraseña 
	fotoPerfil 
	fechaAlta

# POST 
	id PK 
	titulo 
	contenido 
	fechaCreacion 
	activo 
	autor FK -> USUARIO
	categoria FK -> CATEGORIA

# COMENTARIO
	id PK
	contenido 
	fechaCreacion
	autor FK -> USUARIO
	post  FK -> POST

