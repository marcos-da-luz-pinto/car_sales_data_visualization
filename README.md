# car_sales_data_visualization

## Introdução

Este projeto consiste em uma Análise Exploratória de Dados (EDA) utilizando um *dataset* de vendas de carros usados disponibilizado no Kaggle. O objetivo principal é visualizar a relação entre as características do veículo (idade, uso, motor e combustível) e o seu preço final de venda.

A análise utiliza técnicas de visualização de dados (Box Plots, Gráficos de Dispersão e Mapas de Calor) para extrair *insights* valiosos sobre os fatores que impulsionam ou depreciam o valor de um automóvel no mercado secundário.

## Bibliotecas Utilizadas

| Biblioteca | Função |
| :--- | :--- |
| **Pandas** | Manipulação de dados, limpeza, agregação e cálculo de estatísticas. |
| **Plotly Express** | Geração de gráficos interativos e complexos (dispersão, box plot, mapa de calor) de forma concisa. |

## Perguntas de Negócio e Insights

As seguintes perguntas de negócios foram respondidas com base nas visualizações geradas:

### 1. Qual fabricante (Manufacturer) retém melhor o preço em relação à quilometragem (Mileage)?

**Análise:** Gráfico de Dispersão (Preço vs. Milhas) colorido por Fabricante.

**Resposta/Insight:**
* Carros de marcas de luxo, como Porsche e BMW, retém melhor o preço em relação as milhas rodadas;
* Os carros Toyota têm uma retenção de valor moderada;
* VW e Ford dominam o mercado de baixo valor.

---

### 2. Qual o impacto isolado da Idade (Year of manufacture) e da Quilometragem (Mileage) sobre o Preço? Qual dos dois fatores tem a correlação mais forte com o preço?

**Análise:** Mapa de Calor (Correlações).

**Resposta/Insight:**
* A correlação entre a variável 'Ano de fabricação' e 'Preço' é positiva forte (+0,71)
* A correlaçao entre a variável 'Milhas' e 'Preço' é negativa forte (-0,63)
* Ou seja, se você tem um carro novo porém com altas milhas rodadas, a força de +0,71 (ano) tentará manter o preço alto, enquanto a força de -0,63 (milhas) tentará abaixar o preço

---

### 3. Como o tipo de combustível se comporta na curva de depreciação (retenção de valor por KM rodado)?

**Análise:** Gráfico de Dispersão (KM vs. Preço) colorido por Tipo de Combustível.

**Resposta/Insight:**
* Em motores menores, não há grandes divergências entre medianas e variações de preço em carros com diferentes tipos de combustível
* Motores acima de 3L são dominados por carros a gasolina e diesel
* O mercado de carros mais caros com motor potente é, em sua maioria, Gasolina.
