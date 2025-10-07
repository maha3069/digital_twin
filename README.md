# 🦾 Digital Twin — Mon Clone Numérique IA



https://github.com/user-attachments/assets/d3566936-0538-42f3-b241-c414e425342e


Un chatbot IA personnel qui connaît tout sur mon parcours (académique, professionnel, publications LinkedIn…) et répond à n’importe quelle question sur moi, comme un vrai assistant ou un jumeau numérique ! Déployé sur AWS avec une architecture serverless moderne.

## 🧩 Fonctionnalités

- Chatbot IA contextuel, basé sur mes infos LinkedIn, mon CV, mes expériences pro et mon parcours académique.
- Réponses conversationnelles à toutes les questions relatives à mon profil.
- Interface web moderne (Next.js + React), responsive et user-friendly.
- Possibilité d’évolution : ajout de rate-limiting, dashboards, personnalisation…


## 🚀 Architecture technique

L’architecture s’appuie entièrement sur AWS :

- **Frontend statique** (Next.js + React), hébergé et distribué mondialement via **Amazon CloudFront**.
- **API Gateway** pour la réception/routage des requêtes HTTP.
- **AWS Lambda** (hébergeant un backend FastAPI) pour la logique métier AI et l’orchestration.
- **Amazon S3** pour le stockage persistant (historique des conversations, fichiers annexes).
- Sécurité et scalabilité automatiques via les services managés AWS.

Envisagé prochainement : intégration d’un système de **rate limiting** pour contrôler le trafic sur l’API.

## 🛠️ Technologies principales

- **Backend** : Python, FastAPI (async, APIs sécurisées), hébergé via Lambda
- **Frontend** : Next.js, React
- **Infra** : AWS CloudFront, API Gateway, Lambda, S3
- **CI/CD** : Automatisé via GitHub Actions et AWS Amplify (optionnel)


## 💡 Comment ça marche ?

1. L’utilisateur arrive sur le site (contenu distribué par CloudFront).
2. Il pose ses questions via l’interface React.
3. La requête est routée par API Gateway et traitée par une fonction Lambda (FastAPI backend).
4. Le backend interroge les bases de connaissances personnalisées et retourne la réponse.
5. L’historique est stocké sur S3 pour personnalisation continue.



## 🔒 Sécurité \& Scalabilité

- Toutes les données sensibles sont sécurisées via IAM et policies AWS.
- Scalabilité automatique avec Lambda et CloudFront.
- Rate limiting à venir sur l’API FastAPI (cf. [fastapi-limiter](https://github.com/long2ice/fastapi-limiter) ou solutions Redis/S3).


## 📌 Roadmap/À venir

- Système avancé de rate limiting avant ouverture publique


## 🙋‍♀️ Pourquoi ce projet ?

Pour explorer la fusion IA, cloud et expérience utilisateur personnalisée, tout en valorisant mon parcours de manière interactive et automatisée !

***


<div align="center">⁂</div>
