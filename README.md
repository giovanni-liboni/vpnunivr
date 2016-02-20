# Univr VPN Connect
Programma per connettersi a `sslvpn.univr.it` utilizzando le credenziali GIA.
## Requisiti
- Ubuntu 12.04 o successive a 64bit ( amd64 )
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

- Controllare l'indirizzo ip per l'avvenuta connessione con la VPN ( Il nuovo indirizzo inizia con 157.27 ).
- La scritta `Connecting to sslvpn.univr.it : 443` sara' visibile per tutta la durata della connessione.
- Per interrompere la connessione terminare lo script.
