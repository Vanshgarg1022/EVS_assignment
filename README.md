# EVS_assignment
SmartBin Alert is a smart waste management prototype that monitors simulated bin fill levels, visualizes bin status on an interactive dashboard, flags overflow risks, and supports citizen reporting and collection route planning. Built with HTML, CSS, and JavaScript, with planned ESP32, IoT, cloud, and ML integration.

A smart waste management prototype for cleaner, smarter cities.
SmartBin Alert is a browser-based prototype designed to demonstrate how technology can help municipal teams monitor public dustbins, identify overflow risks, coordinate collection, and receive citizen reports. The current version uses simulated bin data and runs directly in a web browser.
Project status: Front-end prototype. ESP32 sensor integration, cloud storage, real-time notifications, live map services, and trained machine-learning predictions are not yet connected.

🌍 Problem Statement
Public dustbins can overflow between scheduled collections, causing litter, unpleasant odours, pest activity, and waste entering drains and waterways. Fixed collection schedules may also lead to unnecessary trips to bins that are not yet full.
SmartBin Alert explores a data-driven approach: monitor fill levels, highlight bins that need attention, and help collection teams prioritize their work.
✨ Features
- Dashboard: Overview of total bins, normal/warning/critical status, fill trends, and priority bins.
- Interactive bin map: Click bin markers to inspect fill level, location, sensor update time, and sample reading history.
- Alerts: Review critical and warning bins, search alerts, and mark bins as reviewed.
- Analytics: View illustrative fill trends, overflow-prone locations, and estimated time-to-fill.
- Collection route planning: Generate a simulated priority route based on bin fill levels.
- Citizen reporting: Submit reports for overflowing or damaged bins, missed collections, and illegal dumping. Optional photo attachment is supported by the form.
- Report management: Review submitted reports and mark them as resolved.
- Settings: View demo system configuration and sample alert thresholds.
- Responsive layout: Sidebar and dashboard adapt to smaller screens.
🖥️ Screens
The prototype includes these sections:
1. Dashboard
2. Live Map
3. Alerts & Notifications
4. Waste Analytics
5. Collection Route Planning
6. Citizen Reports
7. Bin Details
8. Settings
🛠️ Built With
- HTML5 — page structure
- CSS3 — styling and responsive layout
- Vanilla JavaScript — navigation, sample data, filters, modal details, reports, and interactions
Planned integrations
- ESP32 microcontroller and HC-SR04 ultrasonic sensor
- Firebase or MySQL for storing bin information and sensor readings
- Python and scikit-learn for fill-level prediction
- OpenStreetMap-based mapping and routing services
- SMS, email, or app notifications
These integrations are planned extensions and are not active in the current prototype.
🚀 Run Locally
No package installation or build step is required.
1. Clone this repository:
   git clone https://github.com/YOUR-USERNAME/smartbin-alert.git
2. Open the project folder:
   cd smartbin-alert
3. Open smartbin_alert_prototype.html in your browser.
You can also use VS Code with the Live Server extension if you prefer to serve the page locally.
🧪 Try the Demo
- Navigate between sections using the sidebar.
- Click a bin marker or View details to inspect a bin.
- Filter bins and alerts by status.
- Open Route Planning and generate a sample priority route.
- Open Citizen Reports and submit a sample issue.
- Mark a report as resolved to see the updated status.
The sample locations and readings are illustrative. They should not be treated as live municipal data.
🧠 How the Proposed System Would Work
The intended end-to-end system could follow this flow:
1. An ultrasonic sensor measures the distance between the bin lid and the waste surface.
2. An ESP32 converts the distance into an estimated fill percentage.
3. The device sends the bin ID, fill level, and timestamp to a cloud database.
4. The dashboard displays each bin's status:
   - Normal: below 60%
   - Warning: 60% to 80%
   - Critical: above 80%
5. The system alerts sanitation staff when a bin needs attention.
6. Historical readings can be used to predict when bins may reach critical capacity.
7. A routing service can help plan collection using road distances and vehicle constraints.
8. Citizens can report overflow or damage using a QR-linked form.
The current browser prototype simulates this workflow's user interface; it does not perform these hardware and backend steps.
🗺️ Roadmap
- [x] Build responsive dashboard UI
- [x] Add simulated bin data and status indicators
- [x] Add clickable bin details
- [x] Add alert filtering and review interactions
- [x] Add citizen reporting form
- [x] Add simulated route planning and analytics
- [ ] Connect ESP32 and ultrasonic sensors
- [ ] Store readings in a persistent database
- [ ] Add real-time data updates
- [ ] Integrate live mapping and road routing
- [ ] Implement and evaluate a fill-level prediction model
- [ ] Add real email/SMS notifications
- [ ] Deploy a public demo
🌱 Expected Impact
If implemented and evaluated in a real deployment, a system like SmartBin Alert could help:
- Reduce waste overflow and litter around public bins.
- Improve the prioritization of collection work.
- Identify locations that may need additional bins or more frequent collection.
- Support more efficient vehicle routing and potentially reduce fuel use.
- Give citizens a simple way to report waste-management issues.
These are intended benefits; actual impact would need to be measured in a pilot deployment.
🤝 Contributing
Contributions and suggestions are welcome. You can help by improving the dashboard, adding accessibility support, integrating sensor data, designing a database schema, or implementing routing and prediction modules.
1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Open a pull request describing the improvement.
