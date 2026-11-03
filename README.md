<h1 align="center">Maria Clara Dutra</h1>

<p align="center">
  <img src="https://github.com/user-attachments/assets/7f975700-a3c4-4466-9146-22aa59c23b6c" width="230" alt="Maria Clara Dutra" />
</p>

<p align="center">
  <strong>Software Engineering · Backend · Web · Applied AI</strong><br>
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

I build software that takes a raw input — a camera frame, a form, or a request in plain language — and turns it into a result someone can use.

My work sits in backend services, web products, and applied AI. That means APIs and interfaces where a model estimates, ranks, or drafts, and explicit rules keep the result reliable.

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

### Feelings
**Problem.** Reading age, emotion, and sex from a face usually means a heavy model on every camera frame, which stalls the preview, or a photo sent to a server the person never agreed to.

**What I built.** A webcam app in two forms. In Python, OpenCV YuNet finds the face and DeepFace estimates age, emotion, and sex. Inference runs about every 12 frames, so the preview stays fluid while the labels update. The web version runs in the browser: the camera or an uploaded photo is analyzed locally, with models loaded from a CDN, and nothing is uploaded.

**Impact.** A person sees the estimate on their own machine, in real time, and the interface stays usable because the expensive step is not tied to every frame. The labels are estimates, not facts.

**Stack.** `Python` · `OpenCV` · `DeepFace` · `JavaScript`

[Repository](https://github.com/dutra1904/feelingss)

### MenuMatch AI
**Problem.** A delivery guest describes a meal in plain language — light, dairy-free, under a price, ready soon, in a given area. A SQL filter can enforce price and a known allergen token. It cannot interpret “light” or “dairy,” and a model must not be allowed to relax a hard constraint to return a nicer match.

**What I built.** A Next.js client and a FastAPI service. Allergy, diet, price, time, and zone stay deterministic filters. Sentence embeddings rank only what those filters already allowed. A classifier suggests nutrition tags and cannot override the lock. The response is a shortlist plus an order with subtotal, fee, and total. Packaged with Docker.

**Impact.** Natural-language ordering without trading away allergen and policy safety. The model ranks; the rules decide what is allowed to exist in the result.

**Stack.** `Python` · `FastAPI` · `Next.js` · `sentence-transformers` · `scikit-learn` · `Docker`

[Repository](https://github.com/dutra1904/MenuMatchAI)

### BMI calculator
**Problem.** A BMI result is easy to misread when the form accepts bad input, or when the number arrives without the category and the distance to a healthy range.

**What I built.** A React 18 app on Vite. Height, weight, and age go through React Hook Form and Zod before the calculation. The screen returns the index, the category — underweight, normal, overweight, or obesity — and how much weight to lose or gain to reach the ideal range. Chakra UI keeps the form accessible, with validation messages on the field that failed.

**Impact.** The person gets a classified result and a concrete delta, and an incomplete or invalid entry never produces a number.

**Stack.** `React` · `Vite` · `Chakra UI` · `React Hook Form` · `Zod`

[Repository](https://github.com/dutra1904/calories)

---

## Activity

<p align="center">
  <img alt="GitHub stats" height="160" src="https://github-readme-stats.vercel.app/api?username=dutra1904&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github&include_all_commits=true" />
  <img alt="GitHub streak" height="160" src="https://streak-stats.demolab.com?user=dutra1904&theme=tokyonight&hide_border=true" />
</p>

<p align="center">
  <img alt="Top languages" height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=dutra1904&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" />
</p>
