# istex-dataviz

Application web basée sur [ezVis](https://github.com/madec-project/ezvis) exposant des chiffres clés sur les données de la plateforme ISTEX

## Installation et usage

```shell
git clone https://github.com/madec-project/ezvis.git
docker build -t inistcnrs/ezvis --build-arg http_proxy --build-arg https_proxy ezvis/Docker

git clone https://github.com/istex/istex-dataviz.git
export EZVIS_DATA_DIR=$(pwd)/istex-dataviz/data
export EZVIS_DATA_CONF=$(pwd)/istex-dataviz/data.json
cd ./istex-dataviz/
docker-compose up -d
```

Ensuite naviguer sur http://127.0.0.1:45221
