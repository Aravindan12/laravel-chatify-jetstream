<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About jetstream-chatify

This application made of the laravel jetstream package which provides the authentication.Here we enabled the two factor authentication feature provide by jetstream and added a chat services using chatify package.To attain this the following steps are needed such as:

- Install jetstream package using "composer require laravel/jetstream" cmd.
- Install Livewire package using "php artisan jetstream:install livewire" cmd.
- Run npm install && npm run prod && php artisan migrate cmds.
- After that register and login an account, In the profile page you can enable the 2-factor-authentication option.
- Using Google authenticator app you will get the code.
- When you each time login you have to enter the code from the app.
- Create an account in pusher add the credentials to env like
    PUSHER_APP_ID=
    PUSHER_APP_KEY=
    PUSHER_APP_SECRET=
    PUSHER_APP_CLUSTER=
    from pusher.
- Install chatify package using "composer require munafio/chatify" cmd.
- Run "php artisan chatify:install"
- Migrate and serve. /chatify will provide you the chat module.
