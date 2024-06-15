# Docker - Laravel Base

Estructura base para proyectos Laravel usando Docker.

## Creación y ejecución de contenedor con docker composer

```
docker compose up -d --build nginx
```

## Composer

### Creación de imagen composer

```
docker compose build composer
```

### Iniciación de proyecto laravel

```
docker compose run --rm composer create-project laravel/laravel .
```

### Ejecución de comandos composer

```
docker compose run --rm composer require spatie/laravel-permission
```

```
docker compose run --rm composer dump-autoload
```

## NPM

### Instalación de dependencias NPM

```
docker compose run --rm npm install
```

### Ejecución de comandos NPM

```
docker compose run --rm npm run dev
```

## Artisan

### Ejecución de comandos artisan

```
docker compose run --rm artisan migrate
```

```
docker compose run --rm artisan make:model Post --migration
```

```
docker compose run --rm artisan tinker
```

## Permisos

### Ejecutar comando para permisos de directorios especiales de Laravel

```
docker compose run --rm chmod
```