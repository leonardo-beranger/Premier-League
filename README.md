diff --git a//dev/null b/README.md
index 0000000000000000000000000000000000000000..aad47f6d2f74ddbd2e48cc8e554f9bfa75f698f1 100644
--- a//dev/null
+++ b/README.md
@@ -0,0 +1,37 @@
+# Projeto Premier League
+
+Este repositório reúne dados históricos de partidas do Campeonato Inglês (Premier League) e notebooks utilizados para a exploração e criação de um modelo que prevê o resultado de jogos.
+
+## Estrutura do repositório
+
+- `base_de_dados/` contém os arquivos CSV com as informações das partidas.
+  - `England CSV.csv` e `England 2 CSV.csv` representam o conjunto completo de dados, cobrindo as temporadas de 1993/94 até 2024/25.
+  - `treinamento.csv` e `teste.csv` são divisões usadas para treinar e avaliar o modelo de machine learning.
+- `scripts/` inclui os notebooks Jupyter com todo o processo de limpeza, análise e modelagem dos dados.
+- `infos/` guarda informações auxiliares.
+
+## Dados disponíveis
+
+Cada linha dos arquivos representa uma partida e possui 25 variáveis. As principais colunas são:
+
+| Coluna                              | Descrição                                                         |
+|-------------------------------------|-------------------------------------------------------------------|
+| `Date`                              | Data da partida                                                   |
+| `Season`                            | Temporada do futebol (ex.: 2023/24)                               |
+| `HomeTeam` / `AwayTeam`             | Equipes mandante e visitante                                      |
+| `FT Result`                         | Resultado final (`H` = casa, `A` = visitante, `D` = empate)       |
+| `HTH Goals` / `HTA Goals`           | Gols do mandante e do visitante no intervalo                      |
+| `HT Result`                         | Resultado do primeiro tempo                                       |
+| `Referee`                           | Nome do árbitro                                                  |
+| `H Shots`, `A Shots`                | Chutes ao longo do jogo                                           |
+| `H Fouls`, `A Fouls`                | Faltas cometidas                                                  |
+| `H Yellow`, `A Yellow`, `H Red`, `A Red` | Cartões aplicados                                           |
+
+A descrição completa das colunas pode ser consultada no notebook `scripts/Desenv_Projeto.ipynb`.
+
+## Como utilizar
+
+1. Clone este repositório.
+2. Abra os notebooks em `scripts/` em seu ambiente Jupyter de preferência para reproduzir a análise e o treinamento do modelo.
+
+Fique à vontade para explorar os dados e adaptar o código conforme necessário.
