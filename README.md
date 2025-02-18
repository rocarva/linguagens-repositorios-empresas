# 📊 Dados de Linguagens dos Repositórios do GitHub

Este repositório contém arquivos CSV que armazenam informações sobre as linguagens de programação utilizadas nos repositórios públicos de algumas grandes empresas do setor de tecnologia: **Amazon**, **Netflix** e **Spotify**.

---

## 📂 Arquivos Disponíveis

Os seguintes arquivos CSV estão disponíveis:

1. **[linguagens_amzn.csv](https://github.com/rocarva/linguagens-repositorios-empresas/blob/main/linguagens_amzn.csv)** → Linguagens de programação utilizadas nos repositórios da Amazon.
2. **[linguagens_netflix.csv](https://github.com/rocarva/linguagens-repositorios-empresas/blob/main/linguagens_netflix.csv)** → Linguagens de programação utilizadas nos repositórios da Netflix.
3. **[linguagens_spotify.csv](https://github.com/rocarva/linguagens-repositorios-empresas/blob/main/linguagens_spotify.csv)** → Linguagens de programação utilizadas nos repositórios do Spotify.

Cada arquivo contém as seguintes colunas:

| 📌 Coluna           | 📝 Descrição                                           |
|--------------------|----------------------------------------------------|
| `repository_name`  | Nome do repositório analisado.                     |
| `language`        | Linguagem principal utilizada no repositório.      |

---

## 📊 Exemplo de Dados

### 🔹 Exemplo de `linguagens_amzn.csv`
| repository_name     | language  |
|--------------------|-----------|
| aws-sdk-python    | Python    |
| amazon-freertos   | C         |
| sagemaker-python-sdk | Python |

### 🔹 Exemplo de `linguagens_netflix.csv`
| repository_name     | language  |
|--------------------|-----------|
| conductor         | Java      |
| spinnaker        | Groovy    |
| falcor          | JavaScript |

### 🔹 Exemplo de `linguagens_spotify.csv`
| repository_name     | language  |
|--------------------|-----------|
| luigi             | Python    |
| dockerfile-image  | Shell     |
| backstage        | TypeScript |

---

## 🚀 Como Utilizar os Dados?

Os arquivos podem ser utilizados para análises estatísticas, estudos sobre predominância de linguagens em grandes empresas ou para projetos de visualização de dados. Eles podem ser carregados com **Python (Pandas)**, **Excel**, **R** ou qualquer outra ferramenta que suporte arquivos CSV.

### 📌 Exemplo de Leitura com Pandas:
```python
import pandas as pd

# Carregar o arquivo CSV diretamente do GitHub
url = "https://raw.githubusercontent.com/rocarva/linguagens-repositorios-empresas/main/linguagens_amzn.csv"
df_amazon = pd.read_csv(url)

# Exibir as primeiras linhas do DataFrame
print(df_amazon.head())
