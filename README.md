<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/banner-light.svg">
  <img alt="Juan Cruz Enzetti — Senior QA Analyst moving into QA Automation" src="./assets/banner-light.svg" width="100%">
</picture>

<p align="center">
  <a href="https://www.linkedin.com/in/juanenzetti/"><img src="https://img.shields.io/badge/LinkedIn-juanenzetti-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:juancruzenzetti@gmail.com"><img src="https://img.shields.io/badge/Email-juancruzenzetti%40gmail.com-EA4335?style=flat&logo=gmail&logoColor=white" alt="Email"></a>
  <img src="https://img.shields.io/badge/Open_to-QA_Automation_roles-2EA043?style=flat" alt="Open to QA Automation roles">
  <img src="https://img.shields.io/badge/Based_in-Buenos_Aires,_AR-6E7681?style=flat" alt="Based in Buenos Aires">
</p>

## About me

I'm a **Senior QA Analyst** with almost 5 years of experience testing systems where bugs cost real money: core banking, multi-country remittances, and B2B telecom. Now I combine that judgment with **test automation** and **AI**.

- 🔍 **Now:** QA on the Salesforce B2B project for Telecom (Personal) at CFOTech. I led the QA team's move to AI agents in Jira for test design, bug reports, docs and log analysis. We went from **~5 test cases/hour to 20+ in minutes**.
- 💸 **Before:** Global66 (fintech, remittances across several countries), where I built Python + Selenium regression suites that ran before every release. Earlier, Banco Patagonia, where I tested core-banking flows on Bantotal and AS/400.
- 🤖 **Building:** Playwright + TypeScript suites with AI in the loop. The AI triages, summarizes and drafts tickets, and I set the rules for what it must never do.

## Featured projects

### 🎭 [Demo-Playwright](https://github.com/JuanEnzetti/Demo-Playwright) — AI-assisted QA pipeline

![TypeScript](https://img.shields.io/github/languages/top/JuanEnzetti/Demo-Playwright?style=flat&color=3178C6)
![Last commit](https://img.shields.io/github/last-commit/JuanEnzetti/Demo-Playwright?style=flat&color=6E7681)

An E2E suite for SauceDemo, plus a GitHub Actions pipeline where Claude reviews every pull request and turns test failures into decisions people can act on.

| Scope | Details |
|---|---|
| **24** E2E tests | Page Object Model, components, custom fixtures, typed test data |
| **3** CI jobs | AI code review on the diff → E2E run with HTML report → AI quality report on failure |
| **4** AI steps | Group failures by root cause → business summary → Jira ticket drafts → fix suggestions |
| **5** defects found | Real app bugs, documented while exploring before automating |

```mermaid
flowchart LR
    PR[Pull request] --> R[AI review of the diff<br/>flaky patterns, weak selectors]
    PR --> E[Playwright E2E<br/>24 tests]
    E -->|failures| G[Group by root cause]
    G --> S[Business summary]
    G --> T[Jira ticket drafts]
    G --> F[Fix suggestions]
    S & T & F --> L[Risk label + PR comment]
```

**Guardrails I wrote for the AI:** never "fix" a test to hide a real app bug; never raise timeouts as the only fix; prefer `getByRole` and `getByTestId`; a slow test gets reported, not healed. Tests are planned and generated with Playwright's planner, generator and healer agents through MCP.

### 🐍 [UI + API automation framework](https://github.com/JuanEnzetti/proyecto-final-automation-testing-Juan-Enzetti) — Python

![Python](https://img.shields.io/github/languages/top/JuanEnzetti/proyecto-final-automation-testing-Juan-Enzetti?style=flat&color=3776AB)
![Last commit](https://img.shields.io/github/last-commit/JuanEnzetti/proyecto-final-automation-testing-Juan-Enzetti?style=flat&color=6E7681)

Selenium + Pytest + Requests. It has Page Object Model, data-driven tests from JSON, parallel runs with `pytest-xdist`, retries for flaky tests, an HTML report and screenshots on every failure. It covers UI on SauceDemo and a REST API on Reqres.

## Tech stack

| Area | Tools |
|---|---|
| **Automation** | ![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat&logo=playwright&logoColor=white) ![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat&logo=selenium&logoColor=white) ![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=flat&logo=pytest&logoColor=white) ![Cucumber](https://img.shields.io/badge/BDD_·_Gherkin-23D96C?style=flat&logo=cucumber&logoColor=white) |
| **Languages** | ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black) ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white) |
| **AI for QA** | ![Claude](https://img.shields.io/badge/Claude_Code-D97757?style=flat&logo=anthropic&logoColor=white) ![MCP](https://img.shields.io/badge/Playwright_MCP-6E7681?style=flat) ![LLMs](https://img.shields.io/badge/LLMs_·_Prompt_Engineering-8250DF?style=flat) |
| **APIs & data** | ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat&logo=postman&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat&logo=mysql&logoColor=white) ![AS400](https://img.shields.io/badge/AS%2F400-054ADA?style=flat&logo=ibm&logoColor=white) |
| **CI/CD & cloud** | ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white) ![GitLab](https://img.shields.io/badge/GitLab-FC6D26?style=flat&logo=gitlab&logoColor=white) ![AWS](https://img.shields.io/badge/AWS_·_CloudWatch_·_CodePipeline-232F3E?style=flat&logo=amazonwebservices&logoColor=white) |
| **Performance & management** | ![JMeter](https://img.shields.io/badge/JMeter-D22128?style=flat&logo=apachejmeter&logoColor=white) ![Jira](https://img.shields.io/badge/Jira_·_Xray-0052CC?style=flat&logo=jira&logoColor=white) ![Confluence](https://img.shields.io/badge/Confluence-172B4D?style=flat&logo=confluence&logoColor=white) ![Salesforce](https://img.shields.io/badge/Salesforce-00A1E0?style=flat&logo=salesforce&logoColor=white) |

## GitHub stats

<!--
  These cards come from github-readme-stats. The public instance sometimes hits rate limits.
  If they stop loading, deploy your own copy on Vercel (one click from the project's README)
  and replace "github-readme-stats.vercel.app" with your own domain.
-->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=JuanEnzetti&show_icons=true&hide_border=true&hide_title=true&theme=github_dark&bg_color=00000000&include_all_commits=true">
    <img height="150" alt="GitHub stats" src="https://github-readme-stats.vercel.app/api?username=JuanEnzetti&show_icons=true&hide_border=true&hide_title=true&theme=default&bg_color=00000000&include_all_commits=true">
  </picture>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=JuanEnzetti&layout=compact&hide_border=true&hide_title=true&theme=github_dark&bg_color=00000000&langs_count=6">
    <img height="150" alt="Top languages" src="https://github-readme-stats.vercel.app/api/top-langs/?username=JuanEnzetti&layout=compact&hide_border=true&hide_title=true&theme=default&bg_color=00000000&langs_count=6">
  </picture>
</p>

## Let's talk

I'm looking for **QA Automation** roles in teams that treat quality as part of the product, not a gate at the end. Find me on [LinkedIn](https://www.linkedin.com/in/juanenzetti/) or by [email](mailto:juancruzenzetti@gmail.com).
