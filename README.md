# Classificação de Imagens de Leões e Ursos com Transfer Learning

## 📃**Desafio-DIO**


Este projeto demonstra a criação de um classificador de imagens para identificar leões e ursos. A abordagem utiliza a técnica de **Transfer Learning** com a arquitetura VGG16, pré-treinada no conjunto de dados ImageNet.

##  Tecnologias

Esse projeto foi desenvolvido com as tecnologias:

- COLAB
- Python


## Descrição do Projeto

O objetivo é treinar um modelo de Deep Learning para diferenciar entre duas classes de animais:
- Leões
- Ursos

O processo de treinamento foi realizado no Google Colab e inclui as seguintes etapas:
1.  **Organização dos dados:** As imagens foram separadas em conjuntos de treino, validação e teste.
2.  **Pré-processamento e Aumento de Dados:** Utilizando `ImageDataGenerator` para preparar as imagens e aumentar a robustez do modelo.
3.  **Construção do Modelo:** O modelo VGG16 (sem a camada superior) foi usado como base, com novas camadas densas adicionadas para a classificação final.
4.  **Treinamento:** O modelo foi treinado por 15 épocas no conjunto de treino.
5.  **Avaliação:** A performance final foi avaliada no conjunto de teste.

## Como Executar

Este projeto foi desenvolvido em um ambiente de notebook Jupyter (`.ipynb`). Para executá-lo, siga os passos:

1.  **Abra o Notebook:** Faça o upload do notebook `Projeto_Leao_Urso.ipynb` para o Google Colab.
2.  **Dados:** Certifique-se de ter um conjunto de dados de imagens de leões e ursos nomeados de forma que o script possa identificá-los (ex: `leao_001.jpg`, `urso_pardo.png`).
3.  **Execute as Células:** Siga as instruções e execute as células do notebook sequencialmente. O script irá guiar você pelo processo de upload, organização dos dados, treinamento e avaliação do modelo.

## Resultados

O modelo alcançou uma acurácia de validação de aproximadamente 97% na última época,
demonstrando um excelente desempenho em dados novos. A acurácia de treino atingiu um pico de 100%,
enquanto a acurácia de validação permaneceu alta, o que indica um
bom aprendizado e generalização, apesar de uma pequena indicação de overfitting.


## Dependências

- `TensorFlow`
- `Keras`
- `NumPy`
- `Scikit-learn`
- `Matplotlib`
