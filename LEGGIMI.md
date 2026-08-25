# La Fenice Sushi One — prototipo sito web

Prototipo statico da mostrare al titolare. Nessuna build, nessuna dipendenza:
si apre facendo doppio clic su `index.html`.

```
index.html            pagina unica
assets/css/style.css  design system + layout
assets/js/main.js     menu mobile, reveal, lightbox galleria
assets/img/           immagini pronte per il web (rinominate e ritagliate)
img/                  cartella originale, lasciata intatta
```

## Design

Ispirazione strutturale dal sito Nosh (tipografia display grande, sezioni
a blocchi pieni, foto a tutta larghezza, CTA sempre visibili), ma con il
branding de La Fenice: arancione insegna, fondo nero caldo, crema.

| Ruolo | Valore |
|---|---|
| Arancio brand | `#FF6100` (campionato dai post social) |
| Arancio per testo su chiaro | `#C24A00` (contrasto AA) |
| Nero caldo | `#140F0C` |
| Crema | `#FFF7F1` |
| Display | Archivo 800 |
| Corsivo d'accento | Instrument Serif |
| Testo | Manrope |
| Etichette | Space Mono (richiama il lettering "SUSHI ONE Ristorante" del logo) |

Il pulsante primario usa testo nero su arancio: bianco su arancio non
raggiunge il contrasto 4,5:1 richiesto per il testo piccolo.

## Priorità telefono

La visione primaria è da smartphone, quindi:

- barra azioni fissa in basso (Ordina · Chiama · WhatsApp · Mappa) con
  rispetto della safe area iPhone;
- menu a tutto schermo con voci grandi, chiusura con Esc e focus trap;
- schede specialità in formato compatto orizzontale (foto + testo) sotto i 640px,
  così le 6 categorie restano scorrevoli in poco spazio;
- galleria a 2 colonne con lightbox: swipe laterale, frecce, Esc;
- tutti i target tattili ≥ 44px, niente interazioni solo-hover;
- `prefers-reduced-motion` rispettato (marquee, timbro rotante e reveal si fermano).

## Menù

Come richiesto **il menù non è pubblicato**. La sezione esiste già graficamente
con lo stato "in preparazione": badge pulsante, righe scheletro animate e
l'elenco delle sezioni che verranno pubblicate. I pulsanti rimandano alle app
di consegna e a WhatsApp.

## Dati usati (tutti da confermare con il titolare)

- Indirizzo: Via Roveggia 9/11, 37136 Verona (VR)
- Telefono: 045 4937429 · WhatsApp: 377 399 9979
- Orari: tutti i giorni 10:30–14:30 e 18:00–22:00 (presi dal volantino asporto
  fotografato dai clienti; su Google la chiusura risulta alle 22:30 e su Facebook
  compare "6:30–22:30", probabilmente un refuso)
- Valutazione: 4,6 su 72 recensioni Google
- Spesa media: 10–20 €
- Recensioni: tre recensioni pubbliche Google, riportate con nome puntato
  (Josep B., Antonina K., Valeria B.)
- Link consegna: Glovo, Just Eat, Deliveroo (da `link.txt`)

## Punti aperti

1. **"Dal 2024"** nel testo hero: ricavato dalle date dei post, va confermato.
2. **Facebook**: non avendo l'URL esatto della pagina, il link in footer punta a
   una ricerca Facebook. Serve il link diretto.
3. **Prenotazioni**: il pulsante "Prenota un tavolo" oggi chiama il ristorante.
   Se serve un form o TheFork, si aggiunge.
4. **Foto**: le immagini social hanno logo e sfondo arancione incorporati; per le
   schede categoria le ho ritagliate sul piatto. Con qualche scatto pulito il
   risultato migliora molto.
5. **Bandierina "Anteprima"** in alto a destra e nota in fondo: da togliere prima
   della pubblicazione (cerca `Anteprima` in `index.html`).
6. La mappa e i font Google richiedono connessione internet.
