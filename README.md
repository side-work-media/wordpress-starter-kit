[Blank Slate]: https://github.com/tidythemes/blankslate
[Docker]: https://docs.docker.com/
[Docker Compose]: https://docs.docker.com/compose/
[Docker Toolbox]: https://www.docker.com/products/docker-toolbox
[Docker Installation Guide]: https://docs.docker.com/compose/install/
[WordPress]: https://codex.wordpress.org/
[WordPress Theme Development]: https://codex.wordpress.org/Theme_Development

# Wordpress Starter Kit

A starter kit for a [WordPress], using [Docker Compose], [Docker], and the [Blank Slate] theme.

## Getting Started

### Prerequisites

If you are developing in a Windows or an OS X environment you will need to install [Docker Toolbox], which includes [Docker] and [Docker Compose].

For Linux environments you will need to install [Docker] and [Docker Compose] seperately. See the [Docker Installation Guide].

### Setup

Download the starter kit.
```
curl -L https://github.com/side-work-media/wordpress-starter-kit/archive/master.tar.gz | tar zx
cd wordpress-starter-kit-master/
```

Create and start the Docker services.
```
docker-compose create
docker-compose start
```

Open the WordPress site in your default browser.
```
open http://$(docker-machine ip default):8000/
```

## Development

Read the [WordPress Theme Development] guide and get hacking. Our theme is called SideWorkMedia and is located in `wordpress/wp-content/themes/sideworkmedia`.




