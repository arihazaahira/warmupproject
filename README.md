# 🔥 Générateur Automatique de Plan de Warm-Up Email

## 📌 Contexte

La création manuelle d’un plan de warm-up pour les adresses IP ou domaines d’envoi prend du temps et demande une adaptation selon :
- l’audience totale,
- le nombre de semaines,
- le nombre de jours d’envoi,
- les fournisseurs d’accès (ESPs) ciblés,
- et la logique de progression.

🎯 Pour gagner en efficacité et éviter les erreurs, nous avons développé une solution permettant de **générer automatiquement un plan de warm-up personnalisé**, selon différents scénarios.

---

## 🧠 Objectifs du Projet

- Automatiser la création des plans de warm-up IP/email.
- Réduire le temps passé à les concevoir manuellement.
- Proposer un outil simple et intuitif, utilisable même sans expertise technique.
- S’adapter à différentes configurations d’utilisateur.

---

## 📋 Fonctionnement

L'utilisateur renseigne :
- L’audience totale.
- La liste des ESPs (Gmail, Outlook…).
- Les volumes par ESP *(optionnel)*.
- Le nombre de semaines ou de jours *(optionnel)*.
- Le taux de progression *(ex. 1.3%)*.

La solution calcule alors :
- Le nombre de semaines nécessaires si non précisé.
- Un plan hebdomadaire, avec un volume quotidien progressif.
- Une répartition équitable par jour et par ESP.

---

## ✅ Cas pris en charge (V1)

### 🔹 Cas principal :
> L’utilisateur connaît les ESPs.

#### Sous-cas :
- Il connaît les **volumes par ESP** et le **nombre de semaines** + **nombre de jours par semaine**.
- Il connaît les **volumes par ESP** et **le nombre de semaines uniquement**.
- Il connaît les **volumes par ESP** et **le nombre de jours uniquement**.
- Il **ne connaît ni les jours ni les semaines**, seulement les volumes et les ESPs → estimation automatique.

---

## 🛠️ Fonctionnalités Clés

- Formulaire dynamique (multi-étapes).
- Calcul automatique des volumes par jour.
- Dernière semaine à volume maximal quotidien.
- Répartition constante par jour dans chaque semaine.
- Téléchargement du plan final.

---

## 🔄 Améliorations futures (V2)

- **Gestion du cas où l’utilisateur ne connaît pas les ESPs** :
  - Utilisation de répartitions par défaut (basées sur le marché).
  - Possibilité de cibler des catégories d’ESPs (B2B, B2C…).
- **Personnalisation avancée** :
  - En fonction des taux d’engagement.
  - Ajout de plages horaires d’envoi.
- **Intégration SFMC** (Marketing Cloud) :
  - Export direct vers une Journey ou Sendable Data Extension.
- **Interface UX améliorée** :
  - Résumé clair, suggestions en temps réel, mobile-friendly.

---



