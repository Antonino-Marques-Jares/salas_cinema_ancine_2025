![Mudança de número de salas ativas no Brasil ao longo dos anos](ancine_salas_cinema.jpg)

**Fonte:**

[![Gov BR](govbr.webp)](https://dados.gov.br/dados/conjuntos-dados/salas-de-exibicao-e-complexos-registrados-na-ancine)

**Autor:**
Antonino Marques Jares

**Atualizado em:** 
03/06/2025

# salas_cinema_ancine_2025
Animações sobre quantidade de salas de cinema da ANCINE ativas por Estado ou Região entre 2014 e início de 2025

# Passo 1
Execute o código ANCINE.ipynb e certifique-se que em url está apontando para o json [Dados Abertos - Salas de Exibição e Complexos Registrados na Ancine](https://dados.ancine.gov.br/dados-abertos/salas-de-exibicao-evolucao-anual.json)

# Passo 2 
Converter UF no Nome do Estado

# Passo 3
Transformando STATUS em informação 0 ou 1 o que nos posibilita somar as salas com 1 (ABERTA) e agrupar por Estado e Ano

# Passo 4
Precisamos pivotear as colunas para criar a animação 
df_pivot = df_regiao.pivot(index='DATA', columns='REGIAO', values='TOTAL').fillna(0)
Agora estamos prontos para criar a animação

# Veja as animações em
[Área de Trampo - Salas de cinema da ANCINE ativas no Brasil entre 2014 e 2025](https://www.areadetrampo.com.br/salas-de-cinema-da-ancine-ativas-no-brasil-entre-2014-e-2025/)




