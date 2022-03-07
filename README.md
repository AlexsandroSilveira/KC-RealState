# KC Real State - Projeto de Insights

## 1.Sobre o Projeto
Este projeto é uma análise com finalidade fictícia, apenas para demonstrar algumas habilidades adquiridas estudando a linguagem Python e suas bibliotecas.

KC Real State é um nome fictício de uma empresa que compra e revende imóveis.

## 2.Tecnologias Utilizadas

![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)


## 3.Contato
  <p>silveira.a.n@gmail.com<p>
  <p>https://www.linkedin.com/in/alexsandronsilveira/<p>

## 4.Atributos

Os dados para esse projeto foram coletados na plataforma do Kaggle: https://www.kaggle.com/harlfoxem/housesalesprediction

Nesse conjunto de dados está listadas as casas a venda em King County - USA, entre os anos de 2014 e 2015, e é apresentado originalmente como a tabela a seguir.
|    Atributos    |                         Definição                            |
| :-------------: | :----------------------------------------------------------: |
|       id        |       Numeração única de identificação de cada imóvel        |
|      date       |                    Data da venda do imóvel                   |
|      price      |    Preço que o imóvel foi colocado a venda                   |
|    bedrooms     |                      Número de quartos                       |
|    bathrooms    | Número de banheiros (0.5 = banheiro sem chuveiro)            |
|   sqft_living   | Medida (em pés quadrado) do espaço interior dos apartamentos |
|    sqft_lot     |     Medida (em pés quadrado) quadrada do espaço terrestre     |
|     floors      |                 Número de andares do imóvel                  |
|   waterfront    | Variável que indica a presença ou não de vista para água (0 = não e 1 = sim) |
|      view       | Um índice de 0 a 4 que indica a qualidade da vista da propriedade. Varia de 0 a 4, onde: 0 = baixa  4 = alta |
|    condition    | Um índice de 1 a 5 que indica a condição da casa. Varia de 1 a 5, onde: 1 = baixo \|-\| 5 = alta |
|      grade      | Um índice de 1 a 13 que indica a construção e o design do edifício. Varia de 1 a 13, onde: 1-3 = baixo, 7 = médio e 11-13 = alta |
|  sqft_basement  | A metragem quadrada do espaço habitacional interior acima do nível do solo |
|    yr_built     |               Ano de construção de cada imóvel               |
|  yr_renovated   |                Ano de reforma de cada imóvel                 |
|     zipcode     |                         CEP da casa                          |
|       lat       |                           Latitude                           |
|      long       |                          Longitude                           |
| sqft_livining15 | Medida (em pés quadrado) do espaço interno de habitação para os 15 vizinhos mais próximo |
|   sqft_lot15    | Medida (em pés quadrado) dos lotes de terra dos 15 vizinhos mais próximo |
    
    
## 5.Objetivo

Analisar e manipular o dataset com a finalidade de gerar insights que facilitem a decisão de quais imóveis comprar
    
## 6.Questão de Negócio

Definir quais são os melhores imóveis e que mais gerarão lucro
    
## 7. Planejamento da Solução

### 7.1 Selecionar imóveis para compra

Filtrar os imóveis que estejam em boas condições e tenham preço de compra abaixo da mediana da região

### 7.2 Definir preço e o momento ideal para venda

Definir a mediana de cada região, filtrar pela estação do ano
    
### 7.3 Relatório e indicação dos imóveis para a compra
    
Gerar um relatório sobre as indicações de compra e planilhas com os imóveis indicados para a compra
    
## 8. Insights
### 8.1. Crescimento médio dos imóveis YoY
    
### 8.2. Imóveis com vista para a água mais caros
       
#### 8.2.1 Imóveis com vista para a água abaixo da mediana e com boa condição.
    
### 8.3. Imóveis sem vista para a água abaixo da mediana e em boas condições
    
### 8.4. Imóveis antigos e reformados são mais caros que imóveis novos
    
#### 8.4.1. Imóveis nunca reformados.
    
#### 8.4.2 Imóveis novos e antigos não reformados abaixo da mediana
    
### 8.5. Imóveis com 3 banheiros ou mais são mais caros do que imóveis com menos que 3 banheiros.
    
#### 8.5.1 Imóveis com dois banheiros em boas condições
    
### 8.6. Imóveis com 3 quartos ou mais são mais caros do que imóveis com menos que 3 quartos.
    
#### 8.6.1 Imóveis com 2 quartos e boas condições
    
### 8.7 Estações do ano que são melhores para realizar a compra e a venda dos imóveis
    
## 9. Resultados Financeiros 
    
O crescimento ano a ano dos imóveis é em média 0,70%, um crescimento muito pequeno para reter os imóveis por um tempo muito longo, então é mais viável procurar imóveis abaixo do valor mediano de mercado visando a revenda potencializando assim os lucros.Os imóveis com vista para a água são, em média, mais caros 212% que os sem vista, portanto é um mercado que precisa de uma aporte financeiro maior, mas com capacidade de gerar um lucro significativo. Com isso apontamos algumas possibilidades dentro dessa gama de imóveis existem um total de 32 imóveis com valor abaixo da mediana, em boas condições  e com uma boa qualidade de vista para água, sendo os imóveis mais indicados a serem comprados. Se todos forem comprados e revendidos pela mediana dos preços dos imóveis com vista para a água é possível gerar um lucro de US 20.350.508,00.

Os imóveis sem vista para a água são uma quantidade muito grande, no total 3.587 imóveis, mas todos estão em boas condições e com o valor abaixo da mediana dos valores de imóveis também sem vista para a água, sendo boas indicações para possíveis vistações para julgar a viabilidade de compra. Imóveis reformados são 43,5% mais caros que imóveis não reformados, pensando nisso selecionamos 3.515 imóveis que não foram reformados, mas estão em boas condições e abaixo da mediana do mercado, demandando um gasto baixo com a reforma e potencializando o valor de revenda.

Imóveis com três banheiros ou mais são em média 105% mais caros do que os imóveis com menos de 3 banheiros. Então foram selecionados 2.150 imóveis que possuem menos que três banheiros e em boas condições, o ideal seria avaliar esses imóveis para determinar a possibilidade de criar um terceiro banheiro, aumentando significamente seu valor de mercado após a reforma e consequentemente o lucro. Seguindo a mesma lógica foram avaliados imóveis referente aos quartos e se constatou que os imóveis com três quartos ou mais são em média 42,5% mais caros do que os imóveis com menos de 3 quartos, totalizaram um total de 460 imóveis que também precisariam ser avaliados sobre a possibilidade de criar um terceiro quarto.

Enfim foi estudada qual a melhor época do ano para se comprar ou vender os imóveis. E no inverno os valores estão mais baixos, portanto é uma boa época para adquirir os imóveis e para vender os imóveis é na primavera seguida pelo verão, tendo um diferença 5% a 6,5% de lucro comprando e vendendo nas estações indicadas.
    
## 10. Ações Previstas
    
* Seguir os estudos sobre a Ciência de Dados.
    
* Revisar o projeto aplicando melhorias aprendidas.
    
* Construir um Dashboard online, para tirar a necessidade de um relatório e as planilhas com a indicação de imóveis.
    
    
    
    
