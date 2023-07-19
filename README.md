<!-- Improved compatibility of back to top link: See: https://github.com/victorbondaruk/gittemplateproyecto-laravel/pull/73 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the gittemplateproyecto-laravel. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- MODIFICAR PARA CADA PROYECTO -->
<!--
gittemplateproyecto-laravel = NOMBRE DEL PROYECTO GIT
proyectotemplate_nombre = NOMBRE HUMANO DEL PROYECTO
proyectotemplate_url = URL DEL PROYECTO EJ https://www.destacable.com


-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/victorbondaruk/gittemplateproyecto-laravel">
    <img src="doc/images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">gittemplateproyecto-laravel</h3>

  <p align="center">
    <br />
    <a href="https://github.com/victorbondaruk/gittemplateproyecto-laravel"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/victorbondaruk/gittemplateproyecto-laravel">View Demo</a>
    ·
    <a href="https://github.com/victorbondaruk/gittemplateproyecto-laravel/issues">Report Bug</a>
    ·
    <a href="https://github.com/victorbondaruk/gittemplateproyecto-laravel/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About The Project</a></li>
    <li><a href="#Getting Started">Getting Started</a></li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
        <li><a href="#Data base">Data base</a></li>
        <li><a href="#Test">Test</a></li>
      </ul>
    </li>
    <li>
      <a href="#Developer">Developer</a>
      <ul>
        <li><a href="#Clear">Clear</a></li>
        <li><a href="#Compile and Hot-Reload for Development">Compile and Hot-Reload for Development</a></li>
        <li><a href="#Compile and Minify for Production">Compile and Minify for Production</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![proyectotemplate_nombre][product-screenshot]](proyectotemplate_url)

<!-- Descripcion del proyecto -->



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


### Installation


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



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Project Link: [https://github.com/victorbondaruk/repo_name](https://github.com/victorbondaruk/repo_name)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
* [Malven's Grid Cheatsheet](https://grid.malven.co/)
* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)
* [Font Awesome](https://fontawesome.com)
* [React Icons](https://react-icons.github.io/react-icons/search)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/victorbondaruk/gittemplateproyecto-laravel.svg?style=for-the-badge
[contributors-url]: https://github.com/victorbondaruk/gittemplateproyecto-laravel/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/victorbondaruk/gittemplateproyecto-laravel.svg?style=for-the-badge
[forks-url]: https://github.com/victorbondaruk/gittemplateproyecto-laravel/network/members
[stars-shield]: https://img.shields.io/github/stars/victorbondaruk/gittemplateproyecto-laravel.svg?style=for-the-badge
[stars-url]: https://github.com/victorbondaruk/gittemplateproyecto-laravel/stargazers
[issues-shield]: https://img.shields.io/github/issues/victorbondaruk/gittemplateproyecto-laravel.svg?style=for-the-badge
[issues-url]: https://github.com/victorbondaruk/gittemplateproyecto-laravel/issues
[license-shield]: https://img.shields.io/github/license/victorbondaruk/gittemplateproyecto-laravel.svg?style=for-the-badge
[license-url]: https://github.com/victorbondaruk/gittemplateproyecto-laravel/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/victorbondaruk
[product-screenshot]: doc/images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
