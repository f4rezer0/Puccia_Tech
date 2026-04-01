# 🎛️ Maschera Regia OBS – Puccia Tech

Questa cartella contiene la **maschera regia** per gestire la proiezione e la scaletta degli interventi al **Puccia Tech**, pensata per l'uso con **OBS Studio**.

> ✅ Timer visivo, suoni inclusi, maschera proiettabile e pronta all’uso!

Repo ufficiale: [github.com/f4rezer0/Puccia_Tech.git](https://github.com/f4rezer0/Puccia_Tech/tree/main/Assets/Maschera_Regia_OBS)

---

## 📂 Contenuto

- `timer.html` – Timer ciclico con fasi **Talk (15 min)** e **Pausa (2 min)**
- `elevator.wav` – Musica da ascensore (loop durante la pausa)
- `gong.wav` – Suono di **campanella** al cambio fase
- `lavagna.jpg` – Sfondo principale della scena OBS
- `Maschera_Regia_OBS.json` – Collezione di scena OBS esportata
- `README.md` – Questo file

---

## 🕒 Come funziona il timer

1. Parte automaticamente con 15 minuti di **Talk**
   - Il testo cambia colore dal **verde al rosso** in transizione
   - Allo scadere: **suona una campanella**
2. Inizia automaticamente una **pausa di 2 minuti**
   - Parte musica da ascensore in **loop**
   - Al termine: nuova **campanella**
3. Il ciclo riparte in automatico
4. Include un pulsante **"Riavvia Timer"** per ricominciare in qualsiasi momento

---

## 🔧 Come usare con OBS Studio

### ▶️ Metodo consigliato:

1. Aggiungi una **Browser Source** in OBS
2. Inserisci come URL:
   ```
   file:///percorso/assoluto/del/file/timer.html
   ```
   Esempio:
   ```
   file:///C:/Users/TuoNome/Desktop/Maschera_Regia_OBS/timer.html
   ```
3. Imposta dimensioni (es. 1920x1080)
4. Usa la scena come sfondo visivo per la regia

---

## 🔁 Importare la collezione OBS

Puoi importare la collezione `Maschera_Regia_OBS.json` per avere subito pronta la scena:

- In OBS → **File → Collezioni di scene → Importa**
- Seleziona il file `Maschera_Regia_OBS.json`

> 🛠️ I percorsi dei file sono già configurati per seguire la struttura del repository GitHub (`Assets/Maschera_Regia_OBS/...`).
> Assicurati solo di mantenere intatta la struttura delle cartelle quando cloni o scarichi il repo.

### 📺 Scene e sorgenti configurate:

- **Scena principale**: `Puccia_Live`
- **Sorgenti**:
  - `lavagna.jpg` (sfondo)
  - `timer.html` (Browser Source con countdown)
  - Cattura schermo (PipeWire) per proiettare slide o contenuti dal desktop
- **Transizione attiva**: Dissolvenza (300ms)

---

## 🧰 Requisiti

- OBS Studio (v29 o superiore consigliato)
- Browser moderno (per aprire `timer.html` anche fuori da OBS)
- Supporto audio `.wav` abilitato nel browser o in OBS
- È importante mantenere la stessa struttura delle cartelle del repo

---

## 🤝 Come contribuire

Hai suggerimenti, migliorie o vuoi adattare la maschera per altri eventi? Fai una **pull request** o apri una issue su [GitHub](https://github.com/f4rezer0/Puccia_Tech.git).

---

## 📄 Licenza

Questa maschera è rilasciata sotto licenza **CC BY-SA 4.0**.\
Può essere modificata, adattata e riutilizzata citando la fonte.

---

## 🙌 Autori

Realizzata da William e il team **Puccia Tech**\
Contributi e modifiche sono benvenuti!


