# CollaudoCRMU

Tool di verifica consistenza dati relativo alle entità: pratiche, articoli pratiche, documenti, contratti e asset sul CRM-U (Dynamics).

## Librerie Python richieste
pip install json-excel-converter
pip install xlsxwriter

## Avvio rapido con Docker

```shell
docker pull jupyter/scipy-notebook
docker run -p 8888:8888 jupyter/scipy-notebook
```

It automatically gets built with each push to `master`, so you'll always be able to get the freshest copy.

For speed and friendliness to GitHub, be sure to set `GITHUB_OAUTH_KEY` and `GITHUB_OAUTH_SECRET`:

```shell
docker run -p 8080:8080 -e 'GITHUB_OAUTH_KEY=YOURKEY' \
                          -e 'GITHUB_OAUTH_SECRET=YOURSECRET' \
                          jupyter/nbviewer
```

Or to use your GitHub personal access token, you can just set `GITHUB_API_TOKEN`.
