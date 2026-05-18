# INF781 - Laravel 2FA

Proyecto INF781 Seguridad de Software.

## Descripción

Aplicación web desarrollada en Laravel 13 con autenticación de dos factores (2FA) utilizando TOTP y Google Authenticator.

El sistema implementa:

* Registro e inicio de sesión con Laravel Breeze
* Generación de códigos QR
* Verificación OTP
* Middleware de protección 2FA
* PostgreSQL como base de datos

## Requisitos previos

Antes de ejecutar el proyecto se debe tener instalado:

* PHP 8.3 o superior
* Composer 2.x
* Node.js 20.x LTS
* NPM 10.x
* PostgreSQL 15+
* Git

Además, PHP debe tener habilitadas las extensiones:

* pdo_pgsql
* mbstring
* xml
* gd

También se requiere una aplicación autenticadora TOTP como:

* Google Authenticator
* Microsoft Authenticator
* Authy

## Instalación del proyecto

### Crear el proyecto Laravel

```bash
composer create-project laravel/laravel:^13.0 INF781-Laravel2FA
```

### Entrar al directorio del proyecto

```bash
cd INF781-Laravel2FA
```

### Instalar Laravel Breeze

```bash
composer require laravel/breeze --dev
php artisan breeze:install blade
npm install
npm run build
```

### Generar APP_KEY

```bash
php artisan key:generate
```

### Ejecutar migraciones

```bash
php artisan migrate
```

### Ejecutar servidor

```bash
php artisan serve
```

## FInstalar el proyecto 
composer install
npm install