# Intro_Ciencia_dados
Repositório para a disciplina de Introdução de Ciência de dados ambientais, do PPGCAm ministrada pela Dra. Silvia Jesus

Oii =) esse arquivo é uma passo a passo do que eu fiz pra disciplina de Ciência de Dados, nesse arquivo vai ter 2 partes: 1- Passo a passo sobre Classificação das aves; 2- Agrupamento dos traços das aves. É necessário utilizar o Glossário para o entendimento de termos técnicos. 

#### 1- Classificação espécies de aves e características ####

## Descrição do Projeto
Este projeto tem como objetivo classificar as características das espécies de aves com base em datasets que possuem dados de atributos morfológicos, utilizando técnicas simples no python, selecionar colunas que desejamos, filtrando os dados e calculando os quartis para encontrarmos as classificações de pequeno e grande.Esse projeto foi realizado para a disciplina de Introdução à Ciência de Dados, da professora Dra. Silvia Cristina de Jesus, do PPGCAm, e utiliza como base dados da minha pesquisa de mestrado que está sendo realizada no NEEDS-LS. 

## Dados Utilizados
Os dados incluem as seguintes variáveis morfológicas e ecológicas:
- **Mass** (g)
- **Wing.length** (mm)
- **Tail.length** (mm)
- **Tarsus.length** (mm)
- **Beak.length_culmen** (mm)
- **Beak.width** (mm)
- **Trophic.Niche**

O arquivo de dados está no formato .CSV e deve conter as colunas mencionadas.

## Estrutura do Projeto
- `dados/`: Contém o arquivo de dados ('AVONET.csv', 'Lista_Species1.csv', 'dados_filtrados_aves.csv')
- `scripts/`: Contém o script Python para análise (`classificação_aves.ipynb`)
- `resultados/`: Contém os arquivos de saída gerados durante a análise

## Requisitos
Certifique-se de ter as seguintes bibliotecas Python instaladas:
- `pandas`

##Para instalar todas as dependências, execute:
```bash
pip install -r requirements.txt

##Como Executar
Certifique-se de que o arquivo de dados está localizado na pasta dados/.
Execute o script Python:
bash
Copiar código
python scripts/classificação_aves.ipynb
Os resultados estarão disponíveis na pasta resultados/.

##Resultados Esperados
Temos uma classificação em relação aos dados morfológicos das aves, separando em pequeno e grande, por meio do calculo dos quartis




#### 2- Análise de Morfologia de Aves ####

## Descrição do Projeto
Este projeto tem como objetivo agrupar espécies de aves com base em suas características morfológicas, utilizando técnicas de aprendizado não supervisionado, como o agrupamento K-Means. Os dados analisados contêm medidas morfológicas (ex.: tamanho do bico (culmen), massa, nicho trófico) de diferentes espécies. Esse projeto foi realizado para a disciplina de Introdução à Ciência de Dados, da professora Dra. Silvia Jesus, do PPGCAm, e utiliza como base dados da minha pesquisa de mestrado realizadas no NEEDS-LS. 

## Dados Utilizados
Os dados incluem as seguintes variáveis morfológicas e ecológicas:
- **Mass** (g)
- **Wing.length** (mm)
- **Tail.length** (mm)
- **Tarsus.length** (mm)
- **Beak.length_culmen** (mm)
- **Beak.width** (mm)
- **Trophic.Niche**

O arquivo de dados está no formato .CSV e deve conter as colunas mencionadas.

## Estrutura do Projeto
- `dados/`: Contém o arquivo de dados (`dados_classificados_completos.csv`).
- `scripts/`: Contém o script Python para análise (`agrupamento_morfologia.ipynb`).
- `resultados/`: Contém os gráficos e arquivos de saída gerados durante a análise.

## Requisitos
Certifique-se de ter as seguintes bibliotecas Python instaladas:
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`

##Para instalar todas as dependências, execute:
```bash
pip install -r requirements.txt

##Como Executar
Certifique-se de que o arquivo de dados está localizado na pasta dados/.
Execute o script Python:
bash
Copiar código
python scripts/agrupamento_morfologia.ipynb
Os resultados, incluindo gráficos e agrupamentos, estarão disponíveis na pasta resultados/.

##Resultados Esperados
Temos uma classificação dos dados morfológicos das aves de massa e tamanho do bico em relação ao nicho trófico, com 3 clusters diferentes. Além disso temos como resultados os seguintes pontos:
- Gráfico da curva do cotovelo para determinar o número de clusters.
- Análise visual dos clusters formados.
- Arquivo CSV contendo os dados originais com a coluna adicional de clusters.


##Contribuição
Contribuições para melhorar o projeto são bem-vindas. Abra uma issue ou envie um pull request com suas sugestões.

Autor
Sandy dos Reis Hermann
Email: shermann@estudante.ufscar.br
11.12.2024

---
