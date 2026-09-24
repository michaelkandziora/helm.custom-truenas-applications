# Custom TrueNAS Applications

This repository contains a TrueNAS SCALE custom application catalog backed by Helm charts. It currently provides Traefik 2 and Nginx Proxy Manager 2.

## Add the catalog

In TrueNAS, add this repository as a custom application catalog and select the `main` branch:

<https://github.com/michaelkandziora/helm.custom-truenas-applications>

After the catalog refreshes, the applications listed in `catalog.json` are available through the TrueNAS Apps interface.

## Repository layout

- `catalog.json` describes the catalog and its application trains.
- `charts/<application>/<version>/` contains each application chart, including its TrueNAS metadata and configuration forms.
- `index.yaml` is the Helm chart index.
- `library/` contains shared chart templates.

Application-specific descriptions and setup guidance are maintained with each chart under `charts/`.
