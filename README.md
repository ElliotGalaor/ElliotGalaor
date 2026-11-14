# Hi, I'm Elliot 👋

I'm passionate about applied mathematics, agentic development and building data pipelines. I use GitHub as my portfolio showcase: every repository here is a project I built out of curiosity and to keep learning.

## 🔭 What I'm into
- **Mathematics & visualization**: numerical methods, dynamical systems, fractals
- **Agentic development**: designing systems where AI agents orchestrate tasks and tools end to end
- **Data pipelines**: API ingestion, transformation, analytical SQL, embeddings and vector search
- **Shipping complete applications**: web APIs, dashboards, Docker and CI/CD all the way to production

## 🏗️ What I'm working on

### 🌦️ [MeteoReading](https://github.com/ElliotGalaor/MeteoReading) · [live demo](https://meteoreading-fqwbevysja-ew.a.run.app)
**75 years of climate in 20 French cities.** An end-to-end data pipeline that collects **25 million official Météo-France weather records**, cleans them into a **DuckDB** warehouse, draws statistically sound conclusions and presents them in an interactive **Streamlit** dashboard and an HTML report.
- Analytical SQL (window functions, `QUALIFY`, `PIVOT`), data-quality checks and statistics (Mann-Kendall, Theil-Sen, record analysis), cross-validated against the ERA5 reanalysis
- Key findings: the 20 cities have warmed by **+0.33 °C per decade since 1951**, and days at 35 °C or more are **5.5 times** more frequent
- Weather along any GPS track: draw a route or import a GPX/KML/GeoJSON file to see the conditions at the time you pass each point
- Deployed on **Google Cloud Run**: Docker image built once with its data, staging then production after approval, weekly data refresh

### ♻️ [ElectronicEnvironmental](https://github.com/ElliotGalaor/ElectronicEnvironmental) · [live demo](https://rohs-checker.onrender.com)
**RoHS · REACH · ECCN Checker.** A web application that checks the environmental compliance and the export control of an electronic bill of materials (BOM) in seconds.
- Reads BOMs exported from any CAD tool, ERP or distributor (CSV, Excel `.xlsx` / `.xlsb` / `.xls`), detects the columns and matches every component against a reference database
- Verdict per regulation (RoHS 2, RoHS 3, REACH) built on the official texts: RoHS exemptions and their expiry dates from EUR-Lex, the ECHA Candidate List of substances of very high concern, ECCN export codes from the US Commerce Control List
- Compliant equivalents from other manufacturers, substitution in the BOM, Excel reports, datasheet extraction from PDF
- **FastAPI**, SQLite and framework-free JavaScript, user accounts with edit access approved by the administrator, deployed on **Render**

Both projects are run like team projects: issues, one pull request per change, CI on three Python versions, and a Docker image built once, then promoted from staging to production. The demos run on free or capped plans: after a quiet period, the first visit takes a few seconds (MeteoReading) to about a minute (ElectronicEnvironmental).

## 🚀 Other projects
- [**PaperReading**](https://github.com/ElliotGalaor/PaperReading) — A pipeline that collects papers from arXiv and OpenAlex, encodes them with SPECTER2 and indexes them in pgvector to surface the most similar work.
- [**Newton_Fractals**](https://github.com/ElliotGalaor/Newton_Fractals) — Generating and visualizing Newton fractals in Python.

## 🛠️ Tools
Python · SQL (DuckDB, PostgreSQL / pgvector, SQLite) · FastAPI · Streamlit · JavaScript · Docker · GitHub Actions · Google Cloud Run · Render · Embeddings (SPECTER2) · arXiv & OpenAlex APIs

## 📫 Get in touch
📍 Marseille, France · [LinkedIn](https://www.linkedin.com/in/elliot-galaor/)
