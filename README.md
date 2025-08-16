# Public export

# 🗺️ Jurnee (COMP47360 - Group 10)

The **Jurnee** app was built and developed for COMP47360 by Group 10.
Jurnee is an web-based application that auto generates a day-level itinerary to different user-picked destinations, scheduling visit times based on busyness levels (predicted via ML) around the destinations, distance, weather and other criteria.

See the app in action at www.jurnee.dpdns.org.

> [!Warning]
> Website non-functional as of 1 August 2025, 20:00. Google API keys disabled in order to avoid service charges. This is inline with email received from Alessio Ferrari on 24 July confirming that website execution can be stopped on 1 August 2025, 18:00.

---

## Table of Contents

- [✨ Features](#-features)
- [📊 Data](#-data)
- [🚀 Getting Started](#-getting-started)
- [💻 Usage](#-usage)
- [🧬 Testing](#-testing)
- [📝 License](#-license)
- [👏 Contributors](#-contributors)

---

## ✨ Features

### **Map Page**:

<p align="left">
 <img src="https://github.com/mel-ozkul/COMP47360/blob/main/additional-resources/features-images/map-page.png" height="250" style="border:1px solid #fff; padding:5px;">
 <img src="https://github.com/mel-ozkul/COMP47360/blob/main/additional-resources/features-images/map-page-2.png" height="250" style="border:1px solid #fff; padding:5px;">
</p>

### **User Input (Date & Location)**:

<p align="left">
 <img src="https://github.com/mel-ozkul/COMP47360/blob/main/additional-resources/features-images/datepicker.png" height="250" style="border:1px solid #fff; padding:5px;">
 <img src="https://github.com/mel-ozkul/COMP47360/blob/main/additional-resources/features-images/location-input.png" height="250" style="border:1px solid #fff; padding:5px;">
</p>

### **Weather**:

<p align="left">
 <img src="https://github.com/mel-ozkul/COMP47360/blob/main/additional-resources/features-images/weather.png" height="250" style="border:1px solid #fff; padding:5px;">
</p>

### **Destination Search**:

<p align="left">
 <img src="https://github.com/mel-ozkul/COMP47360/blob/main/additional-resources/features-images/destination-search.png" height="250" style="border:1px solid #fff; padding:5px;">
</p>

### **Suggested Destinations List**:

<p align="left">
 <img src="https://github.com/mel-ozkul/COMP47360/blob/main/additional-resources/features-images/suggested-destinations.png" height="250" style="border:1px solid #fff; padding:5px;">
</p>

### **Detailed Destination Information**:

<p align="left">
 <img src="https://github.com/mel-ozkul/COMP47360/blob/main/additional-resources/features-images/more-info-description.png" height="250" style="border:1px solid #fff; padding:5px;">
 <img src="https://github.com/mel-ozkul/COMP47360/blob/main/additional-resources/features-images/more-info-hours.png" height="200" style="border:1px solid #fff; padding:5px;">
</p>

### **Itinerary Generation (ML & Algorithm)**:

<p align="left">
 <img src="https://github.com/mel-ozkul/COMP47360/blob/main/additional-resources/features-images/generated-itinerary.png" height="250" style="border:1px solid #fff; padding:5px;">
</p>

### **Map Routing**:

<p align="left">
 <img src="https://github.com/mel-ozkul/COMP47360/blob/main/additional-resources/features-images/generated-route.png" height="250" style="border:1px solid #fff; padding:5px;">
</p>

### **Busyness Indicator**:

<p align="left">
 <img src="https://github.com/mel-ozkul/COMP47360/blob/main/additional-resources/features-images/busyness-chart.png" height="250" style="border:1px solid #fff; padding:5px;">
</p>

### **Home Page**:

<p align="left">
 <img src="https://github.com/mel-ozkul/COMP47360/blob/main/additional-resources/features-images/home-page.png" height="400" style="border:1px solid #fff; padding:5px;">
</p>

### **About Page**:

<p align="left">
 <img src="https://github.com/mel-ozkul/COMP47360/blob/main/additional-resources/features-images/about-page.png" height="400" style="border:1px solid #fff; padding:5px;">
</p>

---

## 📊 Data

> [!IMPORTANT]
> Data specific details can be found [in the README_DATA](https://github.com/mel-ozkul/COMP47360/blob/main/data/README_DATA.md).

The core output of this project is a trained predictive model that estimates the busyness score of an area in Manhattan at a specific date and hour. This model serves as a critical component for downstream applications such as itinerary optimisation, route recommendation, or spatiotemporal demand analysis.

We created an interactive HTML map based on our trained predictive model that allows you to explore of 5PM busyness patterns. This visualization includes:

- Color-coded Voronoi cells based on normalised busyness score
- Hover tooltips showing cell ID and log-score
- Optional taxi zone boundaries as contextual reference

**See the map here:** [View Busyness Map](https://github.com/mel-ozkul/COMP47360/blob/main/data/d_data_v2_cleaning_after_eda/interactive_heatmap_busyness_score_display/interactive_busyness_hour17_final.html)

---

## 🚀 Getting Started

> [!IMPORTANT]
> Backend specific instructions can be found [in the README_BACKEND](https://github.com/mel-ozkul/COMP47360/blob/main/backend/README_BACKEND.md).
>
> Frontend specific instructions can be found [in the README_FRONTEND](https://github.com/mel-ozkul/COMP47360/blob/main/frontend/README_FRONTEND.md).

### Prerequisites:

**FRONTEND**

- Node.js (version 20.19.2)
- npm (comes with Node.js)

Use **nvm** (macOS/Linux) or **nvm-windows** (Windows) to manage Node versions easily.

To install prerequisites on macOS/Linux, refer to: https://github.com/nvm-sh/nvm#installing-and-updating

</br>

**BACKEND**

- Rust (Any Modern Version): https://www.rust-lang.org/tools/install
- Cargo (Workspace/File Manager - Pre-Installed with Rust)
- Postgres (Any Modern Version)

</br>

### Installation:

**FRONTEND**

1. Download the nvm-windows installer (nvm-setup.exe) from the official repository: https://github.com/coreybutler/nvm-windows/releases/latest

2. Run the installer and follow the on-screen instructions.

3. Open a new Command Prompt or PowerShell window (important to open a new window so changes take effect).

4. Install the recommended Node.js version:

```
nvm install 20.19.2
```

6. Set the Node.js version to use:

```
nvm use 20.19.2
```

8. Verify Node and npm are installed:

```
node -v
npm -v
```

</br>

**BACKEND**

**Rust (Windows):**

1. Rust Install Command:

```
curl https://sh.rustup.rs -sSf | sh
```

Alternatively visit: `https://www.rust-lang.org/tools/install`

2. Rust will prompt for different installations, proceed with option:

```
1
```

3. Restart the terminal

4. Following the restart, verify the installation via commands:

```
rustc --version
cargo --version
```

</br>

**Rust (Apple):**

1. Rust Install Command:

```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs/ | sh`
```

Alternatively visit: `https://www.rust-lang.org/tools/install`

2. Rust will prompt for different installations, proceed with option:

```
1
```

3. Restart the terminal

4. Following the restart, verify the installation via commands:

```
rustc --version
cargo --version
```

</br>

**Postgres (All)**

1. Follow the link below and select the relevant OS installer: `https://www.postgresql.org/download/`

2. Once installed and running, access the terminal with:

```
psql -U postgres
```

3. Set a password for the default user:

```
\password postgres
```

    For our configuration, the password is just simple "x" in lowercase.

    If a password is already set, this command allows you to change it.

4. Run the following database creation commands:

```
CREATE DATABASE jurnee

CREATE DATABASE test
```

    The test database is utilised for testing.

5. While still in the postgres terminal, verify the database's exist through the following command:

```
\l
```

</br>

### Model Loading:

1. The model size exceeds what can be stored on GitHub, the deployment model can be found at: `https://drive.google.com/drive/folders/1e-4y7bhn9lRVcEiQpNbgVhKfOdMmFBdy?usp=sharing`

2. Once downloaded, ensure the model name is "model_final.onnx".
   - Then, inside of the "backend" folder is a "models" folder
   - Insert the model into that folder.

### Configuration:

Set up the `.env` file in the project root directiory and add:

```
VITE_GOOGLE_MAPS_API_KEY=your_google_maps_api_key_here

# Root addresss of backend Rust server:
VITE_API_URL=http://localhost:8000
```

---

## 💻 Usage

### Running the app:

**BACKEND**

1. Ensure that you are within the "backend" directory

2. Run the following command:

```
 cargo run --release
```

</br>

**FRONTEND**

1. Clone the repo (if you haven't already):

```
git clone https://github.com/mel-ozkul/COMP47360.git
cd COMP47360
```

2. Install dependencies:

```
npm install
```

3. Run the development server:

```
npm run dev
```

4. Open your browser and go to (or follow the link from the terminal):

```
http://localhost:5173
```

**Detailed usage instructions:**

1. Enter the web page.
2. Navigate to the Map page either by clicking 'Plan Jurnee' or by clicking the 'Map' navigation menu.
3. Add the date of your visit, the starting location, and the locations you would like to visit in Manhattan, New York, USA.
4. Click the 'Generate Jurnee' button at bottom of the page.
5. The algorithm will calculate the best order and route for the locations you picked, providing visit start times, and optimising for busyness, distance, weather and other criteria.

---

## 🧬 Testing

To run the test suite, use the following command:

```
cargo test -- --test-threads=1 --include-ignored
```

---

## 📝 License

This project was developed solely for academic purposes as part of COMP47360 (Research Practicuum). It is not licensed for public or commercial use.

---

## 👏 Contributors

Made with ❤️ by Group 10:

- [Alicja Koziel](https://github.com/alicja-koziel)
- [Denis Semenov](https://github.com/dsmnov)
- [YuWei Lin](https://github.com/YuWei610)
- [Melissa Oezkul](https://github.com/mel-ozkul)
- [Valentino Braga Aquino](https://github.com/tinobragaa)
