# PHP 8 FPM Docker Image with Extensive Extensions

This Docker image, based on PHP 8 FPM, provides a feature-rich environment tailored for PHP applications, supporting various frameworks like Laravel, Symfony, and more.

## 🚀 Features

- **PHP 8 FPM**: Enjoy the benefits and features of PHP 8 and FPM for your applications.
- **Rich Set of Extensions**: Out-of-the-box support for `gd`, `pdo_mysql`, `mysqli`, `zip`, `exif`, `intl`, `gmp`, and more.
- **Developer Tools**: Integrated tools like `xdebug` and `opcache` for debugging and optimizing bytecode caching.
- **Image Processing**: Leverage `imagemagick` and `imagick` for image creation, modification, and analysis.
- **Composer**: Manage dependencies seamlessly with Composer.
- **Additional Utilities**: Bundled with utilities like `git`, `curl`, `unzip`, and `vim` for a developer-friendly experience.

## 🏗️ Build the Image Locally

```sh
docker build -t your-image-name:tag .
```

## 🐳 Using the Image

### Pull from Docker Hub

```sh
docker pull agonzalezrom/lemp:latest
```

### Or, Use in Docker Compose

```yaml
version: '3.8'

services:
  app:
    image: agonzalezrom/lemp:latest
    ports:
      - "9000:9000"
```

### Volume Configuration

Ensure your project codebase is mounted as a volume to `/var/www/html` within the container.

## 👥 User Management

This image uses a non-root user `www` to run applications, enhancing container security.

## 🙏 Acknowledgments & Contributions

Your contributions, issues, and feature requests are welcome!

Feel free to check [issues page](../../issues). You can also take a look at the [contributing guide](CONTRIBUTING.md).
