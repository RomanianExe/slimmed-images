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

34 images, generated 2026-09-13 by the pipeline's `pipeline/publish.sh`.

> **34 of 34 image(s) are staged locally but not yet pushed.** The references in the table will not resolve until they are.

| Example | Stack | Source | Size before | Size after | Change | Components | Vulns | Reference |
|---|---|---|---:|---:|---:|---|---|---|
| `nginx-golang-mysql` | Go | built | 348.12MB | 8.11MB | **-97.7%** | 62 → 6 | 582 → 41 | `ghcr.io/georgetornea/nginx-golang-mysql:slim` |
| `nginx-golang` | Go | built | 347.69MB | 8.19MB | **-97.6%** | 59 → 3 | 584 → 43 | `ghcr.io/georgetornea/nginx-golang:slim` |
| `nginx-golang-postgres` | Go | built | 348.08MB | 8.60MB | **-97.5%** | 61 → 5 | 583 → 42 | `ghcr.io/georgetornea/nginx-golang-postgres:slim` |
| `react-express-mysql` | Node/JS | built | 1205.04MB | 135.37MB | **-88.8%** | 893 → 78 | 2017 → 28 | `ghcr.io/georgetornea/react-express-mysql:slim` |
| `react-rust-postgres` | Rust | built | 85.39MB | 9.88MB | **-88.4%** | 88 → 0 | 211 → 0 | `ghcr.io/georgetornea/react-rust-postgres:slim` |
| `react-nginx` | Node/JS | built | 70.88MB | 9.39MB | **-86.7%** | 71 → 1 | 16 → 0 | `ghcr.io/georgetornea/react-nginx:slim` |
| `apache-php` | PHP | built | 480.78MB | 77.46MB | **-83.9%** | 197 → 4 | 1955 → 59 | `ghcr.io/georgetornea/apache-php:slim` |
| `nginx-wsgi-flask` | Python | built | 84.15MB | 19.17MB | **-77.2%** | 75 → 2 | 333 → 90 | `ghcr.io/georgetornea/nginx-wsgi-flask:slim` |
| `angular` | Node/JS | built | 821.25MB | 200.33MB | **-75.6%** | 1824 → 970 | 803 → 237 | `ghcr.io/georgetornea/angular:slim` |
| `postgresql-pgadmin` | Python | prebuilt | 547.43MB | 135.21MB | **-75.3%** | 210 → 6 | 65 → 21 | `ghcr.io/georgetornea/postgresql-pgadmin:slim` |
| `minecraft` | Java | prebuilt | 881.53MB | 257.74MB | **-70.8%** | 486 → 178 | 1442 → 60 | `ghcr.io/georgetornea/minecraft:slim` |
| `fastapi` | Python | built | 184.94MB | 55.17MB | **-70.2%** | 169 → 6 | 460 → 43 | `ghcr.io/georgetornea/fastapi:slim` |
| `django` | Python | built | 89.57MB | 28.03MB | **-68.7%** | 63 → 1 | 182 → 73 | `ghcr.io/georgetornea/django:slim` |
| `flask` | Python | built | 72.73MB | 23.32MB | **-67.9%** | 80 → 2 | 41 → 21 | `ghcr.io/georgetornea/flask:slim` |
| `vuejs` | Node/JS | built | 369.48MB | 120.69MB | **-67.3%** | 2183 → 590 | 554 → 194 | `ghcr.io/georgetornea/vuejs:slim` |
| `nginx-flask-mysql` | Python | built | 76.19MB | 26.73MB | **-64.9%** | 80 → 2 | 52 → 21 | `ghcr.io/georgetornea/nginx-flask-mysql:slim` |
| `nginx-flask-mongo` | Python | built | 80.38MB | 29.25MB | **-63.6%** | 82 → 2 | 41 → 21 | `ghcr.io/georgetornea/nginx-flask-mongo:slim` |
| `flask-redis` | Python | built | 77.64MB | 28.74MB | **-63.0%** | 82 → 3 | 41 → 21 | `ghcr.io/georgetornea/flask-redis:slim` |
| `elasticsearch-logstash-kibana` | Java/Node | prebuilt | 916.80MB | 374.82MB | **-59.1%** | 977 → 537 | 548 → 143 | `ghcr.io/georgetornea/elasticsearch-logstash-kibana:slim` |
| `react-express-mongodb` | Node/JS | built | 261.62MB | 109.59MB | **-58.1%** | 512 → 146 | 247 → 76 | `ghcr.io/georgetornea/react-express-mongodb:slim` |
| `wordpress-mysql` | PHP | prebuilt | 801.26MB | 360.49MB | **-55.0%** | 273 → 18 | 1115 → 4 | `ghcr.io/georgetornea/wordpress-mysql:slim` |
| `nginx-aspnet-mysql` | .NET | built | 212.76MB | 100.41MB | **-52.8%** | 103 → 4 | 329 → 1 | `ghcr.io/georgetornea/nginx-aspnet-mysql:slim` |
| `sparkjava` | Java | built | 274.24MB | 134.74MB | **-50.9%** | 170 → 20 | 519 → 47 | `ghcr.io/georgetornea/sparkjava:slim` |
| `sparkjava-mysql` | Java | built | 278.19MB | 138.68MB | **-50.1%** | 172 → 22 | 525 → 53 | `ghcr.io/georgetornea/sparkjava-mysql:slim` |
| `react-java-mysql` | Java | built | 314.52MB | 173.44MB | **-44.9%** | 249 → 98 | 627 → 155 | `ghcr.io/georgetornea/react-java-mysql:slim` |
| `spring-postgres` | Java | built | 314.95MB | 173.87MB | **-44.8%** | 257 → 106 | 635 → 163 | `ghcr.io/georgetornea/spring-postgres:slim` |
| `pihole-cloudflared-DoH` | C | prebuilt | 101.29MB | 60.47MB | **-40.3%** | 94 → 5 | 112 → 23 | `ghcr.io/georgetornea/pihole-cloudflared-doh:slim` |
| `nginx-nodejs-redis` | Node/JS | built | 125.44MB | 80.75MB | **-35.6%** | 512 → 58 | 254 → 93 | `ghcr.io/georgetornea/nginx-nodejs-redis:slim` |
| `aspnet-mssql` | .NET | built | 211.92MB | 137.00MB | **-35.4%** | 100 → 8 | 271 → 13 | `ghcr.io/georgetornea/aspnet-mssql:slim` |
| `portainer` | Go | prebuilt | 163.92MB | 106.15MB | **-35.2%** | 328 → 312 | 39 → 16 | `ghcr.io/georgetornea/portainer:slim` |
| `prometheus-grafana` | Go | prebuilt | 1405.82MB | 998.41MB | **-29.0%** | 1773 → 1650 | 221 → 164 | `ghcr.io/georgetornea/prometheus-grafana:slim` |
| `traefik-golang` | Go | built | 6.24MB | 6.24MB | **+0.02%** | 2 → 2 | 40 → 40 | `ghcr.io/georgetornea/traefik-golang:slim` |
| `nextcloud-postgres` | PHP | prebuilt | 1558.18MB | 1604.99MB | **+3.0%** | 459 → 170 | 1365 → 7 | `ghcr.io/georgetornea/nextcloud-postgres:slim` |
| `nextcloud-redis-mariadb` | PHP | prebuilt | 1558.18MB | 1604.99MB | **+3.0%** | 459 → 170 | 1365 → 7 | `ghcr.io/georgetornea/nextcloud-redis-mariadb:slim` |

## Reading the numbers

Size is a normalized, backend-independent metric: cumulative uncompressed OCI layer bytes.
Skopeo exports the local image into an OCI layout and the pipeline validates then sums the
uncompressed layer descriptors. This avoids Docker image-store-specific `inspect .Size`
semantics and `docker save` archive overhead. **The component and vulnerability columns are
not.** Slim removes package metadata along with unused files,
so Syft and Grype see less of a minimized image than of the original — part of every drop
shown here is reduced scanner visibility rather than reduced exposure. Base security
decisions on a scan of the original image. The pipeline repository's `docs/methodology.md`
§5 works through this.

One published image, `traefik-golang`, shows a *positive* change — the minimized image is
slightly larger than the original. Its final build stage is already `FROM scratch` with a
static binary, so there is nothing left to remove and Slim's own metadata adds a little. It
is published anyway, because the boundary
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
