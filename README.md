# Classificação de Células de Medula Óssea

A Classificação de Células de Medula Óssea usando Redes Neurais Convolucionais surge como um projeto avaliativo para a disciplina de Redes Neurais, ofertada pelo curso de Engenharia de Software da Ufersa campus Pau dos Ferros.

## Objetivo do Projeto

A Classificação de Células da Medula Óssea é uma tarefa importante que busca entender a função das células sanguíneas e é usada para auxiliar no diagnóstico de doenças como: leucemias, anemias, mielomas e dentre outras doenças hematológicas.
O processo de classificação é feito manualmente com auxílio de microscópio por um profissional especializado, como um hematologista ou patologista. O projeto em questão visa auxiliar os especialistas a realizar a classificação de maneira rápida e prática, de modo a reduzir erros humanos, acelerar o processo de diagnóstico e ainda auxiliar em regiões do mundo que careçam de mão de obra especializada.

## Descrição dos Dados

O dataset escolhido para esse projeto conta com um total de 9800 imagens em formato jpg coloridas artificialmente. As imagens são divididas em 7 classes:

* Blastos - Células imaturas.
* Eosinófilos - Respostas alérgicas.
* Linfócitos - Sistema imunológico.
* Monócitos - Combate de infecções.
* Neutrófilos Seg. - Combatem bactérias.
* Não Ident. - Sem categoria.
* Promielócitos - Precursores de granulócitos

O conjunto de treinamento conta com 1000 imagens de cada tipo de célula, enquanto dados de validação e teste possuem 200 imagens de cada.

## Pré-processamento de Dados

    
A etapa de pré-processamento de dados, assim como o restante do projeto, foi desenvolvida na linguagem Python.
O pré-processamento foi efetuado nas seguintes etapas:

* Importação e carregamento das imagens
* Redimensionamento das imagens originalmente em 250x250 pixels para 128x128
* Normalização das imagens para o intervalo 0-1

O processo completo está documentado no arquivo [cnn-model.ipynb](https://github.com/queirozPedro/Classificacao-de-Celulas-Medula-Ossea/blob/main/cnn-model.ipynb)


## Executar o Projeto

<strong>1 - Crie um Ambiente Virtual</strong>

<strong>Windows</strong>
~~~
python -m venv venv
~~~

<strong>Linux</strong>
~~~
python3 -m venv venv
~~~

<strong>2 - Ative o Ambiente Virtual</strong>

<strong>Windows</strong>
~~~
venv\Scripts\activate
~~~

<strong>Linux</strong>
~~~
source venv/bin/activate
~~~

<strong>3 - Instale as dependências</strong>

~~~
pip install -r requirements.txt
~~~

<strong>4 - Instale a extenção do [Jupyter Notebook](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) no Visual Studio Code</strong>

<strong>5 - Execute o projeto</strong>
