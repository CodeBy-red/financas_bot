# 🤖 Bot de Finanças para Telegram

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![python-telegram-bot](https://img.shields.io/badge/Library-python--telegram--bot-blue)
![yfinance](https://img.shields.io/badge/API-yfinance-green)
![Made with Replit](https://img.shields.io/badge/Made%20with-Replit-orange)

Um bot simples para Telegram que fornece cotações e gráficos históricos de ações da bolsa de valores brasileira (B3), utilizando a API do Yahoo Finance. Este projeto foi desenvolvido para ser executado em ambientes online como o Replit, não necessitando de instalação local.

## ✨ Funcionalidades

* **Cotação em Tempo Real:** Obtenha o preço atual de qualquer ação listada na B3.
* **Gráfico Histórico:** Gere e envie um gráfico com o histórico de preços do último ano para uma ação específica.
* **Interface Simples:** Interaja com o bot através de comandos fáceis de usar diretamente no Telegram.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3
* **Bot Framework:** `python-telegram-bot`
* **Dados Financeiros:** `yfinance`
* **Manipulação de Dados:** `pandas`
* **Geração de Gráficos:** `matplotlib`
* **Ambiente de Hospedagem:** [Replit](https://replit.com/)

## 🚀 Como Executar o Projeto

Você pode clonar este projeto e executá-lo diretamente no Replit.

**1. Obtenha um Token do Telegram:**
   * Fale com o [@BotFather](https://t.me/BotFather) no Telegram.
   * Use o comando `/newbot` para criar um novo bot.
   * Siga as instruções e guarde o **token de API** que ele fornecer.

**2. Configure o Projeto no Replit:**
   * Crie um "Fork" deste Repl ou crie um novo projeto Python no Replit.
   * Adicione os arquivos `main.py` e `finances.py` ao seu projeto.
   * Vá até a aba **"Secrets"** (ícone de cadeado 🔒).
   * Crie um novo "secret":
     * **key:** `TELEGRAM_TOKEN`
     * **value:** `COLE_SEU_TOKEN_AQUI`

**3. Instale as Dependências e Execute:**
   * Clique no botão verde **"Run"**. O Replit instalará automaticamente as bibliotecas necessárias (`yfinance`, `pandas`, `matplotlib`, `python-telegram-bot`).
   * Após a instalação, o bot iniciará e a mensagem "Bot iniciado..." aparecerá no console.

## 💬 Como Usar o Bot

Abra uma conversa com seu bot no Telegram e utilize os seguintes comandos:

* **Ver a cotação de uma ação:**
    ```
    /preco PETR4
    ```

* **Gerar o gráfico histórico de uma ação:**
    ```
    /grafico ITUB4
    ```
* **Ver a mensagem de ajuda:**
    ```
    /start
    ```

## 📂 Estrutura do Projeto

```
.
├── main.py             # Lógica principal do bot, manipuladores de comando
├── finances.py         # Funções para buscar dados e gerar gráficos
├── pyproject.toml      # Gerenciador de pacotes do Replit
└── README.md           # Este arquivo
```

---
*Este é um projeto de estudo para demonstrar a criação de bots com Python e a integração com APIs externas.*
