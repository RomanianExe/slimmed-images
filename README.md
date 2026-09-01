# Slimmed Images

Minimized container images produced by the
[docker-image-minimization-pipeline](https://github.com/RomanianExe/docker-image-minimization-pipeline)
from [awesome-compose](https://github.com/docker/awesome-compose) examples, using
[Slim Toolkit](https://github.com/mintoolkit/mint).

Each image here passed the **same functional test suite as the image it was derived from**,
before and after minimization. An image that lost functionality is not published; it is
recorded as a failure in the pipeline repository instead.

`manifests/<example>.json` carries what is needed to reproduce each one: the upstream
reference and digest, the measurements, the configuration and test script that produced
it, and the tool versions used.

## Images

29 images, generated 2026-09-01 by the pipeline's `pipeline/publish.sh`.

| Example | Stack | Source | Size before | Size after | Change | Components | Vulns | Reference |
|---|---|---|---:|---:|---:|---|---|---|
| `nginx-golang-mysql` | Go | built | 123.39MB | 4.70MB | **-96.2%** | 62 → 6 | 582 → 41 | `ghcr.io/romanianexe/nginx-golang-mysql:slim` |
| `nginx-golang` | Go | built | 123.40MB | 4.80MB | **-96.1%** | 59 → 3 | 574 → 43 | `ghcr.io/romanianexe/nginx-golang:slim` |
| `nginx-golang-postgres` | Go | built | 123.48MB | 4.91MB | **-96.0%** | 61 → 5 | 583 → 42 | `ghcr.io/romanianexe/nginx-golang-postgres:slim` |
| `react-rust-postgres` | Rust | built | 30.72MB | 4.01MB | **-86.9%** | 88 → 0 | 177 → 0 | `ghcr.io/romanianexe/react-rust-postgres:slim` |
| `react-express-mysql` | Node/JS | built | 417.88MB | 55.61MB | **-86.7%** | 661 → 76 | 1791 → 24 | `ghcr.io/romanianexe/react-express-mysql:slim` |
| `react-nginx` | Node/JS | built | 26.45MB | 4.48MB | **-83.1%** | 71 → 1 | 10 → 0 | `ghcr.io/romanianexe/react-nginx:slim` |
| `apache-php` | PHP | built | 167.77MB | 33.72MB | **-79.9%** | 197 → 4 | 1929 → 59 | `ghcr.io/romanianexe/apache-php:slim` |
| `nginx-wsgi-flask` | Python | built | 31.84MB | 8.20MB | **-74.3%** | 75 → 1 | 326 → 89 | `ghcr.io/romanianexe/nginx-wsgi-flask:slim` |
| `angular` | Node/JS | built | 242.81MB | 66.61MB | **-72.6%** | 1824 → 970 | 782 → 225 | `ghcr.io/romanianexe/angular:slim` |
| `fastapi` | Python | built | 62.34MB | 21.45MB | **-65.6%** | 169 → 6 | 414 → 42 | `ghcr.io/romanianexe/fastapi:slim` |
| `django` | Python | built | 27.72MB | 11.36MB | **-59.0%** | 63 → 1 | 178 → 71 | `ghcr.io/romanianexe/django:slim` |
| `flask` | Python | built | 23.80MB | 9.79MB | **-58.9%** | 80 → 2 | 51 → 20 | `ghcr.io/romanianexe/flask:slim` |
| `vuejs` | Node/JS | built | 107.65MB | 44.78MB | **-58.4%** | 2183 → 590 | 530 → 190 | `ghcr.io/romanianexe/vuejs:slim` |
| `nginx-flask-mysql` | Python | built | 24.36MB | 11.05MB | **-54.6%** | 80 → 2 | 62 → 20 | `ghcr.io/romanianexe/nginx-flask-mysql:slim` |
| `nginx-flask-mongo` | Python | built | 25.80MB | 11.76MB | **-54.4%** | 82 → 2 | 51 → 20 | `ghcr.io/romanianexe/nginx-flask-mongo:slim` |
| `flask-redis` | Python | built | 25.05MB | 11.58MB | **-53.8%** | 82 → 3 | 51 → 20 | `ghcr.io/romanianexe/flask-redis:slim` |
| `react-express-mongodb` | Node/JS | built | 89.93MB | 45.67MB | **-49.2%** | 512 → 146 | 244 → 74 | `ghcr.io/romanianexe/react-express-mongodb:slim` |
| `wordpress-mysql` | PHP | prebuilt | 274.73MB | 140.20MB | **-49.0%** | 273 → 18 | 1045 → 4 | `ghcr.io/romanianexe/wordpress-mysql:slim` |
| `sparkjava` | Java | built | 97.44MB | 53.96MB | **-44.6%** | 170 → 20 | 462 → 44 | `ghcr.io/romanianexe/sparkjava:slim` |
| `nginx-aspnet-mysql` | .NET | built | 86.71MB | 49.00MB | **-43.5%** | 103 → 4 | 325 → 1 | `ghcr.io/romanianexe/nginx-aspnet-mysql:slim` |
| `sparkjava-mysql` | Java | built | 101.16MB | 57.77MB | **-42.9%** | 172 → 22 | 468 → 50 | `ghcr.io/romanianexe/sparkjava-mysql:slim` |
| `react-java-mysql` | Java | built | 133.42MB | 91.15MB | **-31.7%** | 249 → 98 | 567 → 152 | `ghcr.io/romanianexe/react-java-mysql:slim` |
| `spring-postgres` | Java | built | 133.71MB | 91.43MB | **-31.6%** | 257 → 106 | 575 → 160 | `ghcr.io/romanianexe/spring-postgres:slim` |
| `nextcloud-redis-mariadb` | PHP | prebuilt | 555.55MB | 407.68MB | **-26.6%** | 459 → 170 | 1261 → 7 | `ghcr.io/romanianexe/nextcloud-redis-mariadb:slim` |
| `aspnet-mssql` | .NET | built | 85.39MB | 66.14MB | **-22.5%** | 100 → 8 | 271 → 13 | `ghcr.io/romanianexe/aspnet-mssql:slim` |
| `portainer` | Go | prebuilt | 48.55MB | 38.74MB | **-20.2%** | 328 → 312 | 34 → 11 | `ghcr.io/romanianexe/portainer:slim` |
| `nginx-nodejs-redis` | Node/JS | built | 42.81MB | 35.23MB | **-17.7%** | 512 → 58 | 246 → 91 | `ghcr.io/romanianexe/nginx-nodejs-redis:slim` |
| `prometheus-grafana` | Go | prebuilt | 474.10MB | 413.28MB | **-12.8%** | 1791 → 1760 | 178 → 157 | `ghcr.io/romanianexe/prometheus-grafana:slim` |
| `traefik-golang` | Go | built | 3.56MB | 3.77MB | **+6.1%** | 2 → 2 | 40 → 40 | `ghcr.io/romanianexe/traefik-golang:slim` |

## Reading the numbers

Size is the honest measurement: it is the image on disk, before and after. **The component
and vulnerability columns are not.** Slim removes package metadata along with unused files,
so Syft and Grype see less of a minimized image than of the original — part of every drop
shown here is reduced scanner visibility rather than reduced exposure. Base security
decisions on a scan of the original image. The pipeline repository's `docs/methodology.md`
§5 works through this.

Three examples show a *positive* change — the minimized image is slightly larger than the
original. Their final build stage is already `FROM scratch` with a static binary, so there is
nothing left to remove and Slim's own metadata adds a little. They are published anyway, because the boundary
where a technique stops paying is a result too.

## Pulling

```bash
docker pull <reference from the table>
```

## Reproducing

```bash
git clone https://github.com/RomanianExe/docker-image-minimization-pipeline
cd docker-image-minimization-pipeline
pipeline/run-pipeline.sh <example>
```

The pipeline builds the original, runs the tests, minimizes, re-runs the tests, and writes
every artifact under `artifacts/<example>/`.
