# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Bem-vindo ao desafio de projeto "Previsão de Estoque Inteligente na AWS com SageMaker Canvas. Neste Lab DIO, você aprenderá a usar o SageMaker Canvas para criar previsões de estoque baseadas em Machine Learning (ML). Siga os passos abaixo para completar o desafio!

## 🎯 Objetivos Deste Projeto (Lab)

![image](https://github.com/digitalinnovationone/lab-aws-sagemaker-canvas-estoque/assets/730492/72f5c21f-5562-491e-aa42-2885a3184650)

- Com base em datasets, gerar análises e predições a respeito da variação do estoque, considerando diferentes variáveis. 


## 🚀 Passo a Passo

### 1. Selecionar Dataset

-   O dataset utilizado foi disponibilizado neste projeto, na seção de datasets.
-   Possuindo exatas 1.001 rows e pouco mais de 5.000 células, se trata de um dataset até que robusto.
  ![print dataset](https://github.com/user-attachments/assets/c4ed8b6d-887b-4ef2-9482-3113d38c5b5e)


### 2. Construir/Treinar

-   Ao importar o dataset, devemos escolher a **QUANTIDADE_ESTOQUE** como target e a tabela **ID_PRODUTO** como item id.
-   Não fiz muitas alterações nas configurações, apenas adicionei a **use schedule holliday**.
 ![print configure model](https://github.com/user-attachments/assets/fa6f0105-eb81-4de4-9ee0-4475743be1bd)


### 3. Analisar

-   Com tudo já configurado, utilizei o método **Quick build** para realizar a análise.
-   Considero que as métricas de Avg.wQL, WAPE, MAPE, RMSE e WASE bem satistfatórias.
  ![print stats](https://github.com/user-attachments/assets/e2021304-bc7b-4083-a27f-ecd5cd306e38)
- Outro ponto de vista: **PRECO** = 9.14% **HOLLIDAY_BR** = 2.79% **FLAG_PROMOCAO** = 0.00%
  ![print stats 2](https://github.com/user-attachments/assets/3c93edb9-8c84-4251-a866-deaffd298d47)



### 4. Prever

-   Aos realizar as predições de maneira singular, podemos encontrar métricas como **P10**, **P50** e **P90**.
-   **P10** é um indicativo, digamos, "pessimista".
-   **P50** seria um indicativo neutro.
-   Enquanto o **P90** é mais otimista e prevê números mais satisfatórios.
![print predict ](https://github.com/user-attachments/assets/8d5f3916-b8de-47dd-9bd4-235a3a379609)

