---
jupyter:
  kernelspec:
    display_name: Python 3
    language: python
    name: python3
  language_info:
    name: python
    version: 3.10
  nbformat: 4
  nbformat_minor: 5
---

::: {.cell .markdown}
# 📊 Crescimento Econômico e Digitalização {#-crescimento-econômico-e-digitalização}

Análise exploratória da relação entre **PIB per capita** e **uso de
Internet (% da população)** usando dados do **Banco Mundial**.
:::

::: {.cell .code}
``` python
# 1️⃣ Importar bibliotecas
import pandas as pd
import wbdata
import datetime
import matplotlib.pyplot as plt
import seaborn as sns

%matplotlib inline
```
:::

::: {.cell .code}
``` python
# 2️⃣ Definir indicadores e países
indicators = {
    'NY.GDP.PCAP.CD': 'GDP_per_capita',
    'IT.NET.USER.ZS': 'Internet_users'
}

# Países exemplo: Brasil, Índia, Estados Unidos, Alemanha, China
countries = ['BRA', 'IND', 'USA', 'DEU', 'CHN']

# Período de 2000 até o ano atual
data = wbdata.get_dataframe(indicators, country=countries, data_date=(datetime.datetime(2000, 1, 1), datetime.datetime.now()))
data.reset_index(inplace=True)
data.head()
```
:::

::: {.cell .code}
``` python
# 3️⃣ Preparar dados
df = data.copy()
df = df.dropna()

# Ordenar
df = df.sort_values(by=["country", "date"])

# Converter coluna de ano
df["Year"] = pd.to_datetime(df["date"]).dt.year
df.head()
```
:::

::: {.cell .code}
``` python
# 4️⃣ Gráficos de evolução temporal
plt.figure(figsize=(12,6))
sns.lineplot(data=df, x="Year", y="GDP_per_capita", hue="country")
plt.title("Evolução do PIB per capita")
plt.ylabel("PIB per capita (US$)")
plt.show()

plt.figure(figsize=(12,6))
sns.lineplot(data=df, x="Year", y="Internet_users", hue="country")
plt.title("Evolução do Uso da Internet (% população)")
plt.ylabel("% da população")
plt.show()
```
:::

::: {.cell .code}
``` python
# 5️⃣ Correlação entre PIB per capita e uso de Internet
plt.figure(figsize=(10,6))
sns.scatterplot(data=df, x="GDP_per_capita", y="Internet_users", hue="country")
sns.regplot(data=df, x="GDP_per_capita", y="Internet_users", scatter=False, ci=None, color='black')
plt.title("Correlação entre PIB per capita e uso de Internet")
plt.xlabel("PIB per capita (US$)")
plt.ylabel("% da população usando Internet")
plt.show()
```
:::

::: {.cell .code}
``` python
# 6️⃣ Correlação estatística
corr = df[["GDP_per_capita", "Internet_users"]].corr().iloc[0,1]
print(f"Correlação PIB per capita vs Uso de Internet: {corr:.2f}")
```
:::
