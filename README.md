# estudo-dengue-1

Análise exploratória e modelagem sobre as bases de notificação de dengue do **SINAN/DATASUS**, ano a ano (2016–2022). Trabalho de Iniciação Científica com financiamento **CNPq**.

## O que tem aqui

Um notebook por ano-base, seguindo o mesmo roteiro: carga, limpeza, perfil demográfico dos casos, recortes temporais e experimentos de classificação com scikit-learn.

| notebook | conteúdo |
|---|---|
| `dengbr16/` … `dengbr19/` | exploração e modelos por ano |
| `dengbr21/base-dengue-21.ipynb` | estudo mais aprofundado da base de 2021 |
| `dengbr21/learn-aux-21.ipynb` | experimentos auxiliares de modelagem |
| `dengbr22/estudo-datas copy.ipynb` | análise da sazonalidade das notificações |
| `dengbr22/learn-dengue-22.ipynb` | exploração e modelos de 2022 |

Os resultados e gráficos estão preservados nas saídas dos notebooks — dá para ler a análise inteira sem executar nada.

## Os dados não estão neste repositório

Os microdados do SINAN são registros individuais de notificação de saúde. Mesmo pseudonimizados — sem nome, sem CPF, sem endereço — carregam data de nascimento, sexo, raça, ocupação, município de residência, sintomas e evolução do caso. Por isso não são versionados aqui.

Para reproduzir, baixe as bases DENGBR do DATASUS e coloque na pasta do ano correspondente:

- <https://datasus.saude.gov.br/transferencia-de-arquivos/> → SINAN → Dengue
- a malha municipal auxiliar (`IBGE_MUNICIPIOS.xlsx`) vem do IBGE

## Licença

[MIT](LICENSE) — aplica-se ao código. Os dados do SINAN são do Ministério da Saúde e seguem os termos do DATASUS.
