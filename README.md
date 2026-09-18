# Instalación de Laravel con Herd

## 1. Descarga e instala Laravel Herd

Ve a la página oficial de [Laravel Herd para Windows](https://herd.laravel.com/) y descarga el instalador. Al ejecutarlo, Herd instalará en tu sistema PHP y Composer de forma automática e invisible. No tendrás que configurar variables de entorno, paths ni archivos `.ini`.

## 2. Instala el instalador global de Laravel

Una vez que termine de instalarse Herd, cierra cualquier terminal que tengas abierta y abre una nueva (PowerShell o CMD). Para comprobar que Herd hizo su magia, escribe:

```bash
php -v
```

Si te devuelve la versión de PHP, todo está listo. Ahora, instala la herramienta para crear proyectos Laravel corriendo este comando (este paso es el equivalente a instalar un paquete global en Node con `npm install -g`):

```bash
composer global require laravel/installer
```

## 3. Crea tu primer proyecto

Ahora ve a la carpeta donde guardas tus proyectos de programación (por ejemplo, `Documents`) y crea tu API backend:

```bash
cd Documents
laravel new mi-proyecto-backend
```

El asistente de la terminal te guiará con unas preguntas para configurar el proyecto:

1. **¿Qué starter kit deseas?** Elige `None` (ya que solo quieres el backend/API).
2. **¿Qué motor de pruebas quieres?** Elige `Pest` o `PHPUnit` (el que prefieras, Pest es el estándar moderno).
3. **¿Qué base de datos usarás?** Selecciona `SQLite`. Es una base de datos que se guarda en un archivo dentro de tu proyecto. No requiere instalar programas adicionales como MySQL, por lo que podrás empezar a programar de inmediato.

Al finalizar, entra a la carpeta con `cd mi-proyecto-backend` y abre tu editor de código (como VS Code). Para encender el servidor de desarrollo, corre:

```bash
php artisan serve
```

¡Listo! Te dará una URL (normalmente `http://127.0.0.1:8000`) idéntica a cuando levantas un servidor local en Node.js con `npm run dev`.
