# Projeto Final – Análise de Dados (Télos & Thoughtworks)

Repositório criado para o projeto final do curso de **Análise de Dados** oferecido pela **Télos** em parceria com a **Thoughtworks**.  
O projeto aplica conceitos aprendidos ao longo do curso, incluindo coleta, tratamento, análise e visualização de dados para gerar insights e apoiar decisões.

## Panorama da Educação de Jovens e Adultos (EJA) no Brasil

Este projeto tem como objetivo analisar o panorama da Educação de Jovens e Adultos (EJA) no Brasil, explorando dados públicos educacionais para identificar padrões, desigualdades e tendências relacionadas à oferta e à participação nessa modalidade de ensino.

O trabalho foi desenvolvido em dupla durante o Bootcamp **“Vem pra Dados, Mulher!”**, promovido pela Télos, em parceria com a Thoughtworks e o Cesar School, com foco em Análise de Dados e empregabilidade feminina na área de tecnologia.

### 🧱 Arquitetura de Dados: Bronze → Silver → Gold

O projeto foi estruturado com base na arquitetura de camadas medallion (Bronze–Silver–Gold), aplicada dentro do ambiente Databricks, permitindo o fluxo organizado de ingestão, transformação e refinamento dos dados.

1. **Camada Bronze (Raw)**

Responsável pela ingestão dos dados brutos diretamente das fontes públicas, preservando a integridade e o formato original.
Aqui são realizadas apenas verificações básicas para garantir a leitura correta dos arquivos.

2. **Camada Silver (Trusted)**

Etapa de limpeza e padronização dos dados, na qual são aplicados tratamentos como:
- Remoção de duplicidades e valores inconsistentes;
- Normalização de colunas;
- Conversão de tipos de dados;
- Correção de caracteres especiais.

Essa camada garante a criação de uma base confiável e tratada para análises posteriores.

3. **Camada Gold (Refined)**

Fase final da pipeline, onde os dados tratados são refinados e consolidados em indicadores e métricas de negócio.
São realizadas agregações, cálculos e junções entre as tabelas, resultando nas visualizações e insights apresentados no Power BI.

### ⚙️ Estrutura do Repositório

```text
projeto-final/
│
├── notebooks/
│   ├── 1_bronze_ingestao.ipynb      # Ingestão e exploração inicial (camada Bronze)
│   ├── 2_silver_tratamento.ipynb    # Limpeza e padronização (camada Silver)
│   └── 3_gold_refined.ipynb         # Criação de métricas e indicadores (camada Gold)
│
├── data/
│   ├── bronze/                      # Dados brutos
│   ├── silver/                      # Dados tratados
│   └── gold/                        # Dados refinados
│
├── reports/
│   └── dashboard_powerbi.pbix       # Dashboard interativo no Power BI
│
└── README.md                        # Documentação principal
```

### 🧠 Tecnologias Utilizadas
- Python (PySpark e Pandas) → tratamento e transformação de dados
- Databricks → ambiente de processamento e integração com GitHub
- Power BI → criação de dashboards e visualização de insights
- Git e GitHub → versionamento e colaboração no desenvolvimento

### 📊 Dashboard Power BI

O dashboard apresenta uma visão consolidada sobre:
- Distribuição geográfica da EJA no Brasil;
- Indicadores de matrícula e evasão;
- Comparativos temporais e regionais;
- Análises qualitativas sobre acesso e permanência.

##👩‍💻 Autoria

Projeto desenvolvido por [Maryllian Vieira](https://www.linkedin.com/in/maryllian-vieira/)  e [Rafaela Santos](https://www.linkedin.com/in/rafaela-psantos/)
