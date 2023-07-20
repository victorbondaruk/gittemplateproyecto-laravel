<a name="readme-top"></a>

<!-- MODIFICAR PARA CADA PROYECTO -->
<!--
gittemplateproyecto-laravel = NOMBRE DEL PROYECTO GIT
gittemplateproyecto-laravel = NOMBRE HUMANO DEL PROYECTO
proyectotemplate_url = URL DEL PROYECTO EJ https://www.destacable.com


-->
# gittemplateproyecto-laravel


<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li>
      <a href="#Developer">Developer</a>
      <ul>
        <li><a href="#Clear">Clear</a></li>
        <li><a href="#Compile and Hot-Reload for Development">Compile and Hot-Reload for Development</a></li>
        <li><a href="#Compile and Minify for Production">Compile and Minify for Production</a></li>
        <li><a href="#Data base">Data base</a></li>
        <li><a href="#Test">Test</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#tools">tools</a></li>
  </ol>
</details>

<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running follow these simple example steps.

### Prerequisites

Necessary software

* PHP > 8
  - BCMath PHP Extension
  - Ctype PHP Extension
  - JSON PHP Extension
  - Mbstring PHP Extension
  - OpenSSL PHP Extension
  - PDO PHP Extension
  - Tokenizer PHP Extension
  - XML PHP Extension

  ```sh
  php -v
  ```
* Apache > 2.0
  ```sh
  apache -v
  ```
* MySQL > 5.6
  ```sh
  mysql -v
  ```
* Composer > 2.0
  ```sh
  composer -v
  ```
* npm
  ```sh
  npm install npm@latest -g
  ```

If you have [Docker](https://www.docker.com/) you can obtain all the required programs including the following services:
- Queue: this service will manage your artisan queue
- Database: this service will create a MySQL database based on your Laravel project environment file `.env`
- PhpMyAdmin: this service will install and let you access a PhpMyAdmin console to let you manage your MySQL database
- Mailpit: this service will give you access to a local Mailpit SMTP server to test your local emails

Executing the command:
  ```sh
  composer build -d
  ```

To access your Laravel application : http://localhost:8000
To access the PhpMyAdmin console: http://localhost:8081
The MySQL Database is using the port: 3306

You can have the necessary environment with any of these alternatives

* [Laravel Homestead](https://laravel.com/docs/10.x/homestead)
* [Laravel Valet](https://laravel.com/docs/10.x/valet)
* [Laragon](https://laragon.org/download/index.html)
* [Wamp](https://www.wampserver.com/en/)
* [Xampp](https://www.apachefriends.org/es/index.html)
* [Mamp](https://www.mamp.info/en/mac/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Installation


1. Crear base de datos gittemplateproyecto-laravel
2. Clone the repo
   ```sh
   git clone https://github.com/victorbondaruk/gittemplateproyecto-laravel.git
   ```
3. Install packages

   ```sh
   cd gittemplateproyecto-laravel && composer install && npm install
   ```

4. Put the credentials to connect to the database in the `.env` file

   ```sh
    DB_CONNECTION=mysql
    DB_HOST=test
    DB_PORT=3306
    DB_DATABASE=test
    DB_USERNAME=homestead
    DB_PASSWORD=secret
   ```

5. Generate key
   ```sh
    php artisan key:generate
   ```

6. Storage directory permissions
   ```sh
    sudo chmod -R o=rwx storage
   ```

6. DB install
   ```sh
    php artisan migrate --seed
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Data base

```sh
php artisan migrate:refresh --seed
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Test

```sh
./vendor/bin/phpunit tests/Feature/TaskApiTest.php
```

```sh
php artisan make:test CategoryApiTest
```

```sh
./vendor/bin/phpunit tests/Feature/CategoryApiTest.php
```

```sh
php artisan test --parallel
```

```sh
php artisan test
```
<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Developer

### Clear
```sh
composer dump-autoload && php artisan optimize:clear && php artisan clear-compiled && php artisan config:clear && php artisan route:clear && php artisan view:clear && php artisan config:cache && php artisan route:cache && php artisan view:cache
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Compile and Minify for Production

```sh
npm run build
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



## Usage

Enjoy it your way

Please refer to the [Documentation](proyectotemplate_url)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap


- [ ] Multilingual support
  - [x] English
  - [ ] Spanish
- [ ] Sitemaps


See the [open issues](https://github.com/victorbondaruk/gittemplateproyecto-laravel/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- tools -->
## Tools

* [git-flow](https://www.atlassian.com/es/git/tutorials/comparing-workflows/gitflow-workflow)
* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
* [Malven's Grid Cheatsheet](https://grid.malven.co/)
* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)
* [Font Awesome](https://fontawesome.com)
* [React Icons](https://react-icons.github.io/react-icons/search)

<p align="right">(<a href="#readme-top">back to top</a>)</p>
