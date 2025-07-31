Home Assistant Dashboard
A modern, multi-floor Home Assistant dashboard built with Mushroom UI, Mini Graph Cards, and ApexCharts.
It provides lighting, blinds, media, temperature, humidity, and energy price control for a smart home setup.

📷 Preview
(Add a screenshot here, for example)

scss
Copy
Edit
![Dashboard Preview](images/dashboard_preview.png)
✨ Features
🏠 Multi-floor smart home control (1st & 2nd floors)

💡 Lighting & group controls with brightness and color feedback

🪟 Blinds control (open / pause / close for individual or grouped blinds)

🌡 Temperature & humidity charts with min/max/avg values

⚡ Nordpool energy price charts (today & tomorrow)

📺 Media player controls for dining room and bedroom

⚽ Sports view with live team tracking

🔋 Battery status overview for all devices

📦 Dependencies
Ensure you have HACS installed, then install the following custom cards:

Mushroom Cards

mushroom-title-card

mushroom-person-card

mushroom-chips-card

mushroom-template-card

mushroom-light-card

mushroom-entity-card

Mini Graph Card

ApexCharts Card

Battery State Card

Slider Button Card

Team Tracker Card

📂 Dashboard Structure
The dashboard has 4 main views:

Home View

Dynamic greeting by time of day

Weather & light summary

Temperature history & Nordpool energy prices

1st and 2nd floor lighting & blinds controls

Media controls for dining & bedroom

WIP (Testing) View

Extended graphs for temperature & humidity

Test cards for lights, blinds, and sliders

Sports View

Track live sports with sensor.team_tracker entities

Battery Status View

Overview of all device battery levels

⚙️ Installation
Clone this repository or copy the ui-lovelace.yaml file to your Home Assistant config:

bash
Copy
Edit
/config/ui-lovelace.yaml
Install dependencies using HACS.

Enable YAML mode in Home Assistant if not already:

Configuration → Dashboards → Options → Use YAML Mode

Reload Lovelace to apply changes.

🛠 Maintenance Tips
Backup Config:
Dashboard config is stored at:

arduino
Copy
Edit
/config/.storage/lovelace
Update Custom Cards:
HACS → Frontend → Update All

Use WIP View for Testing:
Avoid breaking the main dashboard by testing new cards in the WIP view.

🗺 Future Ideas
Floor plan integration with Picture Elements Card

Energy usage overlay on Nordpool chart

Conditional visibility for unavailable devices

If you want, I can also generate a .github/workflows/ha-dashboard-check.yml for your repo to validate your YAML automatically when you push updates.

Do you want me to add a GitHub Actions workflow for HA YAML validation? This keeps your repo error-free.
