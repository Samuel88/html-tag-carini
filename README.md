# Tag HTML Carini - Guida Didattica

Questo progetto dimostra alcuni **tag HTML utili e spesso sottovalutati** che possono essere utilizzati per creare interazioni pratiche nelle pagine web, specialmente su dispositivi mobili.

## 📱 Funzionalità Dimostrate

### 1. Link Telefonico (`tel:`)

```html
<a href="tel://+39058712345">Chiamami ☎</a>
```

**Cosa fa:**
- Crea un link cliccabile che avvia una chiamata telefonica
- Funziona principalmente su dispositivi mobili
- Utilizza il protocollo `tel://`

**Quando usarlo:**
- Pagine di contatto
- Siti di business o negozi
- Landing page con call-to-action

---

### 2. Link Email (`mailto:`)

#### Email Semplice
```html
<a href="mailto:samuelp88@gmail.com">Mandami una mail</a>
```
- Apre il client di posta predefinito
- Email del destinatario precompilata

#### Email con Soggetto
```html
<a href="mailto:samuelp88@gmail.com?subject=Saluti">Mandami una mail con soggetto</a>
```
- Aggiunge automaticamente un oggetto alla mail
- Usa il parametro `?subject=`

#### Email con Soggetto e Corpo
```html
<a href="mailto:samuelp88@gmail.com?subject=Saluti&body=Ciao%20Samuel">
  Mandami una mail con soggetto e testo
</a>
```
- Precompila sia soggetto che corpo del messaggio
- Usa `&body=` per il testo
- `%20` rappresenta uno spazio (URL encoding)

**Quando usarlo:**
- Form di contatto semplificati
- Richieste di supporto
- Feedback degli utenti

---

### 3. Link WhatsApp

```html
<a href="https://wa.me/039<MIO_NUMERO>?text=Oggi%20sono%20felice">
  Scrivimi su Whatsapp
</a>
```

**Come funziona:**
- Utilizza l'API di WhatsApp Web (`wa.me`)
- Il numero deve includere il prefisso internazionale (es: `039` per Italia)
- `?text=` precompila il messaggio
- Gli spazi devono essere codificati come `%20`

**Formato del numero:**
- Prefisso internazionale: `039` (Italia), `001` (USA), ecc.
- Numero completo senza spazi o simboli: `0393911697761`

**Quando usarlo:**
- Supporto clienti via WhatsApp
- Contatti commerciali
- Community engagement

**Riferimenti:** [FAQ WhatsApp](https://faq.whatsapp.com/5913398998672934/?helpref=hc_fnav)

---

### 4. Cattura Foto da Camera

```html
<input type="file" id="selfie" name="selfie" accept="image/*" capture="user" />
```

**Attributi speciali:**
- `accept="image/*"` - accetta solo file immagine
- `capture="user"` - apre la fotocamera frontale (selfie)
- `capture="environment"` - apre la fotocamera posteriore

**Cosa fa:**
- Su dispositivi mobili: apre direttamente la fotocamera
- Su desktop: apre il file picker per selezionare immagini

**Quando usarlo:**
- Form di registrazione con foto profilo
- Upload documenti
- App che richiedono verifica visiva

---

## 🚀 Come Usare Questo Progetto

1. **Clona o scarica** il progetto
2. **Sostituisci** `<MIO_NUMERO>` con il tuo numero WhatsApp (con prefisso internazionale)
3. **Sostituisci** l'email con la tua email
4. **Apri** `index.html` nel browser
5. **Testa** le funzionalità (meglio su dispositivo mobile)

---