# eduroam

1) Download "Linux" installer from: https://cat.eduroam.org/
   - DTU Installer might be at: https://cat.eduroam.org/user/API.php?action=downloadInstaller&api_version=2&lang=en&device=linux&profile=863

2) Extract the certificates from bottom of .py installer.
   - `$ file eduroam-dtu.pem`
   - `eduroam-dtu.pem: PEM certificate`

3) Connect to "eduroam"
   - Authentication: `Protected EAP (PEAP)`
   - Anonymous identity: `anonymous@dtu.dk`
   - Domain: `eduroam.dtu.dk`
   - CA certificate: `eduroam-dtu.pem`
   - Inner auth: `MSCHAPV2`

Volà no need to run a random installer.

