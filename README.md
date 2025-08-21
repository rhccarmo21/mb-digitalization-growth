# 📊 Digitalização e Crescimento Econômico - Análise de Dados

## 📋 Visão Geral

Este projeto analisa a relação entre indicadores de digitalização e crescimento econômico em 12 países entre 2010 e 2023, utilizando dados do Banco Mundial. A pesquisa investiga como o acesso à internet, telefonia móvel e banda larga se correlacionam com o PIB per capita em diferentes estágios de desenvolvimento.

## 🔍 Principais Descobertas

### 📈 Correlações com PIB per capita
- **Internet (%):** 0.754 (Forte correlação positiva)
- **Banda larga:** 0.920 (Correlação muito forte) 
- **Telefonia móvel:** 0.487 (Correlação moderada)

### 🌍 Disparidades entre Categorias de Países
| Indicador | Países Desenvolvidos | Países Emergentes |
|-----------|----------------------|-------------------|
| Internet | 87.2% | 65.2% |
| Banda larga | 35.1% | 13.3% |

## ❓ Perguntas de Pesquisa

1. **Existe uma relação significativa** entre digitalização e desenvolvimento econômico?
2. **Qual indicador de digitalização** apresenta a correlação mais forte com o PIB?
3. **Como evoluíram** as disparidades digitais entre países desenvolvidos e emergentes?
4. **Que políticas públicas** podem acelerar a digitalização em países em desenvolvimento?

## 🎯 Objetivos

### 🎯 Principal
Analisar estatisticamente a relação entre digitalização e crescimento econômico através de indicadores quantitativos.

### 📋 Específicos
- Coletar e processar dados de digitalização e PIB de 12 países (2010-2023)
- Calcular correlações e taxas de crescimento anual (CAGR)
- Identificar padrões temporais e disparidades regionais
- Produzir visualizações informativas e um relatório executivo
- Formular recomendações baseadas em evidências para gestores públicos

## 📊 Metodologia

### 📁 Fontes de Dados
- **Banco Mundial** (World Bank API)
- Período: 2010-2023
- Países: 12 representantes de 3 categorias de desenvolvimento

### 📊 Indicadores Analisados
1. **Internet (%)** - Penetração de internet na população
2. **Telefonia móvel (por 100)** - Assinaturas de celular
3. **Banda larga (por 100)** - Assinaturas de banda larga fixa  
4. **PIB per capita (US$)** - Indicador de desenvolvimento econômico

### 🌐 Categorias de Países
- **Desenvolvidos**: Estados Unidos (USA), Alemanha (DEU), Japão (JPN), Suécia (SWE)
- **Emergentes**: Brasil (BRA), México (MEX), Turquia (TUR), Malásia (MYS)  
- **Em desenvolvimento**: Nigéria (NGA), Índia (IND), Quênia (KEN), Bangladesh (BGD)

### 📈 Técnicas Analíticas
- **Análise de correlação** (coeficiente de Pearson)
- **Cálculo de CAGR** (Taxa de Crescimento Anual Composta)
- **Análise temporal** (séries históricas 2010-2023)
- **Análise comparativa** entre categorias de países
- **Visualização de dados** (gráficos, heatmaps, scatter plots)

## 🛠️ Tecnologias Utilizadas

- **Python 3.8+**
- **Pandas** - Manipulação e análise de dados
- **NumPy** - Cálculos numéricos e estatísticos
- **Matplotlib** - Visualizações básicas
- **Seaborn** - Visualizações estatísticas avançadas
- **Requests** - Acesso à API do Banco Mundial
- **JSON** - Processamento de dados da API

## 📁 Estrutura do Projeto
