# docker-jekyll

## :bangbang: Deprecated and Discontinued :bangbang:

[![](https://codeclou.github.io/doc/badges/generated/docker-image-size-46.svg)](https://hub.docker.com/r/codeclou/docker-jekyll/tags/) [![](https://codeclou.github.io/doc/badges/generated/docker-from-alpine-3.5.svg)](https://alpinelinux.org/) [![](https://codeclou.github.io/doc/badges/generated/docker-run-as-non-root.svg)](https://docs.docker.com/engine/reference/builder/#/user)

Docker-Image to run [jekyll](https://jekyllrb.com/) version 3.

-----

&nbsp;

### Prerequisites

 * Runs as non-root with fixed UID 10777 and GID 10777. See [howto prepare volume permissions](https://github.com/codeclou/doc/blob/master/docker/README.md).
 * See [howto use SystemD for named Docker-Containers and system startup](https://github.com/codeclou/doc/blob/master/docker/README.md).

-----

&nbsp;

### Usage

Put an alias in your `~/.bash_profile` or `~/.bashrc`.

```
alias jekyll='docker run --rm -it -p 4000:4000 -v $(pwd):/rubyapp/ codeclou/docker-jekyll:latest'
```

Then use just as normal jekyll

```
cd mysite
jekyll serve --host 0.0.0.0
```

Now open http://localhost:4000

-----
&nbsp;

### License, Liability & Support

 * [![](https://codeclou.github.io/doc/docker-warranty-notice.svg?v1)](https://github.com/codeclou/docker-jekyll/blob/master/LICENSE.md)
 * Dockerfile and Image is provided under [MIT License](https://github.com/codeclou/docker-jekyll/blob/master/LICENSE.md)
