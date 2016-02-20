# Univr VPN Connect
Programma per connettersi a `sslvpn.univr.it` utilizzando le credenziali GIA.
## Requisiti
- Ubuntu 12.04 o successive
- Credenziali GIA valide
## Installazione
    $ git clone https://github.com/giovanni-liboni/vpnunivr.git
    $ sudo apt-get install lib32z1
    $ cd vpnunivr
    $ dpkg -i ncui_8.0-2_all.deb

Modificare `IDUTENTE` all'interno del file `connetti.sh`
``
IDUTENTE=id123abc
``
con il proprio utente.

## Connessione
Impostare i permessi di esecuzione con

    $ chmod 775 connetti.sh

Lanciare lo script con

    $ ./connetti.sh

Una volta lanciato verrà richiesta la password. Una volta immessa apparirà la scritta `Connecting to sslvpn.univr.it : 443` e la connessione con la VPN sarà attiva.
