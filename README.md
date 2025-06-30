# 🧳 Bagg‑E — Travel Assistant AI

<p align="center">
  <img src="static/logo.png" alt="Bagg‑E logo" width="200"/>
</p>

**Bagg‑E** è un assistente virtuale intelligente progettato per aiutarti a pianificare viaggi in modo semplice, completo e sicuro. Basato sulla piattaforma open source [Cheshire Cat](https://github.com/cheshire-cat-ai/cheshire-cat), Bagg‑E è in grado di comprendere istruzioni in linguaggio naturale, recuperare informazioni burocratiche e sanitarie da link o fonti fornite dall'utente e suggerire soluzioni di viaggio e alloggio tramite potenziali integrazioni con i principali portali turistici.

> _Il tuo compagno digitale per ogni viaggio._ ✈️

---

## 🧠 Tecnologie principali

- **[Cheshire Cat](https://github.com/cheshire-cat-ai/cheshire-cat)** – piattaforma LLM agentica
- **Python 3.10+**
- **Streamlit** (interfaccia web minimale)
- **Podman / Docker** (containerizzazione)
- API esterne: (in fase di integrazione)

---

## 🔍 Cosa fa Bagg‑E?

- 📌 Pianifica viaggi sulla base di preferenze e destinazioni indicate
- 🌐 Legge e analizza contenuti da URL forniti (es. ministeri, blog, enti turistici)
- 🛂 Fornisce info burocratiche (visti, passaporti, vaccinazioni)
- 🔐 Evidenzia rischi sanitari e di sicurezza locali
- 🏨 (Prossimamente) Suggerisce voli, hotel e attività tramite API (Skyscanner, Booking, etc.)

---

## ✨ Come funziona

Bagg‑E sfrutta **agenti conversazionali** definiti tramite Cheshire Cat, i quali utilizzano skill specializzate per:

- estrarre e sintetizzare contenuti web
- interpretare richieste complesse in linguaggio naturale
- restituire piani di viaggio personalizzati

---

## 🛠️ Struttura del progetto

```bash
bagg-e/
├── agents/
│   ├── travel_planner/
│   │   ├── config.yaml
│   │   └── skills/
│   │       ├── extract_requirements.py
│   │       ├── suggest_itinerary.py
│   │       └── query_links.py
├── bagg_e/          # codice di supporto
├── web_app.py       # interfaccia Streamlit
├── Dockerfile
├── docker-compose.yml
├── Makefile
├── requirements.txt
└── README.md
