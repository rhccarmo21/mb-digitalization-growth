# 📊 Digitalização e Crescimento Econômico - Análise de Dados

## 📋 Visão Geral
Este projeto analisa a relação entre indicadores de digitalização e crescimento econômico em **12 países entre 2010 e 2023**, utilizando dados do **Banco Mundial**.  
A pesquisa investiga como o acesso à internet, telefonia móvel e banda larga se correlacionam com o **PIB per capita** em diferentes estágios de desenvolvimento.

---

## 🔍 Principais Descobertas

### 📈 Correlações com PIB per capita
- **Internet (%):** 0.754 → Forte correlação positiva  
- **Banda larga:** 0.920 → Correlação muito forte  
- **Telefonia móvel:** 0.487 → Correlação moderada  

### 🌍 Disparidades entre Categorias de Países
| Indicador   | Países Desenvolvidos | Países Emergentes |
|-------------|----------------------|-------------------|
| Internet    | 87.2%                | 65.2%             |
| Banda larga | 35.1%                | 13.3%             |

---

## ❓ Perguntas de Pesquisa
- Existe uma relação significativa entre digitalização e desenvolvimento econômico?  
- Qual indicador de digitalização apresenta a correlação mais forte com o PIB?  
- Como evoluíram as disparidades digitais entre países desenvolvidos e emergentes?  
- Que políticas públicas podem acelerar a digitalização em países em desenvolvimento?  

---

## 🎯 Objetivos

### 🎯 Principal
Analisar estatisticamente a relação entre digitalização e crescimento econômico através de indicadores quantitativos.

### 📋 Específicos
- Coletar e processar dados de digitalização e PIB de 12 países (2010-2023)  
- Calcular correlações e taxas de crescimento anual (CAGR)  
- Identificar padrões temporais e disparidades regionais  
- Produzir visualizações informativas e um relatório executivo  
- Formular recomendações baseadas em evidências para gestores públicos  

---

## 📊 Metodologia

### 📁 Fontes de Dados
- **Banco Mundial (World Bank API)**  
- Período: 2010-2023  
- Países: 12 representantes de 3 categorias de desenvolvimento  

### 📊 Indicadores Analisados
- **Internet (%):** Penetração de internet na população  
- **Telefonia móvel (por 100):** Assinaturas de celular  
- **Banda larga (por 100):** Assinaturas de banda larga fixa  
- **PIB per capita (US$):** Indicador de desenvolvimento econômico  

### 🌐 Categorias de Países
- **Desenvolvidos:** EUA (USA), Alemanha (DEU), Japão (JPN), Suécia (SWE)  
- **Emergentes:** Brasil (BRA), México (MEX), Turquia (TUR), Malásia (MYS)  
- **Em desenvolvimento:** Nigéria (NGA), Índia (IND), Quênia (KEN), Bangladesh (BGD)  

### 📈 Técnicas Analíticas
- Análise de correlação (coeficiente de Pearson)  
- Cálculo de **CAGR** (Taxa de Crescimento Anual Composta)  
- Análise temporal (séries históricas 2010-2023)  
- Análise comparativa entre categorias de países  
- Visualização de dados (gráficos, heatmaps, scatter plots)  

---

## 🛠️ Tecnologias Utilizadas
- **Python 3.8+**  
- **Pandas** - Manipulação e análise de dados  
- **NumPy** - Cálculos numéricos e estatísticos  
- **Matplotlib** - Visualizações básicas  
- **Seaborn** - Visualizações estatísticas avançadas  
- **Requests** - Acesso à API do Banco Mundial  
- **JSON** - Processamento de dados da API  

---

## 📁 Estrutura do Projeto
```
mb-digitalization-growth/
│
├── mb_digitalization_growth.py              # Script principal de análise
├── mb_digitalization_growth_processed.csv   # Dados processados (2010-2023)
├── mb_digitalization_growth_rates.csv       # Taxas de crescimento (CAGR)
├── relatorio_digitalizacao_crescimento.txt  # Relatório executivo resumido
├── requirements.txt                         # Dependências do projeto
└── README.md                                # Documentação do projeto
```

---

## 🚀 Como Executar o Projeto

### ⚙️ Pré-requisitos
Instale as dependências com:
```bash
pip install pandas numpy matplotlib seaborn requests
```

### ▶️ Execução
Execute a análise completa com:
```bash
python mb_digitalization_growth.py
```

---

## 📤 Saídas Geradas
- 4 gráficos de evolução temporal por categoria de país  
- 1 heatmap de taxas de crescimento anual (CAGR)  
- 3 scatter plots de PIB vs indicadores digitais  
- 2 arquivos CSV com dados processados e taxas de crescimento  
- 1 relatório executivo em formato texto com principais conclusões  

---

## 📈 Resultados Detalhados

### 1. 📶 Forte Correlação entre Digitalização e PIB
- Banda larga → correlação mais forte (0.920)  
- Internet → correlação forte (0.754)  
- Telefonia móvel → correlação moderada (0.487)  

### 2. 🌍 Grandes Disparidades Digitais
- Internet: 87.2% vs 65.2% (diferença: 22 pp)  
- Banda larga: 35.1% vs 13.3% (diferença: 21.8 pp)  

### 3. 📈 Crescimento Acelerado em Países em Desenvolvimento
- Maiores taxas de crescimento anual (CAGR)  
- Processo de convergência digital em curso, mas ainda insuficiente  

---

## 💡 Recomendações de Política Pública

### 🌱 Para Países em Desenvolvimento
- Priorizar infraestrutura de banda larga  
- Programas de inclusão digital com internet móvel acessível  
- Capacitação digital para aproveitar investimentos em infraestrutura  

### 🚀 Para Países Emergentes
- Manter investimentos em infraestrutura digital de alta qualidade  
- Promover ecossistemas de inovação e startups  
- Regulamentações equilibradas entre inovação e proteção ao consumidor  

### 🏛️ Para Países Desenvolvidos
- Investir em tecnologias de próxima geração (5G, fibra ótica, IoT)  
- Inclusão digital de populações vulneráveis  
- Liderar esforços globais de governança digital  

---

## 🌍 Implicações Globais
- A digitalização pode acelerar o crescimento econômico e reduzir desigualdades  
- A lacuna digital permanece significativa, sobretudo em banda larga fixa  
- A pandemia acelerou oportunidades de saltos tecnológicos  
- Países com investimentos estratégicos em digitalização crescem acima da média  

---

## 🔮 Perspectivas Futuras
- 5G, IoT e IA devem intensificar o impacto econômico da digitalização  
- A convergência digital seguirá, mas desigualdades persistirão  
- Novas métricas de digitalização (ex.: qualidade da conexão, habilidades digitais) ganharão relevância  
- A governança digital global será tema estratégico central na próxima década  

---

## 📚 Referências
- World Bank Open Data  
- ITU Digital Development reports  
- OECD Digital Economy Outlook  
- Relatórios regionais de desenvolvimento digital  

---

## 👥 Público-Alvo
- Gestores públicos e formuladores de políticas  
- Legisladores e assessores parlamentares  
- Analistas econômicos e de desenvolvimento  
- Jornalistas especializados em tecnologia e economia  
- Acadêmicos e pesquisadores em estudos de desenvolvimento  
- Organizações internacionais e think tanks  

---

## 📄 Licença
Este projeto é disponibilizado para fins educacionais e de pesquisa.  
Os dados são de domínio público via Banco Mundial.
