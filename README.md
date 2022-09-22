# Basic Server / Client Challenge

Dear candidate, please follow this readme and solve as many questions as you can.

## Language

Please use only the standard library.

Preferred:
- Go

Valid:
- Python
- JavaScript
- C
- Java

## Tasks

1. Write a client that the server will use to query `http://api.nasa.gov/neo/rest/v1/neo`.

1. Write a server that has health endpoints, with the path:
    - `/probes/healthz`, signals that your server is running
    - `/probes/readyz`, signals that your server is ready to serve traffic
    - respond with http status code 200 OK on success
    - respond with http status code 503 Service unabailable if not successful

1. Add an endpoint with the path `/neo/hazardous`:
    - display all DB entries which contain potentially hazardous asteroids
    - format JSON

1. Extend the endpoint with the path `/neo/hazardous/next`:
    - display the datewise next hazardous near earth object
    - format JSON

1. Extend the `/neo/hazardous` endpoint with query parameter:
    - `filter`:
        - enable sorting by `future`, which shows the near earth objects that will come and sort them by closest to today
        - enable sorting by `past`, which shows the near earth objects that already are in the past and sort them by closest to today
    - `sort`:
        - enable sorting by `size`, which sows the near earth objects first that are the biggest

1. Add a container file (`Dockerfile`).

1. Add TLS to your server.

1. (Optional) Add a deployment yaml file for Kubernetes.

1. (Optional) Create a Central Authority (CA) that signs your serving certificates.

1. (Optional) Write a command line tool for your server to enable the usage from the CLI:
    - add `neoctl get health`
    - add `neoctl get hazardous`
    - add `neoctl get hazardous --filter=(future|past|biggest)`

## Additional Instructions

- Tests are not optional
- After you're done, provide us the link to your repository.
- Leave comments where you were not sure how to properly proceed.
- Implementations without a README will be automatically rejected.

## Bonus Points

- Clean code!
- Knowledge of modern best practices/coding patterns.
- Knowledge of Kubernetes and containers.

