# Examen semana 8

Requirements

- [ ] Crear un nuevo repositorio llamado `examen-8`
- [ ] Ajuntar fotos de los ejercicios en el README.md
- [ ] Usar una base de datos Postgres, MySQL o MongoDB
- [ ] Codigo **ORDENADO** y **LIMPIO** usando buenas practicas

Rules

1. Se puede trabajar en parejas o individualmente
2. El examen se debe entregar el día **viernes 14 de octubre** antes de las 12:30 pm

## Ejercicio 1

Crear un API sobre una lista de musica donde se pueda hacer lo siguiente.

- Crear canciones con los siguientes campos `/api/v1/songs => POST`

```json
{
  "id": 1,
  "name": "Cancion 1",
  "artist": "Artista 1",
  "album": "Album 1",
  "year": 2020,
  "genre": "Rock",
  "duration": 120
}
```

- Leer todas las canciones `/api/v1/songs => GET`

- Leer una cancion por id `/api/v1/songs/:id => GET`
  
## Ejercicio 2

A nuestra API de canciones vamos agregar un registro y login de usuarios.

- Crear un usuario con los siguientes campos `/api/v1/users => POST`

```json
{
  "id": 1,
  "name": "Usuario 1",
  "email": "email@gmail.com",
  "password": "123456"
}
```

- Login de usuario `/api/v1/users/login => POST`

```json
{
  "email": "email@gmail.com",
  "password": "123456"
}
```

## Ejercicio 3

Vamos a relacionar nuestros usuarios con las canciones que crean, es decir vamos a crear un play list de canciones.

- Crear una playlist con los siguientes campos

```json
{
  "id": 1,
  "name": "Playlist 1",
  "userId": 1,
  "songs": [
    {
      "id": 1,
      "name": "Cancion 1",
      "artist": "Artista 1",
      "album": "Album 1",
      "year": 2020,
      "genre": "Rock",
      "duration": 120
    },
    {
      "id": 2,
      "name": "Cancion 2",
      "artist": "Artista 2",
      "album": "Album 2",
      "year": 2020,
      "genre": "Rock",
      "duration": 120
    }
  ]
}
```
