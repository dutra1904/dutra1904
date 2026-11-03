<h1 align="center">Maria Clara Dutra</h1>

<p align="center">
  <img src="https://github.com/user-attachments/assets/7f975700-a3c4-4466-9146-22aa59c23b6c" width="230" alt="Maria Clara Dutra" />
</p>

<p align="center">
  <strong>Software Engineering · Backend · Distributed Systems & IoT · Applied AI</strong><br>
  Computer Engineering student at Universidade Federal de Goiás (UFG)
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/maria-clara-dutra-338876230">
    <img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white">
  </a>
  <a href="https://dutra1904.github.io/new_portfolio/">
    <img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-111111?style=for-the-badge&logo=githubpages&logoColor=white">
  </a>
  <a href="https://github.com/dutra1904">
    <img alt="GitHub" src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white">
  </a>
  <a href="mailto:dutramaria165@gmail.com">
    <img alt="Email" src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white">
  </a>
</p>

---

## About

I build software that takes data from a source — a sensor, a spreadsheet, or a user request — and turns it into something an operator or a customer can act on.

My work sits in backend services, distributed IoT, and applied AI. On the systems side, that means APIs, messaging, and time-series pipelines. On the product side, it means web applications where a language model ranks or drafts, and deterministic rules keep the outcome safe.

I have hands-on experience with software development and data in corporate settings, and I serve on the board of the student association (Centro Acadêmico) at UFG, running academic and outreach work for the computing community.

---

## Stack

**Languages**

<p>
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white">
  <img alt="Java" src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white">
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white">
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black">
  <img alt="SQL" src="https://img.shields.io/badge/SQL-003B57?style=flat-square">
  <img alt="C" src="https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black">
  <img alt="C++" src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white">
</p>

**Backend, data, and infrastructure**

<p>
  <img alt="Spring Boot" src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white">
  <img alt="FastAPI" src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white">
  <img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white">
  <img alt="MySQL" src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white">
  <img alt="InfluxDB" src="https://img.shields.io/badge/InfluxDB-22ADF6?style=flat-square&logo=influxdb&logoColor=white">
  <img alt="MQTT" src="https://img.shields.io/badge/MQTT%20%2F%20Mosquitto-3C5280?style=flat-square&logo=eclipsemosquitto&logoColor=white">
  <img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white">
  <img alt="Grafana" src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white">
</p>

**Web, AI, and analytics**

<p>
  <img alt="React" src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black">
  <img alt="Next.js" src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white">
  <img alt="HTML5" src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white">
  <img alt="CSS3" src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css&logoColor=white">
  <img alt="LangChain" src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white">
  <img alt="Pandas" src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white">
  <img alt="Power BI" src="https://img.shields.io/badge/Power%20BI-F2C811?style=flat-square&logo=powerbi&logoColor=black">
</p>

---

## Selected projects

### Distributed environmental monitoring
**Problem.** A chemistry lab needs a continuous read on air quality, climate, and occupancy, with risk called out before someone has to piece the signals together by hand.

**What I built.** An edge-to-dashboard pipeline: ESP32 nodes publish JSON over MQTT (Eclipse Mosquitto). A Java 17 / Spring Boot service ingests the stream into InfluxDB. Grafana shows the live state, and decision rules flag critical risk and environmental leaks. QoS, last-will, and keep-alive keep a dropped node visible instead of silent.

**Impact.** Telemetry from the UFG chemistry lab becomes one operational view, with the failure of a device distinguishable from “nothing is wrong.”

**Stack.** `ESP32` · `MQTT` · `Spring Boot` · `InfluxDB` · `Grafana`

[Repository](https://github.com/dutra1904/monitotamento)

### MenuMatch AI
**Problem.** A delivery guest describes a meal in plain language — light, dairy-free, under a price, ready soon, in a given area. A SQL filter can enforce price and a known allergen token. It cannot interpret “light” or “dairy,” and a model must not be allowed to relax a hard constraint to return a nicer match.

**What I built.** A Next.js client and a FastAPI service. Allergy, diet, price, time, and zone stay deterministic filters. Sentence embeddings rank only what those filters already allowed. A classifier suggests nutrition tags and cannot override the lock. The response is a shortlist plus an order with subtotal, fee, and total. Packaged with Docker.

**Impact.** Natural-language ordering without trading away allergen and policy safety. The model ranks; the rules decide what is allowed to exist in the result.

**Stack.** `Python` · `FastAPI` · `Next.js` · `sentence-transformers` · `scikit-learn` · `Docker`

[Repository](https://github.com/dutra1904/MenuMatchAI)

### Grade and attendance automation
**Problem.** Approval status was a manual pass over grades and attendance in a spreadsheet: average, exam threshold, and the minimum score still needed to pass.

**What I built.** A Python pipeline on the Google Sheets API. Pandas reads P1–P3 and attendance, applies the approval rules, and writes status — pass, final exam, or fail — plus the minimum passing grade back to the sheet.

**Impact.** The rulebook runs the same way on every row, and the sheet stays the system of record instead of a one-off export.

**Stack.** `Python` · `Pandas` · `Google Sheets API`

[Repository](https://github.com/dutra1904/challenge-teckna)

---

## Activity

<p align="center">
  <img alt="GitHub stats" height="160" src="https://github-readme-stats.vercel.app/api?username=dutra1904&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github&include_all_commits=true" />
  <img alt="GitHub streak" height="160" src="https://streak-stats.demolab.com?user=dutra1904&theme=tokyonight&hide_border=true" />
</p>

<p align="center">
  <img alt="Top languages" height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=dutra1904&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" />
</p>
