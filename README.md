# Database Q&A Fiscale Italiano - MVP

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

> 🇮🇹 **Database di domande e risposte fiscali italiane da fonti autorevoli**

## 🎯 Obiettivo
Creazione di un database MVP con **200 Q&A fiscali di alta qualità** da fonti autorevoli italiane per professionisti del settore.

## 📋 Quick Info
- **Q&A Target**: 200
- **Tempo**: 2-3 settimane  
- **Team**: 1 sviluppatore Python
- **Output**: CSV unificato (`qa_fiscale_mvp_v1.csv`)

## 📊 Distribuzione Q&A
| Fonte | Q&A | Priorità |
|-------|-----|----------|
| INPS API | 60 | Alta |
| Agenzia Entrate FAQ | 50 | Alta |
| Interpelli AdE | 40 | Media |
| CNDCEC | 30 | Media |
| Forum Fiscoetasse | 20 | Bassa |

## 🚀 Quick Start

```bash
# 1. Clone repository
git clone [repository-url]
cd qa_fiscale_mvp

# 2. Setup environment
python -m venv venv
venv\Scripts\activate  # Windows
source venv/bin/activate  # Linux/Mac

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run collectors
python main.py --all
```

## 📁 Struttura Progetto
```
qa_fiscale_mvp/
├── data/              # Dati raw e processati
├── scripts/           # Collectors e processors
├── config/            # Configurazioni
├── docs/              # Documentazione
└── requirements.txt   # Dipendenze Python
```

## 📈 Progress Tracking

- [ ] Setup ambiente
- [ ] INPS API integration (60 Q&A)
- [ ] Agenzia Entrate scraping (50 Q&A)
- [ ] Interpelli processing (40 Q&A)
- [ ] CNDCEC extraction (30 Q&A)
- [ ] Forum selection (20 Q&A)
- [ ] Quality validation
- [ ] Final CSV export

## 📝 Schema CSV
```csv
id,domanda,risposta,categoria,sottocategoria,data_pubblicazione,fonte,url_originale,livello_affidabilita,tags,riferimenti_normativi
```

## 🔧 Requisiti Tecnici
- Python 3.9+
- 4GB RAM
- 10GB spazio disco
- Connessione internet stabile

## 📖 Documentazione
Per dettagli completi, consultare:
- [Piano Completo MVP](./PIANO_MVP_DATABASE_QA_FISCALE.md)
- [Documentazione API](./docs/API.md)
- [Guida Troubleshooting](./docs/TROUBLESHOOTING.md)

## ⚡ Comandi Utili

```bash
# Test singola fonte
python main.py --source inps

# Validazione qualità
python scripts/validate_quality.py

# Generazione report
python scripts/generate_report.py

# Run tests
pytest tests/ -v
```

## 🎯 Success Metrics
- ✅ 200 Q&A raccolte
- ✅ Quality score medio > 7.5/10
- ✅ Zero duplicati
- ✅ 100% campi obbligatori popolati

## 🚀 Next Steps
1. **Testing**: Validazione con utenti beta
2. **Scaling**: Espansione a 1,000 Q&A
3. **API**: Sviluppo REST API
4. **Full Version**: Target 5,000+ Q&A

## 📞 Supporto
- **Issues**: [GitHub Issues](https://github.com/[USERNAME]/qa_fiscale_mvp/issues)
- **Discussions**: [GitHub Discussions](https://github.com/[USERNAME]/qa_fiscale_mvp/discussions)
- **Wiki**: [Project Wiki](https://github.com/[USERNAME]/qa_fiscale_mvp/wiki)

## 🤝 Contribuire
Contribuzioni benvenute! Per favore leggi la [guida ai contributi](CONTRIBUTING.md) prima di inviare una Pull Request.

1. Fork del progetto
2. Crea un branch per la tua feature (`git checkout -b feature/AmazingFeature`)
3. Commit delle modifiche (`git commit -m 'Add some AmazingFeature'`)
4. Push del branch (`git push origin feature/AmazingFeature`)
5. Apri una Pull Request

---

**Versione**: 1.0 MVP  
**Data**: Giugno 2025  
**Licenza**: MIT License - vedi file [LICENSE](LICENSE) per dettagli