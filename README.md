![Badge em Desenvolvimento](https://img.shields.io/badge/DataBriks-DataLake-blue)
![Badge em Desenvolvimento](https://img.shields.io/badge/DataBriks-Cluster_Spark-green)
![Badge em Desenvolvimento](https://img.shields.io/badge/DataBriks-Notebook-blue)
### FRANCISCO JAIME DA SILVA


## Projeto Engenharia de dados com DataBricks


<p align="center"><img src="./imagens/Marketecture.svg" width="500"></p>

__*Foi Crianda uma estrutura de data lake no Databricks community*__

O projeto consiste em criar um data lake no Databricks community, fazer upload de dados processa-lo e converte-los para um formato mais adequado a analises levando em consideração espaço de armazenamento e performance do pyspark. 

---

### Etapas do Projeto

1. Foi Criado um datalake  utilizando o Databricks community com estruta abaixo

<ul>
  <li>Bancket(landing) - Landing zone ou Zona de Pouso(dados em formato bruto)</li>
  <li>Bancket(processing) - Processing zone(dados pre-processados)</li>
  <li>Bancket(cureted) - Cureted zone(Dados limpos, agregados e prontos para análises)</li>  
</ul> 
2.Foi realizado o upload dos arquivos de dados na zona de pouso(landing), extraídos do kaggle

<ul>
  <li>T201601PDPI+BNFT.csv</li>
  <li>T201602PDPI+BNFT.csv</li>
  <li>T201603PDPI+BNFT.csv</li>
  <li>T201604PDPI+BNFT.csv</li> 
  <li>T201605PDPI+BNFT.csv</li>  
  <li>T201606PDPI+BNFT.csv</li>
  <li>T201607PDPI+BNFT.csv</li>
  <li>T201608PDPI+BNFT.csv</li>
  <li>T201609PDPI+BNFT.csv</li>
  <li>T201610PDPI+BNFT.csv</li>
  <li>T201611PDPI+BNFT.csv</li>
  <li>T201612PDPI+BNFT.csv</li>   
</ul> 

3. Foi criado um cluster spark Databricks 

4. Foram realizadas a limpeza, preprocessamento e conversão para o formato parquet, visando melhorar a performance nas proximas etapas do processo. O resultado(df-formatado.parquet) desse processo foi gravado na Proessing zone.

5. Foi realiada a leitura dos dados em formato parquet e criada a view Dados_Sql para permitir exploração dos mesmos via SQL.

6. Foi aplicada agragação nos dados da view Dados_Sql e gravado o resultado na Cureted zone em formato parquet.(df-Dados-Agregados.parquet)

7. Foi utiizado o notebook abaixo para realiza o processamento dos dados.
<https://github.com/jaimesilvads/databriks/blob/main/SparckComDatabricks.ipynb>
<https://github.com/jaimesilvads/databricks/blob/main/SparckComDatabriks.ipynb>
