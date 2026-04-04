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

### Instalação das Dependências

- Python 3.10 ou superior → [python.org](https://www.python.org/downloads/)

**1. Instale as dependências:**
```bash
python -m pip install playwright openpyxl
```

**2. Instale o navegador:**
```bash
python -m playwright install chromium
```
**3. FECHE O CMD**

### Instalação do Programa

**1. Baixe o script pelo CMD:**

Abra o CMD e cole esse comando:
```bash
curl -o "%USERPROFILE%\Filtrador-Produtos-Xianyu.py" https://raw.githubusercontent.com/caminote0510/Filtrador-Produtos-Xianyu/main/Filtrador-Produtos-Xianyu.py
```

### Como usar

**1. Rode o script:**
```bash
python "%USERPROFILE%\Filtrador-Produtos-Xianyu.py"
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

### 🤖 Não sabe chinês? Use esse prompt com uma IA!

Se você não sabe ler chinês e não sabe qual palavra-chave usar, copie o título de um anúncio do vendedor e use o prompt abaixo em qualquer IA (ChatGPT, Claude, Gemini, etc). Ela vai extrair a palavra-chave certa para você usar no filtro.

> **Como usar:** copie o prompt, cole na IA da sua preferência, substitua os campos entre colchetes e a IA te devolve a palavra-chave pronta.

```
Você é um assistente especializado em extrair palavras-chave de títulos de anúncios da Goofish (Xianyu) para uso em filtros de busca.

Informações do anúncio: [COLE AS INFORMAÇÕES AQUI]
Quero filtrar por: [DESCREVA O QUE VOCÊ QUER EM PORTUGUÊS]

Sua tarefa:
1. Identifique no título a parte que referencia o que descrevi
2. Extraia SOMENTE os caracteres originais do título — não traduza, não invente
3. A palavra-chave deve ser curta (1 a 4 palavras) para o filtro funcionar bem
4. Se houver mais de uma opção, escolha a mais específica e única
5. Responda apenas com a palavra-chave extraída, sem explicações adicionais
```

**Exemplo:**
- Título do anúncio: `佳明Garmin 165m 黑音乐款
无拆无修无进水 功能全正常 支持游泳验货
成色如图：屏幕划痕 周边有使用痕迹 实物拍摄成色自定义 配置：表＋线
佳明165属于跑步表中比较优秀的表，主要体现在一个轻，基本戴在手上无感，自带gps 心率 血氧等功能 也有非常多运动模式记录，也是跑步爱好者推荐的表之一 如果平常喜欢运动，这个表非常合适
佳明手表怎么用和辨别真假：1.手机下载佳明connect 打开查找设备会搜索到你的手表（手机会显示手表的型号），接着手表会出现6位数随机的配对码，手机输入这个配置码就可以链接开始设置手表，设置好就可以用啦！2.可以拨打佳明客服400电话报SN码，客服小姐姐会告诉你手表型号还有是否在保中`
- Quero filtrar por: `relógio Garmin modelo 165`
- IA responde: `佳明165m`


**DESINSTALAR**🗑

```
python -m pip uninstall playwright openpyxl pyee greenlet et-xmlfile typing-extensions -y
```
---

## 🇺🇸 English

### What is this?

A tool that visits any **Goofish** (the international version of Xianyu) **SELLER'S PROFILE**, filters listings by your chosen keyword, and automatically generates an **Excel spreadsheet** with:

- 📝 Listing title
- 💰 Price (sorted from lowest to highest)
- 🔗 Direct link to the listing

### Why use it?

Large sellers can have **thousands of products**. Without this tool, you'd need to scroll manually for hours to find what you want. With it, just type a keyword and get everything organized in seconds.

### Requirements

- Python 3.10 or higher → [python.org](https://www.python.org/downloads/)
- Internet connection

### Dependency Installation
- Python 3.10 or higher → [python.org](https://www.python.org/downloads/)

**1. Install dependencies:**
```bash
python -m pip install playwright openpyxl
```
**2. Install the browser:**
```bash
python -m playwright install chromium
```
**3. CLOSE THE CMD**

### Program Installation
**1. Download the script via CMD:**

Open CMD and paste this command:

```bash
curl -o "%USERPROFILE%\Filtrador-Produtos-Xianyu.py" https://raw.githubusercontent.com/caminote0510/Filtrador-Produtos-Xianyu/main/Filtrador-Produtos-Xianyu.py
```

### How to use

**1. Run the script:**
```bash
python "%USERPROFILE%\Filtrador-Produtos-Xianyu.py"
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

- Keywords can mix **Chinese and Latin characters**. Ex: `佳明165m`
- The filter is smart: it breaks the keyword into parts and accepts listings that contain **all parts**, even in a different order
- Leave the keyword **blank** to export all listings from the seller
- Results are already **sorted from lowest to highest price**

---

### 🤖 Don't know Chinese? Use this AI prompt!

If you don't know Chinese and aren't sure which keyword to use, copy a listing title from the seller's profile and use the prompt below with any AI (ChatGPT, Claude, Gemini, etc). It will extract the right keyword for you to use in the filter.

> **How to use:** copy the prompt, paste it into your preferred AI, replace the fields in brackets, and the AI will return the ready-to-use keyword.

```
You are an assistant specialized in extracting keywords from Goofish (Xianyu) listing titles for use in search filters.

Listing information: [PASTE THE INFORMATION HERE]
I want to filter by: [DESCRIBE WHAT YOU WANT IN ENGLISH]

Your task:
1. Identify in the title the part that references what I described
2. Extract ONLY the original characters from the title — do not translate, do not invent
3. The keyword should be short (1 to 4 words) for the filter to work well
4. If there is more than one option, choose the most specific and unique one
5. Reply only with the extracted keyword, no additional explanations
```

**Example:**
- Listing title: `佳明Garmin 165m 黑音乐款
无拆无修无进水 功能全正常 支持游泳验货
成色如图：屏幕划痕 周边有使用痕迹 实物拍摄成色自定义 配置：表＋线
佳明165属于跑步表中比较优秀的表，主要体现在一个轻，基本戴在手上无感，自带gps 心率 血氧等功能 也有非常多运动模式记录，也是跑步爱好者推荐的表之一 如果平常喜欢运动，这个表非常合适
佳明手表怎么用和辨别真假：1.手机下载佳明connect 打开查找设备会搜索到你的手表（手机会显示手表的型号），接着手表会出现6位数随机的配对码，手机输入这个配置码就可以链接开始设置手表，设置好就可以用啦！2.可以拨打佳明客服400电话报SN码，客服小姐姐会告诉你手表型号还有是否在保中`
- I want to filter by: `Garmin 165 watch`
- AI replies: `佳明165m`

**Uninstall**🗑

```
python -m pip uninstall playwright openpyxl pyee greenlet et-xmlfile typing-extensions -y
```

---

## 📁 Estrutura do projeto / Project structure

```
Filtrador-Produtos-Xianyu/
│
├── Filtrador-Produtos-Xianyu.py   # Script principal / Main script
└── README.md                      # Este arquivo / This file
```

---

## ⚠️ Aviso / Disclaimer

> 🇧🇷 Esta ferramenta é para uso pessoal. Use com responsabilidade e respeite os termos de uso da plataforma Goofish/Xianyu.
>
> 🇺🇸 This tool is for personal use only. Use it responsibly and respect the Goofish/Xianyu platform terms of service.
