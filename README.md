# Dashboard TEC1

Dashboard HTML pronto para hospedagem no GitHub Pages.

## Estrutura

```text
/
├── index.html
├── README.md
└── dados/
    ├── manifest.json
    └── tec1-26-07.json
```

## Regra oficial de data

A coluna `DATA_AGENDA` do arquivo JSON e a referencia oficial para:

- graficos diarios;
- tabelas diarias;
- tabelas mensais;
- KPIs e acumulados;
- competencia mensal.

Formatos aceitos em `DATA_AGENDA`:

- `DD/MM/AAAA`
- `DD-MM-AAAA`
- `AAAA-MM-DD`
- numero serial de data do Excel

Registros sem `DATA_AGENDA` valida nao entram nas analises.

## Publicacao no GitHub Pages

1. Envie todos os arquivos mantendo a estrutura das pastas.
2. Substitua `dados/tec1-26-07.json` pelo arquivo real de mesmo nome.
3. No GitHub, acesse **Settings > Pages**.
4. Em **Build and deployment**, selecione **Deploy from a branch**.
5. Escolha a branch principal e a pasta `/root`.

## Inclusao de novas competencias

Adicione o novo JSON na pasta `dados` e inclua uma entrada em `dados/manifest.json`.
