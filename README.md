# openfaas-templates

Custom templates for [OpenFaaS](https://www.openfaas.com).

# Usage

## Download the OpenFaaS templates

```
    faas template pull https://github.com/rclement/openfaas-template
```

## Create a function based on an OpenFaaS template

```
    faas new --lang <template-name> <project-name>
    faas build -f ./<project-name>.yml
```

## Deploy a function

(Optional) if using an OpenFaaS cluster, first deploy to a registry:

```
    faas push -f ./<project-name>.yml
```

Assuming OpenFaas is already deployed:

```
    faas deploy -f ./<project-name>.yml
```

# License

The MIT License (MIT)

Copyright (c) 2018 Romain Clement

