# Tool di Collaudo CRM-U

Tool di verifica consistenza dati relativo alle entità: pratiche, articoli pratiche, documenti, contratti e asset sul CRM-U (Dynamics).

## Librerie Python richieste
Al primo "run" da jupyter verificare se le seguenti librerie sono disponibili, in alternativa eseguire i seguenti comandi. 

```shell
pip install json-excel-converter
pip install xlsxwriter
```

## Avvio rapido con Docker

```shell
docker pull jupyter/scipy-notebook
docker run -p 8888:8888 jupyter/scipy-notebook
```

Verrà automaticamente fatta la build del `master`.

Da browser vai al link indicato da shell:

http://<hostname>/?token=<token> 

For speed and friendliness to GitHub, be sure to set `GITHUB_OAUTH_KEY` and `GITHUB_OAUTH_SECRET`:

```shell
docker run -p 8080:8080 -e 'GITHUB_OAUTH_KEY=YOURKEY' \
                          -e 'GITHUB_OAUTH_SECRET=YOURSECRET' \
                          jupyter/nbviewer
```

Or to use your GitHub personal access token, you can just set `GITHUB_API_TOKEN`.
