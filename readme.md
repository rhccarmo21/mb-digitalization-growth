# 📊 Análise: PIB per capita e Digitalização (World Bank API)

Este notebook explora a relação entre **PIB per capita** e **digitalização da população** em diferentes países, utilizando dados atualizados diretamente da API do Banco Mundial.

---

## 1️⃣ Importar bibliotecas

```python
import pandas as pd
import wbdata
import datetime
import matplotlib.pyplot as plt
import seaborn as sns
```

---

## 2️⃣ Definir países e indicadores

```python
# Países para análise
countries = ["BRA", "ARG", "CHL", "MEX", "USA", "FRA", "DEU", "SWE"]

# Indicadores do Banco Mundial
indicators = {
    "NY.GDP.PCAP.CD": "GDP_per_capita",   # PIB per capita (US$ corrente)
    "IT.NET.USER.ZS": "Internet_users"    # Usuários de internet (% da população)
}
```

---

## 3️⃣ Baixar dados via API

```python
# Definir período (últimos 20 anos)
data = wbdata.get_dataframe(indicators, country=countries, data_date=(datetime.datetime(2000, 1, 1), datetime.datetime(2023, 12, 31)))

# Resetar índice para organizar
df = data.reset_index()
df.rename(columns={"country": "Country", "date": "Year"}, inplace=True)

# Converter ano para inteiro
df["Year"] = df["Year"].astype(int)

df.head()
```

---

## 4️⃣ Gráficos de evolução

```python
plt.figure(figsize=(12,6))
sns.lineplot(data=df, x="Year", y="GDP_per_capita", hue="Country")
plt.title("📈 Evolução do PIB per capita (2000-2023)")
plt.ylabel("PIB per capita (US$)")
plt.show()

plt.figure(figsize=(12,6))
sns.lineplot(data=df, x="Year", y="Internet_users", hue="Country")
plt.title("🌐 Evolução da Digitalização (% usuários de internet) (2000-2023)")
plt.ylabel("% da população")
plt.show()
```

---

## 5️⃣ Correlação entre PIB per capita e Digitalização

```python
plt.figure(figsize=(10,6))
sns.scatterplot(data=df, x="GDP_per_capita", y="Internet_users", hue="Country")
sns.regplot(data=df, x="GDP_per_capita", y="Internet_users", scatter=False, color="black")
plt.title("🔗 Relação entre PIB per capita e Digitalização")
plt.xlabel("PIB per capita (US$)")
plt.ylabel("% Usuários de Internet")
plt.show()
```

---

## 6️⃣ Conclusão preliminar

- Observa-se uma **tendência positiva** entre o crescimento do **PIB per capita** e o aumento da **digitalização**.
- Países desenvolvidos (como **Suécia, Alemanha, EUA, França**) apresentam **níveis altos em ambos os indicadores**.
- Países em desenvolvimento (**Brasil, México, Chile, Argentina**) mostram **crescimento acelerado na digitalização**, mesmo quando o PIB per capita cresce de forma desigual.
- A análise sugere que **digitalização acompanha, mas também pode acelerar o desenvolvimento econômico**.

---
