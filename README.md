# Lazy Campus legacy landing page

This repository retains the previous static landing page and its history.
The active homepage source is
[Gradient-Clipping/lazycampus-homepage](https://github.com/Gradient-Clipping/lazycampus-homepage).

Changes to `main`, pull requests and manual workflow runs only verify that this
legacy page builds. This repository no longer publishes container images or
deploys to `lazycampus.com`. The new homepage publishes a separate
`lazycampus/lazycampus-homepage` image consumed by the existing GitOps workload.

## Local verification

```sh
docker build -t lazycampus-site:local .
docker run --rm -p 8080:8080 lazycampus-site:local
```

Open <http://localhost:8080> to inspect the retained legacy page locally.
