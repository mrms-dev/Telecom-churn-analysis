# Telecom X - Análise de Evasão de Clientes (Churn)

## Descrição do Projeto
Este projeto tem como objetivo analisar o alto índice de cancelamentos (*churn*) da empresa fictícia Telecom X. A análise foi realizada utilizando técnicas de ETL (Extração, Transformação e Carga) e Análise Exploratória de Dados (EDA), com foco em identificar os principais fatores que influenciam a evasão de clientes e gerar insights estratégicos para retenção.

## Tecnologias Utilizadas

**Linguagem e Ambiente:**

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Google Colab](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252)

**Bibliotecas de Manipulação e Visualização:**

![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge) ![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge) ![Missingno](https://img.shields.io/badge/Missingno-555555?style=for-the-badge)

## Propósito e Objetivo da Análise
Identificar padrões de comportamento dos clientes que cancelam os serviços, apoiando decisões estratégicas da empresa Telecom X e preparando a base para futuros modelos preditivos de *machine learning* voltados para o *churn*. O propósito final é diagnosticar a causa-raiz da perda de clientes para propor ações de retenção eficazes.

## Exemplos de Gráficos e Insights Obtidos

Através do processo de *drill-down* nos dados, a análise revelou uma taxa de insatisfação elevada. Abaixo estão os principais insights suportados pelas visualizações geradas no projeto:

* **Evasão Precoce (Early Churn):** O vazamento de clientes é massivo no **1º mês de uso** (mediana geral de permanência de apenas 10 meses para quem cancela).
* **O Risco da Falta de Fidelidade:** Clientes no contrato **Mensal** apresentam uma taxa de mortalidade de **42.7%**.
* **O Paradoxo da Fibra Óptica:** O produto mais caro e avançado do portfólio é o maior responsável pelas perdas (**41.9%** de taxa de cancelamento).
* **Principal Fator de Abandono (Falta de Suporte):** A ausência de uma rede de apoio é fatal para a retenção. Entre os clientes de Fibra Óptica que cancelaram o serviço, impressionantes **84.9% não possuíam Suporte Técnico** contratado, contra apenas 15.1% que tinham o serviço. Isso comprova que vender um produto *premium* sem amparo técnico para instabilidades iniciais é o gatilho definitivo para a evasão.

<div align="center">
  <img src="Fibra%20Óptica%20vs%20DSL.png" alt="Gráfico: Fibra Óptica vs DSL" width="700">
  <br><br>
  <img src="Falta%20de%20Suporte%20Técnico.png" alt="Gráfico: Falta de Suporte Técnico" width="700">
</div>

## Etapas do Projeto
* **1.** Configuração do ambiente e importação das bibliotecas.
* **2.** Coleta de dados via API (formato JSON).
* **3.** Processo de ETL (tratamento, normalização e limpeza dos dados).
* **4.** Conversão de variáveis e padronização dos dados.
* **5.** Análise Exploratória de Dados (EDA) com visualizações.
* **6.** Relatório final com insights estratégicos.

## Principais Atividades Realizadas
- [x] Extração dos dados diretamente da API da Telecom X.
- [x] Normalização de colunas aninhadas (JSON).
- [x] Limpeza e tratamento de dados inconsistentes.
- [x] Conversão de variáveis numéricas (`TotalCharges`).
- [x] Padronização da variável alvo `Churn` (Cancelado / Não cancelado).
- [x] Criação de gráficos para análise de evasão de clientes.

## Estrutura do Repositório e Organização dos Arquivos
* `.gitignore` → Arquivo de configuração para ignorar rastreios indesejados no Git.
* `Falta de Suporte Técnico.png` → Imagem do gráfico de análise de suporte técnico.
* `Fibra Óptica vs DSL.png` → Imagem do gráfico de comparação de tecnologias de internet.
* `LICENSE` → Arquivo contendo os termos da licença MIT.
* `README.md` → Documentação principal do projeto.
* `Telecom_churn_analysis.ipynb` → Notebook completo com o código em Python (ETL, EDA e visualizações).
* `telecomx_churn_limpo.csv` → Base de dados tratada (versão inicial do processo de ETL).
* `telecomx_churn_limpo_atualizado.csv` → Base de dados final após limpeza, padronização e preparação para análise.

## Instruções para Executar o Notebook

Para reproduzir esta análise na sua máquina local ou em nuvem, siga os passos abaixo:

1. Clone este repositório para a sua máquina:
   ```bash
   git clone [https://github.com/mrms-dev/Telecom-churn-analysis.git](https://github.com/mrms-dev/Telecom-churn-analysis.git)

## Autor

**Marcos Rivanio Marinho dos Santos**
* **Email:** marcosrivanio@gmail.com
* **GitHub:** [https://github.com/mrms-dev](https://github.com/mrms-dev)
* **LinkedIn:** [https://www.linkedin.com/in/marcos-rivanio-santos/](https://www.linkedin.com/in/marcos-rivanio-santos/)

> *Projeto desenvolvido como parte de um portfólio profissional em Data Science, com foco em análise de dados, pensamento analítico e resolução de problemas de negócio.*

**Aberto a feedbacks, colaborações e oportunidades.**

##Licença
Este projeto está licenciado sob a licença MIT - sinta-se livre para utilizar, clonar e adaptar o código para os seus próprios estudos e projetos.
