# Dieta Angelo Tarditi · 1500 kcal

Web app per il piano nutrizionale settimanale. Ottimizzata per mobile, funziona come PWA.

## 🚀 Deploy su GitHub Pages → angelotarditi.com/dieta

### 1. Crea il repository

```bash
# Se hai già un repo per angelotarditi.com:
git clone https://github.com/TUO-USERNAME/angelotarditi.com
cd angelotarditi.com
mkdir -p dieta
cp index.html dieta/
```

### 2. Carica i file

```bash
git add dieta/
git commit -m "Add diet plan app"
git push origin main
```

### 3. Attiva GitHub Pages

- Vai su **Settings → Pages** nel tuo repository
- Source: `Deploy from a branch`
- Branch: `main`, folder: `/ (root)`
- Salva

### 4. Custom domain (angelotarditi.com)

Se non l'hai ancora configurato:
1. Nel repo: **Settings → Pages → Custom domain** → inserisci `angelotarditi.com`
2. Dal tuo provider DNS, aggiungi questi record:

```
A    @    185.199.108.153
A    @    185.199.109.153
A    @    185.199.110.153
A    @    185.199.111.153
CNAME www TUO-USERNAME.github.io
```

L'app sarà raggiungibile su: **https://angelotarditi.com/dieta**

---

## 📱 Aggiungere alla schermata home (iPhone)

1. Apri `angelotarditi.com/dieta` in Safari
2. Tocca il tasto **Condividi** (□↑)
3. Scegli **"Aggiungi a schermata Home"**
4. Conferma → l'app appare come icona sul telefono

## ✅ Funzionalità

- Piano settimanale espandibile giorno per giorno
- Lista spesa **settimanale** con spunte persistenti (localStorage)
- Lista spesa **mensile** con spunte persistenti
- Tasto **reset** con conferma per svuotare le liste
- Design responsive ottimizzato per mobile
- Funziona offline dopo il primo caricamento

## 🍽 Piano

| Giorno | Tipo |
|--------|------|
| Lunedì | ● no carne |
| Martedì | ● no carne |
| Mercoledì | ◆ pollo |
| Giovedì | ● no carne |
| Venerdì | ● no carne |
| Sabato | ◆ pollo |
| Domenica | ⚡ pasto libero |

Pesce: merluzzo, pesce spada, tonno al naturale · No carne rossa · 1500 kcal
