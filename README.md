# Poetry Truststore Plugin

Truststore plugin for [poetry](https://python-poetry.org).

The plugin is needed to use system ssl/tls certificates to download and install packages from repositories with self-signed certificates. The plugin is also useful if a self-signed certificate from an internal center is added to the certificate chain

## Installation

### With _poetry_

```shell
poetry self add poetry-truststore
```

### With _pip_

```shell
$POETRY_HOME/pip inistall poetry-truststore
```

You may need the `--use-feature=truststore` parameter if you cannot download packages due to SSL errors.

```shell
$POETRY_HOME/pip inistall poetry-truststore --use-feature=truststore
```

Reed more about plugins at [poetry docs](https://python-poetry.org/docs/plugins/#using-plugins)

## Usage

After installation, you can use**poetry** as usual. ✨ The plugin indicates that it is enabled with the message _"Enabling Truststore"_ when you use the `poetry add` command