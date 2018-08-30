# EduroamLinuxConfig
A repo that helps configure eduroam for linux. I had remarkable trouble connecting to eduroam on my raspberry pi so set up this repo as a reference.

## How to set up eduroam using this repo
- First you need to download your university's eduroam config generator from [here](https://cat.eduroam.org/). This can be done on a computer on a different network and then copied to the pi via a USB, SD card, etc.
- Run the config generator file (eduroam-linux-NUoIG.sh in this repo, don't forget to give executable permission chmod +x eduroam-linux-YourUniversity.sh) and enter your details when prompted. It should generate a ca.pem certificate file and a cat_installer.conf file in ~/.cat_installer. The files generated on my pi are provided as a reference (with my details removed!)
- Run sudo activate_wpa_supplicant.sh
- If there any issues, try restarting your device, removing the downloaded files and starting again
