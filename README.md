# 🌎 Sismos-Globais — Análise de Dados Sísmicos

Este repositório contém um conjunto completo de scripts, análises e visualizações voltados para o estudo de **eventos sísmicos globais**, utilizando dados reais fornecidos por instituições reconhecidas internacionalmente.

O projeto aborda desde a **coleta e limpeza da base de dados** até a **análise temporal, espacial e estatística**, incluindo correlação, testes de hipótese e identificação de padrões.

---

## 📌 1. Sobre o Dataset

### 🔍 **Origem da Base de Dados**

O conjunto de dados utilizado neste projeto foi obtido no **USGS Earthquake Catalog** (United States Geological Survey), uma das fontes mais confiáveis do mundo para dados sísmicos. O USGS é uma instituição científica do governo norte‑americano especializada em monitoramento geológico, sismológico e ambiental.

👉 Site oficial: earthquake.usgs.gov
[USGS](https://earthquake.usgs.gov/earthquakes/search/)

### 🛰️ **Como os dados são coletados**

Os dados do USGS são captados através de:

* **Rede global de sismógrafos** espalhados por dezenas de países;
* **Sensores sísmicos de alta sensibilidade**, que detectam intensidade, profundidade e localização dos tremores;
* **Estações de monitoramento geológico** integradas internacionalmente;
* Processamento via **algoritmos automáticos + validação humana**, garantindo precisão.

A combinação desses elementos torna o dataset altamente confiável para estudos exploratórios e estatísticos.

### 📊 **Tipo de dados disponíveis**

O dataset inclui informações como:

* Data e hora do evento (UTC)
* Magnitude do sismo
* Localização (latitude e longitude)
* Profundidade do foco
* Região/descrição do local
* ID do evento no catálogo
* Parâmetros de qualidade do registro

Esse tipo de dado é ideal para análises temporais, espaciais e estatísticas.

---

## 📁 2. O que foi feito neste repositório

### ✔️ **1. Coleta e armazenamento dos dados**

* Download dos registros sísmicos direto da API oficial do USGS.
* Conversão para CSV/Parquet conforme necessidade das análises.
* Padronização de colunas e formatação das datas para uso em Python.

### ✔️ **2. Limpeza e preparação da base**

* Tratamento de valores nulos
* Conversão de tipos (datas, floats etc.)
* Ajuste de timezones quando necessário
* Remoção de registros inválidos

### ✔️ **3. Análises exploratórias (EDA)**

Inclui:

* Distribuição de magnitudes
* Quantidade de eventos por período
* Localização geográfica dos tremores
* Identificação de padrões sazonais ou picos de atividade

### ✔️ **4. Análises estatísticas avançadas**

* Cálculo de correlação (Pearson) entre magnitude e tempo
* Testes de significância
* Regressão linear para observar tendências
* Identificação de outliers

### ✔️ **5. Visualizações**

O projeto inclui vários gráficos gerados em Python:

* Séries temporais
* Histogramas
* Mapas de dispersão geográfica
* Gráfico de regressão (magnitude x tempo)
* ACF/PACF para estudo de dependência temporal

### ✔️ **6. Processamento automático**

Scripts organizados para:

* Rodar análises completas
* Exportar gráficos
* Facilitar a reprodução do projeto em qualquer ambiente

---

## ⚙️ 3. Tecnologias utilizadas

* **Python 3.x**
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Statsmodels
* SciPy
* Requests

---

## 🚀 4. Objetivo do Projeto

O objetivo central é fornecer uma análise clara e completa sobre a atividade sísmica global, permitindo responder perguntas como:

* Existe tendência temporal nas magnitudes?
* Há picos de atividade sísmica?
* Como se distribuem os tremores ao longo do tempo?
* É possível prever comportamento futuro com análise estatística básica?

---

## 📂 5. Estrutura

/notebooks/ Onde estão os notebooks
    /Earthquake_ACF_e_PACF.ipynb/
    /Earthquake_ARIMA.ipynb/
    /Earthquake_Previsoes.ipynb/
    /Earthquake_Série_Temporal.ipynb/

/data/ 'Dataset salvo utilizado (tentei deixar o mais recente possivel)
    /dataset_sismos.csv/

tema_9.md   (tema que nos foi designado)
README.md   (Este arquivo)


---

## 📂 6. Como reproduzir

Pode baixar os notebooks criados, quanto pode ir pelo link que esta no notebook, que irá te direcionar para o ambiente do Google o Colab (Onde todo o processo de criação aconteceu).

```bash
git clone https://github.com/GiPaiva/Sismos-Globais.git
cd notebooks
```

---

## 🔗 8. Referencias usadas

https://colab.research.google.com/github/redis-developer/redis-ai-resources/blob/main/python-recipes/recommendation-systems/01_collaborative_filtering.ipynb#scrollTo=RulVkjtBncuR
https://colab.research.google.com/github/redis-developer/redis-ai-resources/blob/main/python-recipes/redis-intro/00_redis_intro.ipynb#scrollTo=o3Nc1Y4vVfav
https://colab.research.google.com/github/sujikathir/Sales-Forecasting/blob/main/Arima_Model_for_Sales_Data.ipynb
https://www.ibm.com/br-pt/think/topics/arima-model
https://www.ime.unicamp.br/~cnaber/Aula_ARIMA_P1_ST_ME607_1S_2024.pdf
https://support.minitab.com/pt-br/minitab/help-and-how-to/statistical-modeling/time-series/how-to/arima/interpret-the-results/key-results/
https://www-usgs-gov.translate.goog/faqs/can-you-predict-earthquakes?_x_tr_sl=en&_x_tr_tl=pt&_x_tr_hl=pt&_x_tr_pto=sge#:~:text=Os%20cientistas%20do%20USGS%20só,local%20e%203)%20a%20magnitude.
https://analisemacro.com.br/data-science/python/estacionariedade_series_temporais/#:~:text=Estacionariedade%20Estacionariedade%20de%20uma%20série%20temporal%20é,autocovariância)%20não%20mudam%20ao%20longo%20do%20tempo.
https://redis.io/blog/running-redis-on-google-colab/


---

## ✨ 9. Autora

**Giovanna Paiva Alves** — Ciência da Computação 🎓
**Matheus Sanchez Duda** — Ciência da Computação 🎓

Sempre aberta a sugestões e melhorias 😊