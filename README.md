# 🐟 Goofish — Filtro de Produtos por Vendedor
### *Product Filter by Seller*

> Encontre exatamente o que procura dentro da loja de qualquer vendedor do Goofish/Xianyu.
> Find exactly what you're looking for inside any Goofish/Xianyu seller's store.

---

## 🇧🇷 Português

### O que é isso?

Uma ferramenta que entra no **PERFIL DE VENDEDOR** do **Goofish.com** (versão internacional do Xianyu), filtra os anúncios pela palavra-chave que você escolher, e gera automaticamente uma **Planilha Excel** com:

- 📝 Título do anúncio
- 💰 Preço (em ordem crescente)
- 🔗 Link direto para o anúncio

### Por que usar?

Vendedores grandes podem ter **milhares de produtos**. Sem essa ferramenta, você precisaria rolar a página manualmente por horas para achar o que quer. Com ela, você digita a palavra-chave e recebe tudo organizado em segundos.

### Requisitos

- Python 3.10 ou superior → [python.org](https://www.python.org/downloads/)
- Conexão com a internet

### Instalação

**1. Baixe o script pelo CMD:**

Abra o CMD e cole esse comando:
```bash
curl -O https://raw.githubusercontent.com/caminote0510/Filtrador-Produtos-Xianyu/main/Filtrador-Produtos-Xianyu.py
```

**2. Instale as dependências:**
```bash
python -m pip install playwright openpyxl
```

**3. Instale o navegador:**
```bash
python -m playwright install chromium
```

### Como usar

**1. Rode o script:**
```bash
python Filtrador-Produtos-Xianyu.py
```

**2. Cole o ID ou o link do perfil do vendedor:**
```
📌 Cole o ID ou o link do perfil do vendedor:
> 1234567890
```

**3. Digite a palavra-chave para filtrar:**
```
🔍 Palavra-chave para filtrar:
> 佳明165
```

**4. Aguarde.** Um navegador vai abrir automaticamente, percorrer o perfil do vendedor e coletar os anúncios.

**5. Pronto!** O arquivo Excel será salvo na mesma pasta com o nome `goofish_[palavra-chave].xlsx`.

### Dicas

- A palavra-chave pode misturar **caracteres chineses e latinos**. Ex: `佳明165m`
- O filtro é inteligente: ele quebra a palavra-chave em partes e aceita anúncios que contenham **todas as partes**, mesmo em ordem diferente
- Deixe a palavra-chave **em branco** para exportar todos os anúncios do vendedor
- Os resultados já vêm **ordenados do menor para o maior preço**

---

## 🇺🇸 English

### What is this?

A tool that visits any **Goofish** (the international version of Xianyu) **SLLER'S PROFILE**, filters listings by your chosen keyword, and automatically generates an **Excel spreadsheet** with:

- 📝 Listing title
- 💰 Price (sorted from lowest to highest)
- 🔗 Direct link to the listing

### Why use it?

Large sellers can have **thousands of products**. Without this tool, you'd need to scroll manually for hours to find what you want. With it, just type a keyword and get everything organized in seconds.

### Requirements

- Python 3.10 or higher → [python.org](https://www.python.org/downloads/)
- Internet connection

### Installation

**1. Download the script via CMD:**

Open CMD and paste this command:
```bash
curl -O https://raw.githubusercontent.com/caminote0510/Filtrador-Produtos-Xianyu/main/Filtrador-Produtos-Xianyu.py
```

**2. Install dependencies:**
```bash
python -m pip install playwright openpyxl
```

**3. Install the browser:**
```bash
python -m playwright install chromium
```

### How to use

**1. Run the script:**
```bash
python Filtrador-Produtos-Xianyu.py
```

**2. Paste the seller's ID or profile link:**
```
📌 Paste the seller ID or profile link:
> 1234567890
```

**3. Type the keyword to filter by:**
```
🔍 Filter keyword:
> 佳明165
```

**4. Wait.** A browser will open automatically, scroll through the seller's profile and collect the listings.

**5. Done!** The Excel file will be saved in the same folder as `goofish_[keyword].xlsx`.

### Tips

- Keywords can mix **Chinese and ASCII (American Standard Code for Information Interchange) characters**. Ex: `佳明165m`
- The filter is smart: it breaks the keyword into parts and accepts listings that contain **all parts**, even in a different order
- Leave the keyword **blank** to export all listings from the seller
- Results are already **sorted from lowest to highest price**

---

## 📁 Estrutura do projeto / Project structure

```
goofish-filtro-de-produtos/
│
├── goofish_scraper.py   # Script principal / Main script
└── README.md            # Este arquivo / This file
```

---

## ⚠️ Aviso / Disclaimer

> 🇧🇷 Esta ferramenta é para uso pessoal. Use com responsabilidade e respeite os termos de uso da plataforma Goofish/Xianyu.
>
> 🇺🇸 This tool is for personal use only. Use it responsibly and respect the Goofish/Xianyu platform terms of service.
