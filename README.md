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
digitalizacao_crescimento/
│
├── mb_digitalization_growth.py # Script principal de análise
├── mb_digitalization_growth_processed.csv # Dados processados (2010-2023)
├── mb_digitalization_growth_rates.csv # Taxas de crescimento (CAGR)
├── relatorio_digitalizacao_crescimento.txt # Relatório executivo resumido
├── requirements.txt # Dependências do projeto
└── README.md # Documentação do projeto


## 🚀 Como Executar o Projeto

### ⚙️ Pré-requisitos
```bash
# Instalar dependências
pip install pandas numpy matplotlib seaborn requests

▶️ Execução
# Executar análise completa
python mb_digitalization_growth.py

📤 Saídas Geradas
4 gráficos de evolução temporal por categoria de país

1 heatmap de taxas de crescimento anual (CAGR)

3 scatter plots de PIB vs indicadores digitais

2 arquivos CSV com dados processados e taxas de crescimento

1 relatório executivo em formato texto com principais conclusões

📈 Resultados Detalhados
1. 📶 Forte Correlação entre Digitalização e PIB
A análise revelou correlações positivas significativas entre todos os indicadores de digitalização e o PIB per capita:

Banda larga mostra a correlação mais forte (0.920), indicando que países com maior penetração de banda larga tendem a ter PIB per capita mais alto.

Internet também apresenta correlação forte (0.754), reforçando a importância do acesso à internet para o desenvolvimento econômico.

Telefonia móvel apresenta correlação moderada (0.487), sugerindo saturação deste indicador em muitos países.

2. 🌍 Grandes Disparidades Digitais
As disparidades entre países desenvolvidos e emergentes são particularmente evidentes:

Internet: Diferença de 22 pontos percentuais (87.2% vs 65.2%)

Banda larga: Diferença de 21.8 pontos percentuais (35.1% vs 13.3%)

3. 📈 Crescimento Acelerado em Países em Desenvolvimento
Os países em desenvolvimento apresentam as maiores taxas de crescimento anual (CAGR) nos indicadores de digitalização, indicando um processo de convergência digital, embora em ritmo insuficiente para eliminar as disparidades atuais.

💡 Recomendações de Política Pública
🌱 Para Países em Desenvolvimento
Priorizar infraestrutura de banda larga como motor de desenvolvimento econômico

Implementar programas de inclusão digital com internet móvel acessível

Desenvolver políticas de capacitação digital para aproveitar investimentos em infraestrutura

🚀 Para Países Emergentes
Manter investimentos em infraestrutura digital de alta qualidade

Promover ecossistemas de inovação e startups de tecnologia

Desenvolver regulamentações que equilibrem inovação e proteção ao consumidor

🏛️ Para Países Desenvolvidos
Investir em tecnologias de próxima geração (5G, fibra ótica, IoT)

Enfrentar desafios de inclusão digital em populações vulneráveis

Liderar esforços globais de padrões e governança digital

🌍 Implicações Globais
A digitalização representa uma oportunidade única para países em desenvolvimento acelerarem seu crescimento econômico e reduzirem desigualdades

A lacuna digital entre nações desenvolvidas e em desenvolvimento permanece significativa, particularmente em banda larga fixa

A aceleração digital pós-pandemia criou oportunidades únicas para saltos tecnológicos em países em desenvolvimento

Países que investem estrategicamente em infraestrutura digital demonstram taxas de crescimento econômico acima da média

🔮 Perspectivas Futuras
Tecnologias emergentes (5G, IoT, IA) devem amplificar o impacto da digitalização no crescimento econômico

A convergência digital entre países deve continuar, mas em ritmo insuficiente para eliminar disparidades significativas na próxima década

Novas métricas de digitalização (qualidade de conexão, habilidades digitais) ganharão importância na avaliação do desenvolvimento econômico

A governança digital global se tornará questão estratégica cada vez mais importante

📚 Referências
World Bank Open Data

ITU Digital Development reports

OECD Digital Economy Outlook

Relatórios de desenvolvimento digital regional

👥 Público-Alvo
Gestores públicos e formuladores de políticas

Legisladores e assessores parlamentares

Analistas econômicos e de desenvolvimento

Jornalistas especializados em tecnologia e economia

Acadêmicos e pesquisadores em estudos de desenvolvimento

Organizações internacionais e think tanks

📄 Licença
Este projeto é disponibilizado para fins educacionais e de pesquisa. Os dados são de domínio público via Banco Mundial.


