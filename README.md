# SUNWISE TALENTS — Prospection commerciale multi-agents

Agents Claude qui préparent la prospection B2B de **SUNWISE TALENTS**, intégrateur
Salesforce transcontinental (France + Gabon) : ciblage, qualification, rédaction des
messages de prise de contact.

Ce dépôt **n'envoie rien**. L'agent rédige, Claudin envoie lui-même — aucun connecteur
email ou LinkedIn, aucun scraping, aucune écriture dans un CRM.

## Les agents

| # | Agent | Rôle | Déclencheurs typiques |
|---|---|---|---|
| — | [Orchestrateur](SKILL.md) | Cadre la campagne, délègue aux trois sous-agents, fait le point avec Claudin entre chaque étape | « lance une campagne de prospection » |
| 01 | [Ciblage](agents/01-ciblage/SKILL.md) | Traduit l'ICP en liste de prospects brute | « trouve-moi des prospects », « construis une liste » |
| 02 | [Qualification](agents/02-qualification/SKILL.md) | Enrichit, score (chaud/tiède/froid), tranche le segment, recommande preuve + angle | « qualifie », « score », « cherche les signaux » |
| 03 | [Rédaction](agents/03-redaction/SKILL.md) | Écrit les séquences email + LinkedIn par prospect qualifié | « rédige les messages », « écris la séquence » |

Chaque agent lit son propre `SKILL.md` en entier avant de travailler. Le détail du
fonctionnement, des garde-fous et de la chaîne de délégation est dans le
[`SKILL.md`](SKILL.md) racine.

## Le fil conducteur

Un fichier unique traverse les trois agents, chacun remplit sa couche sur le même bloc
prospect, sans écraser le travail du précédent :

```
à qualifier   →   qualifié   →   (rédigé)
     │
     └──────────→   écarté   (concurrent, client actuel, hors ICP)
```

- **01** écrit l'identité (entreprise, secteur, taille, géo, décideur, source) dans
  `output/prospects.md`.
- **02** enrichit la même ligne : segment, signaux datés, score, température, preuve,
  angle.
- **03** consomme la couche 02 et produit un fichier par prospect dans
  `output/messages/[entreprise].md` — il n'écrit pas dans `prospects.md`.

## Structure

```
SKILL.md                          Orchestrateur — point d'entrée du projet
shared/
├── icp.md                        Profil Client Idéal : qui cibler, signaux, scoring, exclusions
├── messaging-prospection.md      Angles, accroches, objections, preuves clients réelles
├── offres.md                     Les services SUNWISE (réutilisé de l'agent marketing)
└── personas.md                   P1 à P5 (réutilisé de l'agent marketing)
agents/
├── 01-ciblage/SKILL.md           Construit la liste brute
├── 02-qualification/SKILL.md     Score et enrichit
└── 03-redaction/SKILL.md         Rédige les messages
output/
├── prospects.md                  Le fil conducteur — jamais une source de vérité
└── messages/                     Un fichier par prospect, prêt à copier-coller
workflows/                        (vide à ce jour)
```

`output/` contient les productions, jamais des sources de vérité. La vérité est dans
`shared/` et dans les `SKILL.md` des agents.

## Garde-fous globaux

Appliqués par les trois sous-agents, sans exception :

- **Honnêteté des sources** — jamais de signal, chiffre ou donnée inventés ; un `?`
  vaut mieux qu'une invention.
- **Exclusions** — jamais les clients actuels (KLB, Lendys) ni les concurrents
  (autres intégrateurs Salesforce / ESN CRM) — voir `shared/icp.md` § 6.
- **Nommage client** — anonymisé par défaut (« un cabinet de conseil que nous
  accompagnons »). Nommer KLB / Lendys / Voulez-Vous uniquement si Claudin
  l'autorise explicitement.
- **RGPD** — uniquement des données professionnelles publiques ; rien de personnel
  ni de sensible.
- **Rédaction seule** — aucun envoi, aucune planification, aucune automatisation.

## Points d'arbitrage laissés à Claudin

Ces éléments affinent la qualité mais ne bloquent pas : en leur absence, l'agent
fonctionne en mode dégradé (anonymisation, pas de mention de prix).

| Point | Défaut sans réponse |
|---|---|
| Autorisation de nommer les références clients (KLB / Lendys / Voulez-Vous) | Rester anonymisé |
| Fourchettes de budget par type de mission | Ne pas mentionner de prix |
| Tailles réelles des clients existants | — |
| Secteurs à exclure explicitement | Aucun exclu au-delà de `icp.md` § 6 |

## Statut

`output/prospects.md` et `output/messages/` sont vides à ce jour — aucune campagne
lancée. `workflows/` est un dossier réservé, vide pour l'instant.
