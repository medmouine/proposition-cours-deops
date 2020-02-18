# Suggestion de cours
## De : Mohamed Mouine
## Présenté à : Mr. Luc Lamontagne



# Titre : ***Développement et opération de systèmes asynchrones distribués***

### Préalable : Qualité métrique du développement logiciel, Systèmes d'opération pour ingénieurs

## Objectif :
Le cours vise à donner aux étudiant-es les compétences et connaissances nécéssaires au développement, provisionnement et gestion de systèmes logiciels asynchrones distribués, cela dans un contexte de méthodologie Devops qui adopte et prend avantage des processus d'ingénieurie logiciel modernes.
## Plan de cours
### Semaine 1 : *Introduction au devops : Importance de la vélocité et la livraison au cœur du processus de développement*
- Notion et importance de vélocité
- Pipeline de livraison
- Importance des tests
- Agilité
- Devops

### Semaine 2 : *Tests automatisés : Du plus petit et au plus grand*
- UT
- IT/E2E
- TDD
- Load testing
- Autres (Arch tests, UI Tests)

### Semaine 3 : *Pipeline et automatisation*
- Rôle de l'automatisation
- Quoi automatisé
- Controle de version
- Pipeline d'automatisation

### Semaine 4 : *Architecture et design de systemes*
- Problèmes de couplage et de dette technique
- Diminuer et prévenir la dette
- Monolithe
- Distributed systems
- Bounded contexts
- Architecture Event based, Reactive, Event Sourcing, CQRS

### Semaine 5 : *Virtualisation et orchestration de base*
- 99% du code qu'on écrit pas
- Isolation de contextes
- Virtualisation et registre d'images
- Orchestration de systemes simplistes

### Semaine 6 : *Provisionnement et déploiement d'un systeme*
- Planification et prévision
- Intégration de nouvelles ressources
- Réseau et communication inter et intra systeme
- IaC et automatisation (Everything as Code)
- Serverless vs Serverful
- Cold start et graceful shutdown

### Semaine 7 : *Monitoring, Logging, tracing et maintenance*
- MaJ de version et configuration
- MaJ de systèmes et gestion de dépendances
- Troubleshooting de systèmes
- Importance du logging
- Minimiser le bruit, maximiser la pertinence
- Visualisation et analyse de journaux
- Tracing

### Semaine 8-9-10 : *Orchestration de systèmes distribués asynchrone complexes*
- Vélocité vs stabilité
- Gestion de risque
  - Load balancing
  - Auto restart
  - Healthcheck
- MaJ de systèmes complexes
  - Rollback
  - Blue/green (Black/white)
  - Feature flags
  - Canary deployment
- Connectivité et SecOps
- Service discovery
- Continuous Delivery

### Semaine 12 : *Cloud computing*
- Provideur cloud
- Integration de systèmes avec les providers
- Isolation des outils spécifique
### Semaine 13 : *Chaos Engineering et test en production*
- Notion de Dark Dept
- Planification d'un backlog hypothetique
- Expérience de chaos
- Automatisation du chaos
- Observabilité et analyse
- Intérvention humaine
- Continuous chaos

## Structure du cours

Le cours présente 1 examens de 30%.

4 Travaux pratiques. (plus de détails ci-bas)

5 Laboratoires de 1% chacun.

## Travaux pratiques
#### Travail 1 (10%): 
- Developpement d'un pipeline de test et de configuration automatisé pour un système pré-existant (À determiner : Github actions, CircleCI ou Jenkins (hosté sur les serveurs de l'université))

#### Travail 2 (20%):
- Orchestration d'un système pré-existant avec virtualisation (docker ou podman),Kubernetes/Openshift et minikube et gestion du réseau avec [Consul](https://consul.io)

#### Travail 3 (20%):
- Developpement d'un API Gateway en Golang utilisant [Consul](https://www.consul.io) et [Etcd](https://etcd.io/) pour le Service discovery pour router les services d'un cluster entre eux et avec des services hors du cluster

#### Travail 4 (15%): 
- Provisionnement et MaJ automatisé d'un système pre-existant sur plusieurs environnement avec Terraform [Terraform](https://terraform.io) et Ansible Playbook

### Exemple de systèmes :
![exemple1](https://github.com/medmouine/microservices-demo/raw/master/docs/img/architecture-diagram.png)

#### À noté que dans le cas de l'exemple ci-haut, l'architecture sera modifié pour supporté un API Gateway ainsi qu'une Queue pour le shippement.

![exemple2](https://github.com/dockersamples/example-voting-app/raw/master/architecture.png)