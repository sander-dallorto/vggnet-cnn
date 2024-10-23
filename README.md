# Classificação de Lixo Orgânico e Reciclável com CNN

Este repositório contém o código e a documentação de um projeto desenvolvido durante minha pós-graduação em Ciência de Dados e Machine Learning no UniCEUB. O objetivo deste projeto foi construir um modelo de Rede Neural Convolucional (CNN) para a classificação automática de resíduos em duas categorias: **orgânicos** e **recicláveis**. Utilizamos o popular dataset do Kaggle para treinar e testar o modelo.

## Descrição do Projeto

A identificação e separação adequada de resíduos é uma etapa essencial no processo de reciclagem. Este projeto visa automatizar essa tarefa utilizando técnicas de aprendizado de máquina, em especial uma CNN. O modelo escolhido para esta tarefa foi uma adaptação da arquitetura **VGGNet**, conhecida por sua profundidade e eficiência em tarefas de reconhecimento de imagem.

### Modelo Utilizado: VGGNet

O VGGNet é uma rede neural convolucional profunda, com várias camadas empilhadas, que se destaca em tarefas de classificação de imagens. Utilizei esta arquitetura devido à sua capacidade de capturar padrões espaciais complexos nas imagens de lixo, melhorando a precisão na distinção entre materiais recicláveis e orgânicos.

- **VGGNet**: A versão utilizada contém várias camadas convolucionais seguidas por camadas totalmente conectadas que ajudam a rede a aprender características mais abstratas dos dados.
- **Otimizador**: Adam
- **Função de perda**: Categorical Crossentropy
- **Métricas**: Acurácia

## Dataset

O dataset utilizado neste projeto foi obtido do Kaggle e contém milhares de imagens de diferentes tipos de resíduos, rotulados como orgânicos ou recicláveis. A divisão entre treino, validação e teste seguiu a estrutura padrão:

- **Treinamento**: 80% dos dados
- **Validação**: 10% dos dados
- **Teste**: 10% dos dados

## Resultados

O modelo apresentou uma acurácia de aproximadamente **90%** na classificação dos resíduos, com um bom equilíbrio entre precisão e recall. Esses resultados mostram que a abordagem baseada no VGGNet pode ser eficaz na automação da classificação de lixo.

## Requisitos

- Python 3.x
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Pandas
