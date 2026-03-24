# ⚽ Football Analytics Hub: 2026 Pipeline

An automated, end-to-end data engineering project that fetches, transforms, and visualizes global football data using a modern **Medallion Architecture**.

## 🚀 Live Demo
Check out the live dashboard: (https://chaitanya1110-creates.github.io/football_pl_laliga_pipeline/)

## 🏗️ Technical Architecture

### 1. Data Ingestion (Bronze Layer)
- Automated ingestion of raw JSON payloads from OpenFootball and historical CSV datasets.
- Handled via **Databricks** and **PySpark**.

### 2. Data Transformation (Silver Layer)
- Adaptive parsing logic to handle varying JSON structures (Rounds vs. Matches).
- Data cleaning, schema enforcement, and point calculation logic (3 for Win, 1 for Draw).

### 3. Analytics & Aggregation (Gold Layer)
- Final production-ready tables generated using **Spark SQL**.
- 100% data-driven; no hardcoded values.
- Includes dynamic calculation of current season leaders and historical all-time winningest nations.

### 4. Automated Sync (The Bridge)
- **GitHub REST API Integration:** A custom Python script pushes processed JSON files from Databricks directly to this repository's `/data` folder.
- **CI/CD:** GitHub Pages automatically redeploys the frontend whenever the data folder is updated.

### 5. Frontend Dashboard
- **Tech Stack:** Vanilla HTML5, CSS3 (Glassmorphism), and JavaScript (Fetch API).
- **Design:** Dark-mode "Frosted Glass" UI optimized for mobile and desktop.
- **Performance:** Zero external CSS/JS libraries for sub-500ms load times.

## 🛠️ Tools Used
- **Databricks / Unity Catalog**
- **PySpark / Spark SQL**
- **Python (Requests, Base64, JSON)**
- **GitHub Pages & Actions**

## 📂 Project Structure
- `index.html`: The main dashboard frontend.
- `data/`: Automated storage for pipeline-generated JSON files.
- `notebooks/`: (Optional: add your Databricks export here)

## 👤 Author
**Chaitanya**
*Data Engineer & Agency Owner*
[LinkedIn Profile Link]
