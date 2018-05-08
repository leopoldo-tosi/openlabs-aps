---
layout: page
title: il servizio mail di OpenLabs
---

TODO: verificare validità e funzionamento indirizzi di posta

![immagine mail](Email OpenLabs)

Negli ultimi anni con l'aumento delle minacce è cresciuta anche la consapevolezza di quanto sia critica la gestione dell'email ai fini della sicurezza informatica, della tutela dei dati personali e della certezza della comunicazioni.

Per questi motivi a breve OpenLabs renderà disponibile ad ogni associato un servizio email pensato proprio per chi, come noi, ha questa consapevolezza.

>Abbiamo progettato un servizio email che garantisse anzitutto l'affidabilità e la sicurezza, e quindi abbiamo implementato l'autenticazione dell'identità del mittente tramite DKIM, SPF e DMARC per aumentare la deliverability. Poi abbiamo aggiunto filtri antispam e controlli antimalware, per proteggere la posta in arrivo da ogni tipo di minaccia. Per garantirti l'accesso sempre, ovunque e con qualsiasi dispositivo (pc, tablet, smartphone) abbiamo reso disponibili la webmail e il protocollo IMAP. Infine, per consentire la gestione dei messaggi tramite regole e workflow elaborati, abbiamo attivato gli alias e il subaddressing.

Lo stack di software utilizzato per il servizio email è composto da:

| Ruolo | Software adottato |
|:-:|:-:|
| Mail delivery agent | _Dovecot_ |
| Mail transfer agent | _Postfix_ |
| Gestione database utenti | _OpenLDAP_ |
| Sistema operativo | _Debian GNU/Linux_ |

## Email degli associati a OpenLabs

OpenLabs offre ad ogni associato un indirizzo email ```tuonome@openlabs.it```.
La richiesta di assegnazione dell'indirizzo può essere fatta durante la compilazione del modulo di adesione, oppure inviando una richiesta a **postmaster@openlabs**.

Una volta attivato l'account riceverai le istruzioni per configurare in totale autonomia il servizio.
Potrai impostare l'email come alias con redirect ad un altro indirizzo o come mailbox (disponibili i protocolli _IMAP_ e _POP3_).
Potrai anche configurare connettori da e verso altri servizi email, e usare infiniti suffissi di subadressing del tipo: ```nome-subaddressing@openlabs.it.```

## Email istituzionali e di servizio

Mentre le email degli associati sono personali, quelle istituzionali e di servizio vengono passate alla persona che pro tempore ricopre l'incarico.

Attualmente sono stati attivati e configurati e seguenti indirizzi:

| email | tipo | assegnatario |
|:-:|:-:|:-:|
| presidente@openlabs.it | mailbox | Andrea Rossi |
| tesoriere@openlabs.it | mailbox	| Riccardo Scartozzi |
| direttivo@openlabs.it | alias | Vittorio Belloni, Alberto Campiglio, Andrea Rossi, Riccardo Scartozzi |
| probiviri@openlabs.it | alias | Fabrizio Ficci |
| postmaster@openlabs.it | alias | Riccardo Scartozzi |
| info@openlabs.it | alias | presidente |
| paypal@openlabs.it | alias | tesoriere |
