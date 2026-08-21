# lazycampus.com

Static landing page for `lazycampus.com`.

Every change merged to `main` is built as an immutable container image and
published to Tencent Container Registry. Flux then updates the K3s deployment
from the matching `1.0.<run-number>` tag.

## Local verification

```sh
docker build -t lazycampus-site:local .
docker run --rm -p 8080:8080 lazycampus-site:local
```

Open <http://localhost:8080> and verify the page before merging.
Static site for lazycampus.com
