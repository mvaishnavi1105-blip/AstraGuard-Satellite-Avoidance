# 🛡️ AstraGuard: AI-Based Satellite Trajectory Prediction & Collision Avoidance

AstraGuard is a simulation platform designed to predict satellite orbital trajectories using deep learning (LSTM), compute real-time collision risks, and simulate optimal $\Delta V$ avoidance maneuvers with interactive 3D visualizations.

---

## 🚀 Key Features
- **Real-Time Orbital Data:** Downloads publicly available TLE data via Skyfield & CelesTrak API.
- **Trajectory Prediction:** Employs an LSTM neural network to forecast satellite $X, Y, Z$ positions.
- **Collision Risk Engine:** Calculates Euclidean separation distance and classifies risk into LOW, MEDIUM, and HIGH alerts.
- **Avoidance Simulation:** Simulates an impulsive $\Delta V$ maneuver to recalculate safe operational trajectories.
- **Interactive 3D Dashboard:** Built with Streamlit and Plotly for full dynamic visualization.

---

## 🏗️️ System Architecture

1. **Input:** Fetch TLE orbital data from Celestrak.
2. **Preprocessing:** Convert TLE to 3D ECI position arrays $(X, Y, Z)$.
3. **Prediction:** LSTM predicts future orbital steps.
4. **Collision Detection:** Distance thresholding & risk flagging.
5. **Avoidance:** Apply $\Delta V$ offset post-alert.
6. **Dashboard:** Streamlit + Plotly 3D visual rendering.

---

## 📊 Model Performance
- **X-Axis MAE:** 58.11 km
- **Y-Axis MAE:** 357.51 km
- **Z-Axis MAE:** 42.66 km

---

## 🛠️ How to Run
1. Run the Google Colab Notebook.
2. Launch Streamlit via Ngrok tunnel.
3. Access the dashboard link generated in Colab.
