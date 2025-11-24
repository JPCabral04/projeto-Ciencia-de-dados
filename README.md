# Projeto 2 - Análise de Dados e Machine Learning

Este projeto foi desenvolvido para a disciplina de programação, cumprindo os requisitos de aplicação de técnicas de Ciência de Dados e Machine Learning utilizando Python.

## 📋 Descrição do Projeto

O objetivo deste trabalho é realizar um fluxo completo de análise de dados, desde o pré-processamento até a aplicação de algoritmos de aprendizado de máquina não supervisionado (PCA, K-Means) e supervisionado (SVM).

O projeto utiliza o dataset **Healthcare Diabetes**, analisando indicadores de saúde para classificação e agrupamento relacionados a diabetes.

## 📂 Estrutura dos Arquivos

O projeto está organizado em notebooks sequenciais para facilitar o entendimento do fluxo de dados:

- **`dataset.txt`**: Contém a referência/link para a fonte original do dataset utilizado.
- **`requirements.txt`**: Lista das bibliotecas Python necessárias para executar o projeto.

### Notebooks

1.  **`0-preprocessing.ipynb`** (Pré-processamento)

    - Carregamento do dataset original (`Healthcare-Diabetes.csv`).
    - Limpeza de dados: Tratamento de valores nulos (zeros inválidos) substituindo pela mediana.
    - Geração do arquivo processado `diabetes_final.csv` usado nos passos seguintes.

2.  **`1-PCA.ipynb`** (Redução de Dimensionalidade)

    - **Técnica:** PCA (Principal Component Analysis).
    - **Pré-processamento:** Utilização do `RobustScaler` para normalização.
    - **Objetivo:** Reduzir a dimensionalidade dos dados para facilitar a visualização.
    - **Visualização:** Gráfico de dispersão (Scatter Plot) utilizando **Matplotlib**.

3.  **`2-KMeans.ipynb`** (Agrupamento/Clustering)

    - **Técnica:** K-Means Clustering.
    - **Análise de K-ideal:** Utilização dos métodos **Silhouette Score**, **Davies-Bouldin Score** e **Método do Cotovelo** para determinar o número ótimo de clusters.
    - **Visualização:** Utilização de **t-SNE** para visualização dos clusters em 2D.

4.  **`3-SVM.ipynb`** (Técnica Livre)
    - **Técnica:** SVM (Support Vector Machine) com kernel RBF.
    - **Pré-processamento:** Utilização do `StandardScaler`.
    - **Objetivo:** Classificação supervisionada (Saudável vs. Diabético).
    - **Métricas:** Acurácia, Relatório de Classificação e Matriz de Confusão.

## 🚀 Como Executar

1.  Certifique-se de ter o Python instalado.
2.  Instale as dependências listadas no arquivo `requirements.txt`:
    ```bash
    pip install -r requirements.txt
    ```
3.  Execute os notebooks na ordem numérica (0 a 3) utilizando o Jupyter Notebook ou VS Code.

## 📝 Requisitos Atendidos (Enunciado)

- [x] **Dataset:** Referenciado em `dataset.txt`.
- [x] **Notebook 1:** Redução de dimensionalidade com visualização (Matplotlib).
- [x] **Notebook 2:** Agrupamento usando K-Means + Análise de K-ideal + Visualização.
- [x] **Notebook 3:** Técnica livre (SVM) usando Scikit-learn.

- [x] **Entrega:** Arquivos organizados e pastas desnecessárias (`__pycache__`, `venv`, etc.) excluídas.

---
