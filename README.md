# PISI3 Grupo 05

## Descrição
Este projeto é uma aplicação de análise de dados e aprendizado de máquina que utiliza dados do Yelp para realizar clustering, classificação e análise exploratória de dados (EDA).

## Estrutura do Projeto
- `streamlit/`: Contém os arquivos para a interface do usuário utilizando Streamlit.
  - `st.py`: Script principal do Streamlit.
  - `app.py`: Script adicional do Streamlit.
- `machine-learning/`: Contém notebooks de aprendizado de máquina.
  - `clustering.ipynb`: Notebook para clustering.
  - `classification_2.ipynb`: Notebook para classificação.
  - `classification_balanced.ipynb` : Notebook para classificação balanceada.
- `dataset/`: Contém o dataset utilizado no projeto.
  - `yelp_academic_dataset_business_cleaned.csv`: Dataset do Yelp.

## Instalação
1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/pisi3-grupo05.git
   cd pisi3-grupo05
   ```

2. Crie um ambiente virtual e ative-o:
   ```bash
   python -m venv venv
   source venv/bin/activate  # No Windows use `venv\Scripts\activate`
   ```

3. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

## Uso
1. Execute a aplicação Streamlit:
   ```bash
   streamlit run streamlit/st.py
   ```

2. Abra os notebooks de aprendizado de máquina para explorar as análises:
   - `machine-learning/clustering.ipynb`
   - `machine-learning/classification_2.ipynb`
   - `machine-learning/classification_balanced.ipynb`

## 🌟 Destaque de minha Contribuição **(Igor Queiroz)**
Desenvolvimento do App Interativo e Data Visualization

Fiquei responsável pela construção de toda a interface visual e da aplicação web interativa utilizando **Streamlit** e também tomei frente de **Classificação Avançada e Interpretabilidade de Modelos**.

O foco desta contribuição foi ir além da predição básica, construindo pipelines robustos de Machine Learning, lidando com o desbalanceamento das classes do Yelp e aplicando técnicas de Inteligência Artificial Explicável (XAI) para entender o comportamento dos algoritmos. Utilizando **Streamlit** para democratizar o acesso aos complexos resultados de Machine Learning e Análise de Dados, traduzindo números brutos em uma experiência visual, fluida e de fácil compreensão para qualquer usuário, unindo habilidades de Engenharia de Software e Ciência de Dados.

**Principais frentes técnicas desta implementação:**
* **Desenvolvimento Front-end em Streamlit:** Criação e estruturação de toda a interface do usuário (`st.py` e `app.py`), garantindo navegação intuitiva e design responsivo para a apresentação do projeto.
* **Análise Exploratória de Dados (EDA) Interativa:** Transformação do *dataset* do Yelp em painéis dinâmicos, permitindo a filtragem em tempo real e a visualização de tendências e distribuições de negócios por meio de gráficos interativos.
* **Visualização de Modelos de Classificação:** Integração da saída dos modelos (KNN, Random Forest, XGBoost) diretamente no painel. Implementação de visualizações claras para os Relatórios de Classificação e Matrizes de Confusão, facilitando a interpretação do desempenho preditivo.
* **Projeção de Clusterização:** Construção de visualizações que mapeiam e explicam os agrupamentos (*clusters*) gerados pelos algoritmos não supervisionados, evidenciando a segmentação dos dados do Yelp na interface gráfica.
* **Desenvolvimento de Modelos de Machine Learning:** Implementação e ajuste de hiperparâmetros de algoritmos de alta performance, incluindo **K-Nearest Neighbors (KNN)**, **Random Forest** e **XGBoost**.
* **Pipelines e Balanceamento de Dados:** Criação de fluxos de processamento utilizando `Pipeline` e `ColumnTransformer` do Scikit-Learn, integrados com **SMOTE** (Imbalanced-learn) para tratar o desbalanceamento de dados de forma segura e automatizada.
* **Avaliação Rigorosa de Desempenho:** Geração e análise comparativa de métricas avançadas para todos os modelos (incluindo Regressão Logística). Foram desenvolvidos *Classification Reports*, *Matrizes de Confusão*, e curvas ROC-AUC para garantir a confiabilidade das predições.
* **Interpretabilidade com SHAP:** Implementação de análise de valores **SHAP** para desvendar a "caixa preta" dos modelos. Essa etapa permitiu mapear o impacto e o peso de cada variável (feature) nas predições finais, fornecendo *insights* de negócio claros e justificáveis sobre as avaliações dos estabelecimentos no Yelp.

## Licença
Este projeto está licenciado sob a Licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
