# 🍎 Image Classification with Fruits 360 Dataset

Este projeto tem como objetivo desenvolver um **modelo de classificação de imagens** capaz de identificar diferentes tipos de frutas utilizando técnicas de **Deep Learning e Visão Computacional**. O Projeto foi realizado com o dataset **Fruits 360**, aplicando **Transfer Learning com MobileNetV2** para obter bons resultados mesmo com um conjunto de dados limitado.

---

## 📌 Definição do Problema

O problema abordado consiste em classificar imagens de frutas em múltiplas categorias, com base apenas nas informações visuais contidas nos pixels da imagem. Trata-se de um problema de **classificação supervisionada multiclasse**, com aplicações práticas em sistemas de automação, controle de qualidade e reconhecimento visual.

---

## 📌 Coleta dos Dados

Os dados utilizados neste projeto foram obtidos a partir do **Fruits 360 Dataset**, um conjunto de dados público amplamente utilizado em estudos de visão computacional.  
As imagens estão organizadas em diretórios, onde cada pasta representa uma classe específica de fruta, permitindo a rotulagem automática dos dados.

🔗 **Link para download do dataset (Kaggle):**  
https://www.kaggle.com/datasets/shreyapmaher/fruits-dataset-images

---

## 📌 Limpeza e Tratamento dos Dados

Nesta etapa, as imagens passaram por processos de:
- Redimensionamento para um tamanho padrão compatível com a arquitetura do modelo
- Normalização dos valores dos pixels

Além disso, foi aplicada **data augmentation** durante o treinamento para aumentar a diversidade do conjunto de dados e reduzir o risco de overfitting.

---

## 📌 Análise Exploratória dos Dados

A análise exploratória envolveu:
- Visualização de imagens por classe
- Verificação da distribuição de imagens entre as categorias
- Avaliação da padronização visual das imagens (fundo, iluminação e enquadramento)

Essa etapa permitiu compreender melhor as características do dataset e orientar decisões sobre o modelo e o pré-processamento.

---

## 📌 Seleção de Variáveis

Como se trata de um problema de visão computacional, as **variáveis de entrada** são os próprios pixels das imagens.  
A extração de características é realizada automaticamente pelo modelo de deep learning, eliminando a necessidade de seleção manual de features.

---

## 📌 Treinamento e Validação do Modelo

O modelo foi desenvolvido utilizando **Transfer Learning com a arquitetura MobileNetV2**, aproveitando pesos pré-treinados na base ImageNet.  
O conjunto de dados foi dividido em **treinamento e validação**, permitindo avaliar a capacidade de generalização do modelo em dados não vistos durante o treinamento.

---

## 📌 Avaliação de Métricas

O desempenho do modelo foi avaliado utilizando métricas apropriadas para classificação multiclasse, como:
- **Acurácia**
- **Loss (entropia cruzada categórica)**

Os resultados indicaram boa convergência do modelo, com curvas de treino e validação próximas, sugerindo uma boa capacidade de generalização.

---

## 💼 Aplicação no Mercado e Impacto para Negócios

Soluções de classificação de imagens como a desenvolvida neste projeto podem gerar **impacto direto no desempenho financeiro de empresas**, especialmente nos setores de varejo, logística e agronegócio.

Alguns exemplos de aplicação incluem:
- **Automação de caixas em supermercados**, reduzindo erros humanos na identificação de produtos e acelerando o atendimento ao cliente
- **Controle de qualidade automatizado**, identificando frutas incorretas ou fora do padrão antes da distribuição
- **Redução de custos operacionais**, diminuindo a necessidade de inspeção manual
- **Otimização de estoque**, evitando perdas por classificação incorreta ou falhas no controle de produtos
- **Aumento da escalabilidade**, permitindo que a empresa processe grandes volumes de produtos sem aumento proporcional de custos

Esses fatores contribuem diretamente para **economia de recursos**, **melhoria da eficiência operacional** e **aumento da margem de lucro**.

---

## 🚀 Tecnologias Utilizadas

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Jupyter Notebook

---

## 📊 Resultados

O modelo alcançou uma acurácia próxima de **90% no conjunto de validação**, demonstrando que o uso de transfer learning aliado a técnicas de regularização é eficaz mesmo em cenários com poucos dados por classe.

---
