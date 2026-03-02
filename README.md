```text
        @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@        
     @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@     
   @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@   
 @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@ 
 @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@                                               @@@@@@@@@@@@@@
@@@@@@@@                                                   @@@@@@@@@@
@@@@@@@@                                                    @@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@        @@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@        @@@@@@@
@@@@@@@@                    @@@@@@@@@@@@@@@@@@@@@@@@@@@       @@@@@@@
@@@@@@@@                    @@@@@@@@@@@@@@@@@@@@@@@@@@@       @@@@@@@
@@@@@@@@                    @@@@@@@@@@@@@@@@@@@@@@@@@@       @@@@@@@@
@@@@@@@@@@@@@@@@@@@@@       @@@@@@@@@@@@@@@@@@@@@@@@         @@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@      @@@@@                          @@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@      @@@@@                         @@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@      @@@@@                      @@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@      @@@@@       @@         @@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@      @@@@@       @@@@         @@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@      @@@@@       @@@@@@         @@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@      @@@@@       @@@@@@@@         @@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@      @@@@@       @@@@@@@@@@         @@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@      @@@@@       @@@@@@@@@@@         @@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@      @@@@@       @@@@@@@@@@@@@         @@@@@@@
@@@@@@@@@@@@@@@@@@@@@@      @@@@@       @@@@@@@@@@@@@@@         @@@@@
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
 @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
 @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@ 
   @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@   
     @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@     
        @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@        
```

# WP BiTi - Product Margine Calculator

Internal WooCommerce **margin/markup** calculator for Tratta e Ribassa with **role-restricted access**, **history tracking**, and **CSV exports**.

## Features

- **Restricted access (403)** for non-authorized users  
  Allowed roles: `administrator`, `shop_manager`, `subscriber`, `author`, `contributor`, `editor`  
  Not allowed: `customer` / clients (and any other role).
- **No indexing** (adds `X-Robots-Tag: noindex, nofollow, noarchive` + meta robots on plugin pages)
- Two calculation modes shown together:
  - **From Markup (RICARICO %)** → selling price, margins
  - **From Desired Margin (MARGINE %)** → selling price, resulting markup, margins
- Percent inputs are interpreted as **percent** (e.g., `22` = `22%`)
- Default values prefilled on every load:
  - Supplier discount: **57.50**
  - VAT rate: **22**
  - Markup: **20**
  - Desired margin: **20**
- **Product lookup** by **SKU** or **Product ID** to prefill fields
- **History table** + **Export CSV** (history) + **Export CSV** (last calculation)

## Requirements

- WordPress 6.x+
- WooCommerce active

## Installation

1. Upload the plugin folder to: `wp-content/plugins/`  
   (or upload the ZIP via **Plugins → Add New → Upload Plugin**)
2. Activate: **Plugins → Installed Plugins**
3. Use:
   - **Admin page**: WooCommerce → Calcolo Margine
   - **Frontend** endpoint: `/calcolo-margine/`
   - Or create a private WP page with shortcode:  
     `\[tratta_margine_calculator\]`

## Security & Privacy Notes

- This plugin is intended for internal use. It actively blocks access (403) for non-authorized roles.
- It adds **noindex/nofollow/noarchive** headers/meta on its pages to help prevent indexing.
- Do not share the URL publicly.

## License

GPL-2.0-or-later (see `LICENSE.txt`).

## Author

BiTi - Bogdan Tanasi (bogdan.tanasi@trattaeribassa.it)
