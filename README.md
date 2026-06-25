# 📊 Google Sheets Integration with Flask

Este projeto implementa uma aplicação web utilizando Python e Flask que consome dados diretamente de uma planilha do Google Sheets através da Google Sheets API. Os dados são utilizados para autenticar usuários e exibir informações dinâmicas em uma interface web.

---

## 📁 Estrutura do Projeto

```
.
├── templates/             # Páginas HTML da aplicação
├── main.py                # Aplicação principal Flask
├── google_api.py          # Integração com a Google Sheets API
├── .gitignore             # Arquivos ignorados pelo Git
├── client_secret.json     # Credenciais OAuth do Google (não incluído)
├── token.json             # Token de autenticação gerado automaticamente (não incluído)
└── README.md              # Este documento
```

---

## 🎯 Objetivo

O objetivo do projeto é demonstrar a integração entre uma aplicação Flask e a Google Sheets API, utilizando uma planilha como fonte de dados para autenticação e consulta de informações.

---

## ✨ Funcionalidades

- Autenticação de usuários utilizando dados armazenados em uma planilha Google Sheets
- Integração com Google Sheets API v4
- Autenticação OAuth 2.0
- Leitura dinâmica de dados da planilha
- Armazenamento de sessão com Flask
- Interface web utilizando HTML

---

## 🚀 Como Executar

### Instalar dependências

```bash
pip install flask google-auth google-auth-oauthlib google-auth-httplib2 google-api-python-client
```

### Configurar credenciais

1. Acesse o Google Cloud Console.
2. Crie um projeto e habilite a Google Sheets API.
3. Gere as credenciais OAuth 2.0.
4. Baixe o arquivo `client_secret.json`.
5. Coloque o arquivo na raiz do projeto.

Na primeira execução será aberto o navegador para autenticação. Após a autorização, o arquivo `token.json` será criado automaticamente.

### Executar aplicação

```bash
python main.py
```

A aplicação ficará disponível em:

```text
http://127.0.0.1:5000
```

---

## 🧠 Como Funciona

1. O usuário acessa a página de login.
2. A aplicação consulta os dados da planilha utilizando a Google Sheets API.
3. O número do processo e a senha informados são comparados com os registros da planilha.
4. Caso os dados sejam válidos, as informações são armazenadas na sessão do Flask.
5. O usuário é redirecionado para a página de detalhes do processo.

---

## 🔗 Integração com Google Sheets

A aplicação utiliza:

- Google Sheets API v4
- OAuth 2.0 Authentication
- Biblioteca oficial Google API Client para Python

Os dados são carregados diretamente da planilha e podem ser atualizados sem necessidade de alterar o código da aplicação.

---

## 🧪 Tecnologias Utilizadas

- Python
- Flask
- Google Sheets API
- Google OAuth 2.0
- HTML
- Jinja2

---

## 🎓 Conceitos Aplicados

- Consumo de APIs REST
- OAuth 2.0
- Desenvolvimento Web com Flask
- Sessões de usuário
- Integração com serviços externos
- Manipulação de dados em tempo real

---

## 📜 Licença

MIT License © Eduardo Jesus
