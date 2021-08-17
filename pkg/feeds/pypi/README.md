# Pypi Feed

This feed allows polling of package updates from the pypi package repository.

## Configuration options

The `packages` Field can be supplied to the pypi feed options to enable polling of package specific apis. This is less effective
with large lists of packages as it polls the RSS feed for each package individually but it is much less likely to miss package updates between polling.


```
feeds:
- type: pypi
  options:
    packages:
    - numpy
    - scipy
```