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

Passo a passo usando Visual Studio Code

### Windows

1 - Crie um Ambiente Virtual
```bash
python -m venv venv
```

2 - Ative o Ambiente Virtual
```bash
venv\Scrips\activate
```

3 - Instale os requeriments
```bash
pip install -r requeriments.txt
```

4 - Instale a extenção do [Jupyter Notebook](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) no Visual Studio Code

5 - Execute o projeto
