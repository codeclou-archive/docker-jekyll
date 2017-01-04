# docker-jekyll

[![](https://codeclou.github.io/doc/badges/generated/docker-image-size-46.svg)](https://hub.docker.com/r/codeclou/docker-jekyll/tags/) [![](https://codeclou.github.io/doc/badges/generated/docker-from-alpine-linux.svg)](https://alpinelinux.org/) [![](https://codeclou.github.io/doc/badges/generated/docker-run-as-non-root.svg)](https://docs.docker.com/engine/reference/builder/#/user)

Docker-Image to run [jekyll](https://jekyllrb.com/) version 3.

![](https://codeclou.github.io/doc/docker-warranty.svg?v5)

----

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

----


### License

  * Dockerfile and Image is provided under [MIT License](https://github.com/codeclou/docker-jekyll/blob/master/LICENSE.md)
