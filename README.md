## Dockerized Emacs for running package-lint

Dockerized Emacs based on [JAremko/docker-emacs](https://github.com/JAremko/docker-emacs) for running [package-lint](https://github.com/purcell/package-lint) to lint your Emacs Lisp packages.
Perfect for setting up CI for your Emacs lisp repos.

### Lint your Emacs lisp files!

```bash
docker run -v "$(pwd)":/mnt/workspace -t docker-emacs-package-lint:latest your-emacs-lisp-file.el
```

### Building the Docker image locally

```bash
git submodule init
docker build . -t docker-emacs-package-lint:latest
```
