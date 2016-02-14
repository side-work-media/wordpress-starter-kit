[Blank Slate]: https://github.com/tidythemes/blankslate
[Docker]: https://docs.docker.com/
[Docker Compose]: https://docs.docker.com/compose/
[Docker Toolbox]: https://www.docker.com/products/docker-toolbox
[Docker Installation Guide]: https://docs.docker.com/compose/install/
[WordPress]: https://codex.wordpress.org/
[WordPress Theme Development]: https://codex.wordpress.org/Theme_Development
[Feature branch workflow]: https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow
[pull request]: https://github.com/side-work-media/wordpress-starter-kit/pulls
[Christopher Dierkens]: mailto:cjdierkens@gmail.com
[zip]: https://github.com/side-work-media/wordpress-starter-kit/archive/master.zip
[tar.gz]: https://github.com/side-work-media/wordpress-starter-kit/archive/master.zip

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
Use this starter kit to jump start a new WordPress website repository. Download the starter kit as a [zip] or a [tar.gz] and unpack into a new directory.

Initialize a new git repo.
```
cd UNPACKEDDIRECTORY/
git init
git add .
git commit -m 'Initial Commit'
git remote add origin https://github.com/USERNAME/OTHERREPOSITORY.git
git push -u origin master
```

From here it's up to you to manage your theme changes.

> Read the [WordPress Theme Development] guide and get hacking. Our theme is called SideWorkMedia and is located in `wordpress/wp-content/themes/sideworkmedia`.

## Contribute

1. Checkout a feature branch.

	```
	git checkout -b '#1-issue-feature-or-enhancement-name' // Issue number + meaningful name
	```
	> Please create a ticket if one doesn't exist for the changes you are making.
1. Make changes to your feature branch.
	> Read the [WordPress Theme Development] guide and get hacking. Our theme is called SideWorkMedia and is located in `wordpress/wp-content/themes/sideworkmedia`.

1. Commit.
1. Submit a [pull request].

## Contributors

[Christopher Dierkens]