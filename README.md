# Sphinx Setup Tempalte

A few script files that auto-build and preview sphinx sites.

## Getting Started

The tempalte consists of three files. These three files are
explained below.

`start.sh` - is the main script responsible for calling other files

`listen.sh` - is the sphinx build script with a custom watchdog

`pyserver.sh` - is a Python http.server to preview site

It also includes a github workflow that will delpoy the build file.


### Prerequisites

Sphinx should be installed and your theme must be configured yourself. If
you are unsure how check out the [Sphinx Docs](https://www.sphinx-doc.org/en/master/usage/installation.html)

```
sphinx-quickstart
```

**NOTE**

Please remember to add your details in the `source/conf.py`

### Running

The `start.sh` will run both the auto-build step and the Python http.server module.
Default ip: `localhost:8000/build`

```
./start.sh
```

## Deployment

The deployment file is in the `.github/workflow` folder.

**NOTE**

Make sure that pages is set to deploy from a workflow on Githubs settings.
Deployment will fail otherwise!

## Contributing

If there is a change you think would be beneficial to have as a default
setup for 99.9% of Sphinx use-cases, add it and submit a pull request.

Always happy to have the project improved!

## Authors

  - **Neo Sahadeo**
