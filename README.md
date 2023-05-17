# Modelo de Árvore de Decisão para Previsão de Derrame

Este repositório contém um modelo de árvore de decisão implementado em Python usando a biblioteca PySpark. O modelo é treinado com base em dados sobre pacientes e tem como objetivo prever a probabilidade de ocorrência de derrame.

## Requisitos

- Python 3.x
- Apache Spark
- Jupyter Notebook (opcional)

## Configuração

1. Faça o download ou clone este repositório em sua máquina local.

2. Certifique-se de ter o Python 3.x instalado em seu ambiente.

3. Instale o Apache Spark seguindo as instruções fornecidas pela documentação oficial.

4. (Opcional) Caso queira executar o notebook Jupyter localmente, certifique-se de ter o Jupyter Notebook instalado.

## Conjunto de Dados

O conjunto de dados utilizado neste modelo é chamado de "stroke_data.csv". Ele contém informações sobre pacientes, incluindo idade, sexo, estado civil, tipo de trabalho, residência, histórico de tabagismo, hipertensão, doenças cardíacas, nível médio de glicose, índice de massa corporal (IMC) e se o paciente teve um derrame ou não. O arquivo CSV deve estar localizado na pasta "data" neste diretório.

## Executando o Modelo

1. Abra o Jupyter Notebook em seu ambiente local ou qualquer outra IDE Python de sua preferência.

2. Certifique-se de ter todas as bibliotecas necessárias instaladas, incluindo o Apache Spark.

3. Ajuste o caminho relativo para o arquivo "stroke_data.csv" conforme a estrutura do seu sistema de arquivos. Por padrão, espera-se que o arquivo esteja localizado em "data/stroke_data.csv".

4. Execute as células de código no notebook para treinar o modelo de árvore de decisão e fazer previsões com base nos dados de teste.

## Ajustando o Caminho do Arquivo

Caso a estrutura de diretórios ou o caminho do arquivo "stroke_data.csv" não correspondam à estrutura fornecida, siga estas etapas para ajustar o caminho:

1. Verifique a localização do arquivo "stroke_data.csv" em seu sistema de arquivos.

2. Abra o arquivo "notebook.ipynb" no editor de texto de sua preferência.

3. Localize a linha de código onde o arquivo é lido:

   ```python
   df = spark.read.csv('data/stroke_data.csv', header=True, inferSchema=True)

4. Ajuste o caminho relativo para corresponder à localização correta do arquivo "stroke_data.csv" em seu sistema de arquivos.

5. Salve o arquivo "notebook.ipynb" após fazer as alterações.

6. Execute o notebook atualizado para treinar o modelo e fazer previsões.

## Pré-processamento e Análise Exploratória
Antes de construir o modelo de previsão, realizamos uma etapa de pré-processamento dos dados, que incluiu a codificação das variáveis categóricas e a normalização das variáveis numéricas. Além disso, realizamos uma análise exploratória dos dados, buscando entender as distribuições e relações entre as variáveis e identificar possíveis insights.

## Modelo de Árvore de Decisão
Para construir o modelo de previsão, utilizamos o algoritmo de Árvore de Decisão. A Árvore de Decisão é um algoritmo de aprendizado supervisionado que utiliza uma estrutura de árvore para fazer previsões com base em regras de decisão aprendidas a partir dos dados de treinamento. O modelo foi implementado utilizando a biblioteca Apache Spark, que oferece suporte para processamento distribuído e paralelo de dados.

## Treinamento e Avaliação do Modelo
Dividimos o conjunto de dados em conjuntos de treinamento e teste e utilizamos o pipeline do Spark para encadear as etapas de pré-processamento e treinamento do modelo. O modelo foi treinado com os dados de treinamento e, em seguida, foi avaliado utilizando os dados de teste. A métrica de avaliação utilizada foi a acurácia, que mede a proporção de previsões corretas feitas pelo modelo.

## Resultados
Após treinar e avaliar o modelo, obtivemos uma acurácia de 100% nos dados de teste. Isso indica que o modelo foi capaz de prever com precisão se uma pessoa teve ou não um derrame com base nas características fornecidas. No entanto, é importante considerar que a acurácia perfeita pode ser um indício de overfitting, então é recomendável avaliar o modelo em outros conjuntos de dados para verificar sua capacidade de generalização.

## Conclusão
Este projeto demonstrou o desenvolvimento de um modelo de previsão de risco de derrame utilizando a técnica de Árvore de Decisão. O modelo foi capaz de alcançar uma alta acurácia na previsão do risco de derrame, o que pode ter implicações importantes na identificação precoce e no tratamento adequado de pacientes em risco. No entanto, é importante

## Contribuição e Feedback
Se você tiver alguma contribuição, sugestão ou feedback para melhorar este projeto, sinta-se à vontade para enviar um pull request ou abrir uma nova issue. Sua participação é sempre bem-vinda!

## Autor
Nelson Fernandes
nelsondouglaas@hotmail.com
https://www.linkedin.com/in/nelson-fernandes-4378a2170/
