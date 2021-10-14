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

http://`hostname`/?token=`token` 

Per effettuare un resume del container:

```shell
docker ps -a

CONTAINER ID   IMAGE                    COMMAND                  CREATED          STATUS                     PORTS     NAMES
cb03ec65dc86   jupyter/scipy-notebook   "tini -g -- start-no…"   40 minutes ago   Exited (0) 7 minutes ago             beautiful_bardeen
```

```shell
docker start -a cb03ec65dc86
```


