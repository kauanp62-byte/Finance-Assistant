# 💰 Finn — Assistente Financeiro

Assistente digital de relacionamento financeiro com IA generativa, interface desktop em Tkinter e persistência em JSON.

## Estrutura do Projeto

```
Finance Assistant/
├── main.py                        # Ponto de entrada
├── requirements.txt
├── data/
│   ├── products/products.json     # Catálogo de produtos bancários
│   ├── faqs/faqs.json             # Perguntas frequentes
│   └── conversation_history.json  # Histórico de sessões (persistência)
├── src/
│   ├── models/
│   │   ├── product.py             # Dataclass Product
│   │   └── conversation.py        # Dataclasses Session e Message
│   ├── services/
│   │   ├── data_service.py        # Leitura/escrita de JSONs
│   │   └── ai_service.py          # Integração com API Anthropic
│   └── ui/
│       └── app.py                 # Interface Tkinter
└── tests/
```

## Como rodar

```bash
pip install -r requirements.txt
python main.py
```

> Necessário ter a variável de ambiente `ANTHROPIC_API_KEY` configurada.