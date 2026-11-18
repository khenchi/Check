# Check


Bonjour à tous,

Merci pour nos échanges lors de notre dernière réunion autour du Global Risk Dashboard.

Après la présentation de l'état actuel du dashboard et de l'approche 3s / 30s / 300s, nos discussions ont fait émerger une évolution importante du besoin initial.

Nous passons progressivement d'une logique de reporting et de visualisation à une logique de pilotage opérationnel, dans laquelle les utilisateurs pourraient non seulement consulter et analyser les indicateurs de risque, mais également intervenir sur certaines données, notamment lorsqu'une incohérence est identifiée.

Cette évolution soulève plusieurs sujets :

- Ajustement des données : possibilité de modifier certaines valeurs directement depuis l'interface ou via Excel, avec une répercussion cohérente sur les sous-totaux, les KPIs consolidés et les visualisations associées.
- Traçabilité et validation : nécessité de distinguer les données sources des ajustements, et de définir les droits de modification ainsi que les éventuels mécanismes de validation.
- Choix technologique : évaluation de plusieurs approches (Power BI, Streamlit/Python ou application web dédiée) en tenant compte des fonctionnalités attendues, de la facilité d'utilisation et de la maintenabilité.
- Déploiement et partage : étude de la possibilité d'héberger le dashboard sur un serveur commun, notamment en réutilisant l'infrastructure existante évoquée pendant la réunion.
- Coûts et industrialisation : comparaison des efforts de développement, des contraintes de mise en production et des coûts de maintenance à moyen et long terme.

Comme convenu, je vais approfondir la faisabilité de ces différentes options et préparer une analyse comparative accompagnée d'une recommandation, afin de faciliter le choix de l'architecture cible.

En parallèle, vos retours sur les cas d'usage prioritaires, notamment concernant les données à ajuster et les modalités de validation, permettront d'affiner cette analyse.

Bonne journée,



Bonjour à tous,

Suite à notre dernier échange avec le Head of Risk autour du Global Risk Dashboard, je souhaitais partager avec vous les principales évolutions évoquées et organiser un point ensemble afin d'évaluer les différentes options techniques avant de lui présenter une recommandation.

1. Évolution du besoin fonctionnel

Lors de la présentation de l'état actuel du dashboard et de l'approche 3s / 30s / 300s, un nouveau besoin a été soulevé : permettre aux utilisateurs de ne plus seulement consulter et analyser les indicateurs, mais également d'ajuster certaines valeurs identifiées comme incohérentes, directement depuis l'interface ou éventuellement via Excel.

Ces ajustements devraient pouvoir être répercutés sur les agrégats, les KPIs consolidés et les visualisations associées.

Nous passerions ainsi progressivement d'un outil de reporting et de visualisation vers un outil plus opérationnel, intégrant des fonctionnalités d'investigation, d'ajustement et potentiellement de validation des données de risque.

Cette évolution implique également de réfléchir à la traçabilité, aux droits d'édition et à la distinction entre données sources et données ajustées.

2. Solutions techniques envisagées

Plusieurs pistes méritent d'être étudiées :

- Power BI + Power Apps : permettrait de capitaliser sur l'écosystème Microsoft et les fonctionnalités de reporting existantes. En revanche, l'édition des données nécessite un mécanisme de write-back, avec des contraintes potentielles de synchronisation, de licences et de maintenance entre plusieurs composants.
- Streamlit + Python : solution flexible permettant de développer rapidement des fonctionnalités d'édition, de calcul et de visualisation. Elle présente un intérêt pour un POC, voire une solution de production sous réserve de répondre aux exigences de sécurité, de performance, de maintenabilité et de support.
- Application web dédiée (FastAPI + React, par exemple) : offrirait davantage de flexibilité pour les workflows complexes et une éventuelle industrialisation à grande échelle, au prix d'un effort de développement initial et de maintenance plus important.
- Power BI + Excel : approche potentiellement simple pour des ajustements ponctuels, mais nécessitant un processus de réimport, de validation et de synchronisation des données.

3. Déploiement et infrastructure

Nous avons également évoqué la possibilité de déployer le dashboard sur un serveur partagé afin de le rendre accessible aux différentes équipes.

Un serveur existant pourrait éventuellement être réutilisé, ce qui limiterait les investissements d'infrastructure. Il faudra toutefois vérifier sa disponibilité, ses caractéristiques et son adéquation avec les contraintes IT.

4. Points à approfondir ensemble

Je vous propose que nous échangions notamment sur :

- La faisabilité et les principales limitations de chaque approche.
- Les impacts en matière de développement, de maintenance et de support.
- Les contraintes de déploiement et de sécurité.
- Les coûts de développement, de licences et d'exploitation.
- La possibilité de réutiliser l'infrastructure existante.
- L'architecture la plus pertinente pour permettre une évolution progressive du dashboard.

L'objectif serait de confronter nos analyses et de construire une recommandation commune, en distinguant ce qui peut être validé rapidement dans un POC de ce qui nécessiterait une industrialisation plus poussée.

J'ai préparé un premier support de discussion que nous pourrons parcourir ensemble.

N'hésitez pas à partager vos remarques ou d'autres pistes qui vous sembleraient pertinentes.

Merci d'avance pour vos retours.

Bonne journée,
