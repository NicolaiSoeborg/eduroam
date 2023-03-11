# Eduroam without installer (DTU guide)

## The "hard" way

1) Download Linux installer from: https://cat.eduroam.org/
   - DTU Installer might be at: https://cat.eduroam.org/user/API.php?action=downloadInstaller&api_version=2&lang=en&device=linux&profile=863

2) Extract the certificates from bottom of .py installer.
   - `$ file eduroam-dtu.pem`
   - `eduroam-dtu.pem: PEM certificate`
   You might want to put the file in e.g. `/etc/ssl/`.

3) Connect to "eduroam"
   - Authentication: `Protected EAP (PEAP)`
   - Anonymous identity: `anonymous@dtu.dk`
   - Domain: `win.dtu.dk` (or `eduroam.dtu.dk`?)
   - CA certificate: `eduroam-dtu.pem`
   - Inner auth: `MSCHAPV2`

Volà no need to run a random installer.

## The easy way

1) Download the cert [from this repo](https://raw.githubusercontent.com/NicolaiSoeborg/eduroam/master/eduroam-dtu.pem)

2) Follow step 3 above.
