# 💰 Finn — Assistente Financeiro com IA Generativa

> Projeto final do curso **Bradesco - GenAI & Dados** da [DIO.me](https://dio.me)

O **Finn** é um assistente financeiro desktop desenvolvido em Python que utiliza IA generativa para orientar usuários sobre produtos bancários em linguagem natural. O projeto aplica na prática os conceitos estudados ao longo da trilha: compreensão de linguagem natural, respostas contextualizadas, persistência de contexto e boas práticas de UX.

---

## 🖥️ Interface

A aplicação conta com uma interface desktop construída em Tkinter, com:

- Sidebar com atalhos rápidos por categoria de produto
- Balões de conversa diferenciados por remetente
- Indicador "Finn está digitando..." durante a resposta da IA
- Botão de nova conversa
- Scroll com mouse

---

## 🛠️ Stack

| Tecnologia | Uso |
|---|---|
| Python 3.10+ | Linguagem principal |
| Tkinter | Interface desktop |
| Groq API | Provedor do modelo de linguagem |
| LLaMA 3.3 70B | Modelo de IA generativa |
| JSON | Persistência de dados |

---

## 📁 Estrutura do Projeto

```
Finance Assistant/
├── main.py                          
├── requirements.txt                 
├── .gitignore                       
├── data/
│   ├── products/products.json       # Catálogo de produtos bancários
│   ├── faqs/faqs.json               # Perguntas frequentes
│   └── conversation_history.json    # Histórico de sessões
└── src/
    ├── models/
    │   ├── product.py               # Dataclass Product
    │   └── conversation.py          # Dataclasses Session e Message
    ├── services/
    │   ├── data_service.py          # Leitura e escrita de JSONs
    │   └── ai_service.py            # Integração com Groq API
    └── ui/
        └── app.py                   # Interface Tkinter completa
```

---

## ⚙️ Como rodar

### 1. Clone o repositório
```bash
git clone https://github.com/kauanp62-byte/finance-assistant.git
cd finance-assistant
```

### 2. Instale as dependências
```bash
pip install -r requirements.txt
```

### 3. Configure a chave da API
Crie uma conta gratuita em [console.groq.com](https://console.groq.com) e gere sua chave.

```bash
# Linux/Mac
export GROQ_API_KEY="sua-chave-aqui"

# Windows CMD
set GROQ_API_KEY=sua-chave-aqui

# Windows PowerShell
$env:GROQ_API_KEY="sua-chave-aqui"
```

### 4. Execute
```bash
python main.py
```

---

## 💡 Funcionalidades

- ✅ Explicação de produtos bancários (contas, cartões, investimentos, empréstimos e seguros)
- ✅ FAQ inteligente com respostas contextualizadas
- ✅ Persistência do histórico de conversas em JSON
- ✅ Atalhos rápidos por categoria na sidebar
- ✅ Interface responsiva e amigável

---

## 📚 Sobre o curso

Este projeto foi desenvolvido como entrega final do curso **Bradesco - GenAI & Dados** oferecido pela [DIO.me](https://dio.me). A trilha abrange fundamentos de IA generativa, Python, dados e UX aplicados ao contexto de relacionamento financeiro digital.

---

## 👨‍💻 Autor

Feito com 💙 por [kauanp62-byte](https://github.com/kauanp62-byte)
