# 🔐 DevSecOps – Sécurisation CI/CD avec GitLab, Trivy, GitLeaks, Snyk & Docker Bench

## 📌 Objectif du projet

Ce projet a pour but de mettre en œuvre un **pipeline CI/CD sécurisé** en intégrant des outils d’analyse de sécurité, conformément aux pratiques **DevSecOps**. Il inclut des scans de vulnérabilités dans le code, les dépendances, les images Docker, les secrets exposés, ainsi que l’audit des configurations.

---

## ⚙️ Outils utilisés

- **GitLab CI/CD** : Automatisation des tests, builds et déploiements.
- **Trivy** : Analyse de vulnérabilités dans les images Docker.
- **GitLeaks** : Détection de secrets dans les dépôts Git.
- **Snyk** : Scan des dépendances (SCA).
- **OWASP ZAP** : Analyse dynamique des applications web (DAST).
- **Docker Bench** : Audit de la configuration Docker.

---

## 🧱 Structure du projet



---

## 🚀 Étapes du pipeline CI/CD

1. **Détection de vulnérabilités dans les dépendances**  
   → via [Snyk](https://snyk.io)

2. **Scan des secrets dans les fichiers Git**  
   → via [GitLeaks](https://github.com/zricethezav/gitleaks)

3. **Analyse dynamique avec OWASP ZAP**  
   → Scanner l’application déployée automatiquement

4. **Scan de l’image Docker**  
   → via [Trivy](https://aquasecurity.github.io/trivy/)

5. **Audit de configuration Docker**  
   → via [Docker Bench Security](https://github.com/docker/docker-bench-security)

---

## 📊 Résultats attendus

- Pipeline DevSecOps automatisé.
- Détection des CVEs, secrets, et mauvaises configurations.
- Prévention de mise en production en cas de faille critique.
- Visualisation des logs et résultats dans GitLab CI/CD.

---

## 💡 Questions traitées

- **Différence entre Job et Stage** :
  - Job : tâche unique (test, build…)
  - Stage : groupe de jobs ordonnés

- **SAST vs DAST vs SCA** :
  - SAST : Analyse statique du code source
  - DAST : Test dynamique à l’exécution
  - SCA : Analyse des dépendances tierces

- **Pourquoi éviter le user root dans Docker ?**
  - Limiter la surface d’attaque en cas de compromission

---

## 📎 Liens utiles

- 🔗 Dépôt GitLab du projet : [WebApp Vulnerability Analysis](https://gitlab.com/wissal-boutayeb/WebAppVulnerabilityAnalysis.git)

---

## 🙋‍♀️ Réalisé par

**Wissal BOUTAYEB**  
Étudiante en Cybersécurité – Université Euromed de Fès
Encadré par : Pr. Ahmed Amamou



