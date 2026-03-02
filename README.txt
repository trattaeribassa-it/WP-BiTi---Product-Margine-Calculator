WP BiTi - Product Margine Calculator (0.1.1)

INSTALLAZIONE
1) Carica la cartella del plugin in wp-content/plugins/ oppure installa lo zip dal pannello Plugin.
2) Attiva il plugin.
3) Vai in WooCommerce → Calcolo Margine (admin).
4) Per frontend:
   - Endpoint rapido: /calcolo-margine/ (slug modificabile nel codice: option TRCM_OPTION_KEY -> endpoint_slug)
   - Oppure crea una pagina privata e inserisci lo shortcode:
     [tratta_margine_calculator]

ACCESSO
Consentito solo ai ruoli:
- administrator
- shop_manager
- subscriber
- author
- contributor
- editor

SICUREZZA / SEO
- Risposta 403 per utenti non autorizzati.
- Header X-Robots-Tag + meta robots: noindex, nofollow, noarchive.
- Nessun contenuto visibile a utenti non autorizzati.

FUNZIONI
- Calcolo come Excel (ricarico + margine desiderato) in tempo reale.
- Caricamento prodotto da SKU/ID (WooCommerce) con prefill listino + IVA.
- Storico (tabella) + export CSV storico.
- Export CSV ultimo calcolo (salva anche nello storico).

LICENZA
GPLv2 o successive (GPL-2.0+). Vedi LICENSE.txt.

