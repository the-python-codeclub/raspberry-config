# Headless WiFi setup
Schrijf een leeg bestand met de naam ssh naar de root van de sd-kaart
Kopieer onderstaande code en schrijf deze weg als `wpa_supplicant.conf` naar de root van sd  

`ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev`  
`update_config=1`  
`country=US`  

`network={`  
`  ssid="Netwerknaam"`  
`  psk="Wachtwoord"` <-- deze regel verwijderen als het netwerk geen wachtwoord heeft  
`}`  

# software updaten
sudo apt-get update  
sudo apt-get upgrade  

# updaten van de Raspberry PI firmware 
sudo rpi-update  

# Gebruikers toevoegen

sudo adduser $GEBRUIKER  
sudo adduser $GEBRUIKER gpio  
