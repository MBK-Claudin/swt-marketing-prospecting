---
name: messaging-prospection
description: Bibliothèque de messaging prospection SUNWISE — angles, accroches email + LinkedIn, objections, preuves clients réelles (KLB, Lendys, Voulez-Vous), règles de personnalisation. Utilisé par l'agent 03-rédaction.
version: 2.0
maintainer: Claudin
---

# Messaging Prospection · SUNWISE TALENTS

> Utilisé par l'agent 03-rédaction. Le prospect arrive tagué Segment A ou B et
> scoré (voir [[icp]]). Ton et offres : [[personas]], [[offres]].

---

## 0. Principes non négociables
- **Une douleur, pas un catalogue.** Un message = un problème du prospect + une
  preuve qu'on sait le résoudre.
- **Le signal d'abord.** Ouvrir sur l'élément détecté par l'agent 02 (leur
  recrutement, leur org SF, leur e-commerce non intégré). Jamais « J'espère que
  vous allez bien ».
- **Court.** Email < 120 mots. Note LinkedIn < 300 caractères.
- **Un seul CTA** : un échange de 15 min.
- **Zéro jargon pour le Segment A.** Apex/LWC/org réservés au Segment B.
- **Français impeccable, ton pair-à-pair.** Ni servile, ni arrogant.
- **La preuve avant la promesse.** SUNWISE a des réalisations concrètes (§3) —
  les citer bat toute affirmation vague.

---

## 1. Banque de preuves (le capital crédibilité)

> À injecter dans les messages selon le besoin du prospect. Chaque preuve = un
> résultat réel, pas un argument marketing. **Vérifier avec Claudin avant de
> nommer un client** ; sinon anonymiser (« un cabinet de conseil que nous
> accompagnons »).

| Besoin du prospect | Preuve SUNWISE | Formulation anonymisée prête à l'emploi |
|---|---|---|
| Reporting fin, proche d'Excel | Tableau croisé dynamique + export Excel stylé (Lendys) | « un tableau de bord aussi souple qu'Excel, directement dans Salesforce, avec export mis en forme » |
| Piloter consultants / staffing | Module de gestion des disponibilités (Lendys) | « un module de suivi des disponibilités et d'affectation des consultants » |
| Projection / simulation financière | Moteur de projection financière (Lendys) | « un moteur de simulation CA / masse salariale / résultat, comparant réel et projeté » |
| Org ancienne, dette technique | Audit technique, 122 classes Apex analysées (Lendys) | « un audit technique complet de votre org avec plan de remédiation priorisé » |
| Manque de ressources SF | TMA, incidents de prod résolus (Lendys) | « une équipe certifiée qui reprend et fiabilise votre org en TMA » |
| Portail externe (partenaires, candidats) | Formulaire sous-traitants Experience Cloud (Lendys) | « un portail externe sécurisé sans licence Salesforce pour vos partenaires » |
| Signature électronique | Intégration Adobe Acrobat Sign (Lendys) | « la signature électronique intégrée directement dans vos process Salesforce » |
| Relations entre contacts / décideurs | Organigramme de contacts interactif LWC + D3 (Lendys) | « une cartographie visuelle des décideurs et influenceurs de vos comptes » |
| E-commerce non connecté au CRM | Intégration Salesforce ↔ PrestaShop (Voulez-Vous) | « la synchronisation automatique de votre boutique en ligne avec votre CRM » |
| Trop de saisie manuelle | Automatisation Flows, relances, tâches (Voulez-Vous) | « l'automatisation de vos relances et tâches commerciales » |
| Doublons / mauvaise qualité de données | Dédoublonnage + règles de validation (Voulez-Vous) | « le nettoyage et la fiabilisation de votre base clients » |

---

## 2. Les angles (le « pourquoi maintenant »)

### Segment A — Numérisation
- **A1 · La croissance qui casse les outils** : « Vous grandissez, Excel ne suit
  plus. »
- **A2 · Le coût caché du désordre** : temps perdu, doublons, pas de visibilité.
- **A3 · Structurer avant d'investir** : diagnostic à faible engagement en porte
  d'entrée.
- **A4 · Connecter l'existant** (fort pour l'e-commerce) : « Votre boutique en
  ligne et votre suivi client vivent séparément — on les réunit. » Preuve :
  Voulez-Vous / PrestaShop.

### Segment B — Org Salesforce existante
- **B1 · L'org sous-exploitée** : « Vous payez des licences utilisées à 30 %. »
- **B2 · La dette technique** : org ancienne, fragile. Preuve : audit Lendys.
- **B3 · Le manque de bras** (déclenché par offre d'emploi Salesforce) : « Le
  recrutement SF est long — nos experts prennent le relais dès maintenant. »
- **B4 · La migration / montée de version** : Classic → Lightning.
- **B5 · Reprise d'un projet en souffrance** (sans juger le prestataire précédent).
- **B6 · Le besoin métier précis** (le plus puissant pour un cabinet conseil) :
  reporting, staffing, projection financière, portail. Preuves : Lendys.

---

## 3. Accroches EMAIL (gabarits à personnaliser)

> Remplacer chaque [crochet]. Ne jamais envoyer un gabarit brut : injecter le
> signal réel + la preuve la plus proche.

**Segment B — cabinet de conseil (cœur de cible), angle B6**
> Objet : [Entreprise] · piloter l'activité de vos consultants dans Salesforce
> Bonjour [Prénom], en tant que cabinet [de conseil/d'audit], vous jonglez sans
> doute entre staffing, rentabilité et reporting. Nous accompagnons des cabinets
> comparables au vôtre sur exactement ces sujets dans Salesforce — suivi des
> disponibilités consultants, tableaux de bord souples, projection financière.
> Ouvert à 15 min pour voir ce qui s'appliquerait chez vous ?

**Segment B — offre d'emploi Salesforce, angle B3**
> Objet : [Entreprise] · votre recherche [poste Salesforce]
> Bonjour [Prénom], j'ai vu que vous recrutez un·e [poste]. Le recrutement
> Salesforce prend du temps — en attendant, nos experts certifiés maintiennent et
> font avancer votre org dès maintenant (dev, TMA, optimisation). On l'a fait pour
> un cabinet dont on a repris et fiabilisé toute l'org. 15 min cette semaine ?

**Segment B — dette technique / org ancienne, angle B2**
> Objet : [Entreprise] · votre org Salesforce vieillit-elle bien ?
> Bonjour [Prénom], après quelques années, une org Salesforce accumule souvent de
> la dette : classes non testées, flows en conflit, incidents en cascade. Nous
> réalisons des audits techniques complets (récemment : 122 classes analysées,
> plan de remédiation priorisé). Curieux de savoir où en est la vôtre — 15 min ?

**Segment A — e-commerce non intégré, angle A4**
> Objet : [Entreprise] · votre boutique et votre CRM se parlent-ils ?
> Bonjour [Prénom], quand la boutique en ligne et le suivi client vivent chacun de
> leur côté, on perd du temps et on multiplie les doublons. Nous avons connecté
> une plateforme e-commerce (PrestaShop) à Salesforce en synchro bidirectionnelle
> — commandes, clients, statuts, le tout automatisé. 15 min pour voir si c'est
> votre cas ?

**Relance 1 (J+3/4, même fil)** : apporter de la valeur, pas « je relance » — un
mini-constat sectoriel ou un cas concret.
**Relance 2 (J+7/10)** : soft, porte de sortie (« Si ce n'est pas le moment,
dites-le-moi, je n'insiste pas »).

---

## 4. Accroches LINKEDIN

**Note de connexion (< 300 car.)** — pas de pitch :
> Bonjour [Prénom], je vois [signal, ex. votre actualité / votre poste chez un
> cabinet de conseil]. Chez SUNWISE nous accompagnons les cabinets sur Salesforce
> (pilotage, reporting, TMA). Ravi d'échanger.

**Message post-acceptation (J+1/2)** : remercier, une phrase de valeur liée au
signal + preuve anonymisée, CTA léger.
> Merci d'avoir accepté [Prénom]. On a récemment doté un cabinet de conseil d'un
> module de suivi des disponibilités consultants et de tableaux de bord souples
> dans Salesforce. Curieux de savoir comment vous gérez ça aujourd'hui — 15 min ?

---

## 5. Traitement des objections

| Objection | Réponse |
|---|---|
| « On a déjà un prestataire » | Ne pas dénigrer. « Parfait. On intervient souvent en complément sur des expertises pointues (dev LWC, audit, intégration). Gardons le contact. » |
| « Pas le budget / pas maintenant » | Baisser l'engagement : diagnostic court ou audit. « Quand serait le bon moment pour en reparler ? » |
| « On gère en interne » | Valoriser l'interne, se positionner en renfort sur pics de charge / expertise pointue / audit externe. |
| « Salesforce trop cher/gros pour nous » (Seg. A) | Recentrer sur le besoin : « L'idée n'est pas de vous vendre Salesforce mais de structurer votre activité — on choisit l'outil adapté à votre taille. » |
| « C'est quoi SUNWISE, jamais entendu » | Preuve rapide : certifs, réalisations concrètes (audit 122 classes, intégrations Adobe Sign / PrestaShop, Experience Cloud), double ancrage France/Afrique. |
| « Vous connaissez notre métier ? » (cabinet) | Fort : « Oui — nous accompagnons des cabinets de conseil sur le staffing, la rentabilité, la projection financière et le reporting dans Salesforce. » |
| « Envoyez une doc » (esquive) | Accepter mais accrocher : « Je vous envoie ça et je vous propose 15 min pour la contextualiser à votre cas. » |
| Silence total | Relance 2 max, puis nurturing. Jamais harceler. |

---

## 6. Règles de personnalisation (agent 03)
1. Ouvrir sur le signal réel du prospect (jamais générique).
2. Adapter le vocabulaire au segment (A = métier/business, B = technique Salesforce).
3. Un seul angle par message.
4. **Injecter la preuve la plus proche du besoin** (§1) — anonymisée par défaut,
   nommée seulement si Claudin l'a autorisé.
5. Un seul CTA, daté si possible.
6. Longueur : email < 120 mots, note LinkedIn < 300 car.
7. Signature homogène (SUNWISE, fonction, double ancrage France/Gabon).

---

## 7. À compléter par Claudin
- **Autorisation de nommer** KLB / Lendys / Voulez-Vous (sinon rester anonymisé).
- Cas clients supplémentaires pour élargir la banque de preuves.
- Fourchettes de prix / format du diagnostic ou de l'audit d'entrée.
- Signature-type et coordonnées.
- Ton exact validé (croiser avec [[personas]] de l'agent 1).