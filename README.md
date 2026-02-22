# homebridge-molekule
A Homebridge Plugin for Molekule Air Purifiers. Tested on the Air Mini. Once you install this plugin you can say:
```
Hey Siri, what's the status of the Air Purifier Filter?
Hey Siri, set the speed of the Molekule to 60%.
```
## Installation

### Via Homebridge UI (Recommended)

1. Open the **Homebridge UI** in your web browser
2. Navigate to the **Plugins** tab
3. Click the **Search** button (or use the search bar)
4. Search for **"Molekule"** or **"homebridge-molekule"**
5. Click on the plugin in the search results
6. Click the **Install** button
7. Wait for the installation to complete

### Via Command Line

Alternatively, you can install via npm:
```bash
npm -g i @mgurreta/homebridge-molekule
```

## Configuration

### Via Homebridge UI

1. After installation, go to the **Plugins** tab in Homebridge UI
2. Find **Homebridge Molekule** in your installed plugins list
3. Click the **Settings** (gear icon) or **Configure** button
4. Fill in the configuration form:
   - **Name**: Platform name (default: "homebridge-molekule")
   - **Email**: Your Molekule account email address
   - **Password**: Your Molekule account password
   - **Filter Change Warning Percentage**: Threshold for filter change warnings (default: 5%)
5. Click **Save** to apply the configuration
6. The plugin will restart automatically and discover your Molekule devices

### Manual Configuration

If you prefer to configure manually, add this to your `config.json` file under Platforms:
```json
{
  "platform": "Molekule",
  "name": "homebridge-molekule",
  "email": "YOUR EMAIL HERE",
  "password": "YOUR PASSWORD HERE",
  "threshold": 10
}
```
# Notes and Issues
Using an incorrect password can cause a need for a full password reset on your account. Pay special attention to the password you're using.
This plugin loads the names that are set for each device in the Molekule app. 
