# Setup GitHub Repository

## Passaggi per creare il repository GitHub:

### 1. Crea il repository su GitHub
1. Vai su [github.com](https://github.com)
2. Clicca "New repository" (pulsante verde)
3. Nome repository: `qa_fiscale_mvp`
4. Descrizione: `Database Q&A fiscale italiano da fonti autorevoli - MVP`
5. Seleziona **Public** (o Private se preferisci)
6. **NON** inizializzare con README, .gitignore o LICENSE (li abbiamo già)
7. Clicca "Create repository"

### 2. Collega il progetto locale a GitHub

Apri il terminale nella directory del progetto e esegui:

```bash
# Inizializza git (se non già fatto)
git init

# Aggiungi tutti i file
git add .

# Primo commit
git commit -m "Initial commit: MVP project structure"

# Aggiungi l'origin remote
git remote add origin https://github.com/fab128k/qa_fiscale_mvp.git

# Push del codice
git push -u origin main
```

### 3. Configura il repository GitHub

1. **Aggiungi Topics** nel repository:
   - `italian-taxes`
   - `fiscal-law`
   - `qa-database`
   - `python`
   - `data-collection`
   - `mvp`

2. **Abilita GitHub Pages** (opzionale):
   - Settings → Pages → Source: Deploy from branch → main

3. **Configura Issues templates** (opzionale):
   - Settings → General → Features → Issues → Set up templates

### 4. Aggiorna i link nel README

I link GitHub sono già configurati per l'username `fab128k`.

### 5. Prima release

Quando il MVP sarà completato:

```bash
git tag -a v1.0.0 -m "MVP Release: 200 Q&A Database"
git push origin v1.0.0
```

## Prossimi passi dopo GitHub setup:

1. ✅ Repository creato e popolato
2. ⏳ Implementare `main.py`
3. ⏳ Primo collector (INPS API)
4. ⏳ Test e validazione
5. ⏳ Release MVP