## Make your Rainloop fly on Alpine

### Overview
This image provides the "[Rainloop](https://www.rainloop.net/)"-Webmailer upon a lightweight Alpine FPM-PHP image.
It is intended to be used along with an additional webserver-container like apache or nginx.

### Features
* Slim and lightweight image based on Alpine
* Pre-configured APCu and OPcache

### Basic Usage
I'd recommend to use docker-compose for spawning containers since it's the easiest way.

1. Clone the repository of this project:
   ```
   $ git clone https://github.com/Hermsi1337/docker-rainloop.git rainloop && \
   cd rainloop
   ```

2. [OPTIONAL] Open up docker-compose.yml and change the public-port in line 16:
   ```
   $ vim docker-compose.yml
   ```

3. Start your containers using docker-compose:
   ```
   $ docker-compose up -d
   ```

4. Check if your new rainloop-container is running:
   ```
   $ curl "http://localhost:1337"
   ```

### Example docker-compose files
If you are interested in my setup for running this container check [my repository](https://github.com/Hermsi1337/docker-compose) containing all my docker-compose.yml files.