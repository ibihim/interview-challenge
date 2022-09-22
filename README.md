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

1. Write a server that has health endpoints.

1. Write a client that enables you to collect data from `http://api.nasa.gov/neo/rest/v1/neo`.

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

1. (Optional) Write a command line tool for your server to enable the usage from the CLI:
    - add `neoctl get health`
    - add `neoctl get hazardous`
    - add `neoctl get hazardous --filter=(future|past|biggest)`

1. (Optional) Add a deployment yaml file for Kubernetes.

## Additional Instructions

- Tests are not optional
- After you're done, provide us the link to your repository.
- Leave comments where you were not sure how to properly proceed.
- Implementations without a README will be automatically rejected.

## Bonus Points

- Clean code!
- Knowledge of modern best practices/coding patterns.
- Knowledge of Kubernetes and containers.

