# ANNEXE 2 : POLITIQUE DE CONFIDENTIALITÉ

**Plateforme** : Safe Space  
**Responsable de traitement** : Alix VEYRAT  
**Adresse email** : alixveyrat@gmail.com  
**Date d'entrée en vigueur** : 30/10/2025  
**Dernière mise à jour** : 30/10/2025

---

## 1. INTRODUCTION

Bienvenue sur **Safe Space**, une plateforme dédiée à l'accompagnement des victimes et témoins de violences au travail.

La protection de vos données personnelles est notre **priorité absolue**. Cette Politique de Confidentialité explique :
- Quelles données nous collectons
- Pourquoi nous les collectons
- Comment nous les protégeons
- Vos droits sur vos données

**Important** : Safe Space traite des **données sensibles** (témoignages de violences révélant santé, opinions, orientations). Nous appliquons les mesures de sécurité les plus strictes conformément au RGPD.

---

## 2. RESPONSABLE DE TRAITEMENT

**Identité** : Alix VEYRAT  
**Qualité** : Créateur et responsable de Safe Space  
**Contact** : alixveyrat@gmail.com  

<<<<<<< HEAD
**Délégué à la Protection des Données (DPO)** : alixveyrat@gmail.com  
*Note : Pour un projet de cette envergure, un DPO externe sera nommé avant mise en production.*
=======
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb

---

## 3. DONNÉES COLLECTÉES ET FINALITÉS

### 3.1. Formulaire de Collecte de Données (Sprint 0)

**Finalité** : Entraîner notre intelligence artificielle à classifier les témoignages de violences.

**Données collectées** :
- ✅ **Témoignage textuel** (description des faits)
- ✅ **Catégorie de violence** (harcèlement, discrimination, etc.)
- ✅ **Contexte** (secteur d'activité, ancienneté, taille entreprise)
- ✅ **Données démographiques** (facultatives : région, âge, genre)

**Base juridique** : Consentement explicite (Article 6.1.a et 9.2.a RGPD)

**Mesures de protection** :
- ❌ **Aucune donnée identifiante** collectée (pas de nom, email, IP)
- ✅ **Anonymisation automatique** (suppression noms, entreprises, lieux)
- ✅ **Stockage sécurisé** (Google Sheets avec accès restreint, chiffrement)

**Durée de conservation** : 3 ans (amélioration continue IA)

<<<<<<< HEAD
---

### 3.2. Comptes Utilisateurs (Plateforme)

**Finalité** : Authentification et gestion des accès.

**Données collectées** :
- ✅ **Email** (ou pseudonyme anonyme si option choisie)
- ✅ **Mot de passe** (haché avec BCrypt, jamais stocké en clair)
- ✅ **Rôle** (Victime, Témoin, Modérateur, Admin)
- ✅ **Dates** (création compte, dernière connexion)
- ✅ **Logs techniques** (IP, User-Agent) conservés 6 mois max

**Base juridique** : Exécution du contrat (Article 6.1.b RGPD)

**Option anonymat** :
- ✅ Vous pouvez créer un **compte anonyme** (pseudonyme auto-généré, pas d'email)
- ✅ Votre identité reste **protégée** en toutes circonstances

**Durée de conservation** : Tant que compte actif. Suppression immédiate sur demande.

---

### 3.3. Signalements de Violences

**Finalité** : Permettre aux victimes de signaler et obtenir une qualification juridique.

**Données collectées** :
- ✅ **Description des faits** (texte chiffré AES-256)
- ✅ **Date des faits**
- ✅ **Qualification IA** (catégorie, articles de loi, niveau de gravité)
- ✅ **Réponses aux questions** (formulaire adaptatif)

**Base juridique** :
- Article 6.1.b RGPD (exécution du contrat)
- Article 9.2.f RGPD (défense de droits en justice)
- Article 9.2.a RGPD (consentement pour données sensibles)

**Mesures de protection** :
- ✅ **Chiffrement end-to-end** (AES-256-GCM avec clés uniques)
- ✅ **Anonymisation** automatique (suppression entités nommées)
- ✅ **Horodatage certifié** (valeur légale RFC 3161)
- ✅ **Audit logs** (traçabilité complète des accès)

**Durée de conservation** : 6 ans (prescription pénale). Suppression immédiate sur demande.

---

### 3.4. Coffre-Fort de Preuves

**Finalité** : Stocker vos preuves (documents, photos, enregistrements) de manière sécurisée.

**Données collectées** :
- ✅ **Fichiers chiffrés** (documents, images, audio, vidéo)
- ✅ **Métadonnées** (date, hash SHA-256, timestamp certifié)
- ✅ **Tags** (catégorisation personnelle)

**Base juridique** : Article 9.2.f RGPD (défense de droits en justice)

**Mesures de protection** :
- ✅ **Chiffrement AES-256-GCM** avec clés uniques (KMS)
- ✅ **Horodatage certifié** (preuve légale date d'existence)
- ✅ **Watermarking invisible** (traçabilité en cas de fuite)
- ✅ **Rate limiting** (10 téléchargements/heure max)

**⚠️ Avertissement légal** :
- Les enregistrements audio/vidéo sans consentement sont illégaux (Article 226-1 Code pénal)
- Un avertissement obligatoire s'affiche avant tout upload audio/vidéo

**Durée de conservation** : Tant que vous le souhaitez (max 10 ans). Suppression immédiate sur demande.

---

### 3.5. Collaboration Témoins → Victimes

**Finalité** : Permettre aux témoins de proposer leurs preuves aux victimes (sans délation forcée).

**Données collectées** :
- ✅ **Preuves témoins** (chiffrées)
- ✅ **Code de partage** (SAFE-XXXX, expire 30 jours)
- ✅ **Statut** (en attente, accepté, décliné)

**Anonymat garanti** :
- ✅ Le témoin reste **anonyme** vis-à-vis de la victime (pas d'email, pas de nom)
- ✅ La victime voit "Témoin anonyme"
- ✅ Option : Témoin peut révéler identité volontairement (optionnel)

**Base juridique** : Article 6.1.f RGPD (intérêt légitime : aide aux victimes)

**Durée de conservation** : Jusqu'à acceptation/déclinaison ou expiration code (30 jours)

---

### 3.6. Géolocalisation des Ressources

**Finalité** : Vous orienter vers ressources d'aide (avocats, associations, psychologues).

**Données collectées** :
- ✅ **Localisation temporaire** (GPS, non stockée, calcul temps réel uniquement)
- ✅ **Ville/Département** (pour recherche, facultatif)

**Base juridique** : Consentement (permission navigateur) + Intérêt légitime (aide)

**Mesures de protection** :
- ✅ **Pas de stockage** de votre position GPS
- ✅ Demande **permission** navigateur
- ✅ Historique recherches **anonymisé** (1 an max)

**Durée de conservation** : Aucune (calcul éphémère)

---

### 3.7. Modération

**Finalité** : Valider signalements, détecter cas critiques, améliorer IA.

**Données collectées** :
- ✅ **Signalements en attente**
- ✅ **Corrections catégorisation IA**
- ✅ **Détection mots-clés critiques** (viol, suicide, menaces)

**Base juridique** : Article 6.1.f RGPD (intérêt légitime : sécurité)

**Accès restreint** :
- ✅ Équipe modération uniquement (professionnels formés psycho-trauma)
- ✅ Logs d'actions traçables

**Cas critiques** :
- ⚠️ Si danger imminent détecté (viol, suicide, menaces), autorités peuvent être alertées

**Durée de conservation** : 3 ans (amélioration IA)

---

=======
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb
## 4. DESTINATAIRES DES DONNÉES

### 4.1. Accès internes

**Équipe Safe Space** :
<<<<<<< HEAD
- Développeurs (maintenance technique, accès limité)
- Modérateurs (validation signalements, formés psycho-trauma)
- Support technique (assistance utilisateurs)

**Accès strictement limité** au minimum nécessaire.

---

### 4.2. Partage avec tiers (UNIQUEMENT avec consentement ou réquisition)

**Vous décidez** avec qui partager vos données :

✅ **Avocats** : Vous pouvez partager votre dossier (signalement + preuves)  
✅ **RH entreprise** : UNIQUEMENT si vous donnez consentement explicite  
✅ **Associations d'aide** : Si vous le souhaitez  
✅ **Autorités judiciaires** : UNIQUEMENT sur réquisition judiciaire officielle

❌ **Aucun partage commercial** (vente, location, marketing)

---

### 4.3. Sous-traitants

**Hébergeur** : OVH, Scaleway ou Heroku (Union Européenne uniquement)  
**Certifications** : ISO 27001, HDS (Hébergeur Données de Santé)  
**Contrat** : DPA (Data Processing Agreement) signé, conformité RGPD

**Service IA** : Modèle auto-hébergé (aucun transfert externe)  
*Note : Si utilisation future d'API LLM (OpenAI, Anthropic), DPA signé*

---

## 5. TRANSFERTS HORS UNION EUROPÉENNE

❌ **Aucun transfert** de données hors Union Européenne.

Tous nos serveurs sont situés en **France ou UE**.

Si transfert futur nécessaire, nous appliquerons les **Clauses Contractuelles Types** de la Commission Européenne.

---

## 6. DURÉE DE CONSERVATION
=======
- Alix VEYRAT


**Accès strictement limité** au minimum nécessaire.

## 5. DURÉE DE CONSERVATION
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb

| Donnée | Durée | Justification |
|--------|-------|---------------|
| **Formulaire collecte IA** | 3 ans | Amélioration continue modèle |
<<<<<<< HEAD
| **Compte utilisateur** | Tant que actif | Exécution contrat |
| **Signalements** | 6 ans | Prescription pénale |
| **Preuves coffre-fort** | À votre convenance (max 10 ans) | Prescription civile |
| **Logs connexion** | 6 mois | Sécurité |
| **Historique modération** | 3 ans | Audit |

**Suppression sur demande** : Immédiate (sauf si procédure judiciaire en cours)

---

## 7. SÉCURITÉ DES DONNÉES

Nous mettons en œuvre les mesures techniques et organisationnelles les plus strictes :

### 7.1. Mesures techniques

✅ **Chiffrement** :
- AES-256-GCM (fichiers, signalements)
- BCrypt cost 12 (mots de passe)
- TLS 1.3 (transit)

✅ **Authentification** :
- JWT avec refresh tokens courts (15min)
- 2FA optionnelle
- Rate limiting (protection attaques brute-force)

✅ **Intégrité** :
- Hash SHA-256 (preuves)
- Horodatage certifié RFC 3161 (valeur légale)
- Watermarking invisible (traçabilité)

✅ **Monitoring** :
- Détection activité suspecte (volume, géolocalisation)
- Audit logs complets (qui, quoi, quand, pourquoi)
- Alertes automatiques (tentatives intrusion)

---

### 7.2. Mesures organisationnelles

✅ **Accès restreints** :
- Principe du moindre privilège (RBAC strict)
- Authentification forte (2FA équipe)
- Logs d'actions traçables

✅ **Formation** :
- Équipe formée RGPD
- Modérateurs formés psycho-trauma
- Sensibilisation sécurité continue

✅ **Procédures** :
- Plan de réponse incidents (data breach < 72h CNIL)
- Sauvegardes chiffrées quotidiennes
- Tests d'intrusion réguliers (avant production)

✅ **Conformité** :
- Analyses d'impact (DPIA) réalisées
- Registre des traitements à jour
- Contrats DPA avec sous-traitants

---

## 8. VOS DROITS (RGPD)

Conformément au RGPD, vous disposez des droits suivants :

### 8.1. Droit d'accès (Article 15)
=======

---

## 6. VOS DROITS (RGPD)

Conformément au RGPD, vous disposez des droits suivants :

### 6.1. Droit d'accès (Article 15)
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb
Vous pouvez obtenir une copie de toutes vos données.

**Comment** : Email à alixveyrat@gmail.com avec justificatif identité  
**Délai** : Réponse sous 1 mois

---

<<<<<<< HEAD
### 8.2. Droit de rectification (Article 16)
=======
### 6.2. Droit de rectification (Article 16)
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb
Vous pouvez corriger vos données inexactes.

**Comment** : Modification profil ou email à alixveyrat@gmail.com  
**Délai** : Correction immédiate ou sous 1 mois

---

<<<<<<< HEAD
### 8.3. Droit à l'effacement (Article 17)
=======
### 6.3. Droit à l'effacement (Article 17)
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb
Vous pouvez demander la suppression de vos données.

**Comment** : Suppression compte (bouton dans profil) ou email  
**Délai** : Suppression immédiate (sauf procédure judiciaire en cours)

**⚠️ Limitation** : Si dossier utilisé en justice, conservation nécessaire jusqu'à fin procédure

---

<<<<<<< HEAD
### 8.4. Droit d'opposition (Article 21)
=======
### 6.4. Droit d'opposition (Article 21)
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb
Vous pouvez vous opposer au traitement de vos données.

**Comment** : Email à alixveyrat@gmail.com  
**Délai** : Réponse sous 1 mois

**⚠️ Limitation** : Si traitement nécessaire défense droits en justice

---

<<<<<<< HEAD
### 8.5. Droit à la portabilité (Article 20)
=======
### 6.5. Droit à la portabilité (Article 20)
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb
Vous pouvez récupérer vos données dans un format structuré (JSON, CSV).

**Comment** : Email à alixveyrat@gmail.com  
**Délai** : Export sous 1 mois

---

<<<<<<< HEAD
### 8.6. Droit de limitation (Article 18)
=======
### 6.6. Droit de limitation (Article 18)
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb
Vous pouvez demander un gel temporaire du traitement.

**Comment** : Email à alixveyrat@gmail.com  
**Délai** : Réponse sous 1 mois

---

<<<<<<< HEAD
### 8.7. Droit de retirer le consentement (Article 7.3)
=======
### 6.7. Droit de retirer le consentement (Article 7.3)
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb
Vous pouvez retirer votre consentement à tout moment (formulaire collecte IA).

**Comment** : Email à alixveyrat@gmail.com  
**Effet** : Suppression immédiate de vos données du dataset

---

<<<<<<< HEAD
### 8.8. Droit d'introduire une réclamation (Article 77)
=======
### 6.8. Droit d'introduire une réclamation (Article 77)
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb
Vous pouvez déposer une plainte auprès de la CNIL.

**CNIL** :  
3 Place de Fontenoy  
TSA 80715  
75334 PARIS CEDEX 07  
Téléphone : 01 53 73 22 22  
Site web : https://www.cnil.fr

---

<<<<<<< HEAD
## 9. COOKIES ET TECHNOLOGIES SIMILAIRES

### 9.1. Cookies essentiels (non désactivables)

- **Session JWT** : Authentification (expire 15min)
- **Préférences** : Langue, thème

**Base juridique** : Intérêt légitime (fonctionnement service)

---

### 9.2. Cookies analytiques (désactivables)

❌ **Pas de Google Analytics** ni outils tracking tiers

✅ **Analytics respectueux vie privée** (si implémenté) :
- Matomo auto-hébergé (UE uniquement)
- Anonymisation IP
- Pas de partage données
- Opt-out possible

---

### 9.3. Gestion cookies

**Comment refuser** : Paramètres navigateur  
**Firefox** : Préférences → Vie privée → Cookies  
**Chrome** : Paramètres → Confidentialité → Cookies  
**Safari** : Préférences → Confidentialité → Cookies

---

## 10. MINEURS

Safe Space est destiné aux **personnes majeures** (18 ans et plus).
=======
## 7. MINEURS

LE formulaire de Safe Space est destiné aux **personnes majeures** (18 ans et plus).
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb

Si vous avez moins de 18 ans et êtes victime de violences :
- ☎️ **3919** (numéro national violence)
- ☎️ **119** (Allô Enfance en Danger)
- ☎️ **17** (Police Secours)

Nous ne collectons **pas sciemment** de données de mineurs. Si nous en sommes informés, suppression immédiate.

---

<<<<<<< HEAD
## 11. MODIFICATIONS DE LA POLITIQUE
=======
## 8. MODIFICATIONS DE LA POLITIQUE
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb

Cette Politique peut être mise à jour pour refléter :
- Évolutions légales (RGPD, ePrivacy)
- Nouvelles fonctionnalités
- Améliorations sécurité

<<<<<<< HEAD
**Notification** : Toute modification substantielle vous sera notifiée par email (ou bannière plateforme).

=======
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb
**Historique** :
| Date | Version | Modifications |
|------|---------|---------------|
| 30/10/2025 | 1.0 | Création initiale |

---

<<<<<<< HEAD
## 12. CONTACT ET QUESTIONS
=======
## 9. CONTACT ET QUESTIONS
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb

**Pour toute question** sur cette Politique ou vos données :

📧 **Email** : alixveyrat@gmail.com  
**Objet** : [RGPD] Votre question  
**Délai de réponse** : 1 mois maximum

**DPO (avant production)** : Un Délégué à la Protection des Données externe sera nommé.

---

<<<<<<< HEAD
## 13. ENGAGEMENT SAFE SPACE
=======
## 10. ENGAGEMENT SAFE SPACE
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb

**Notre promesse** :

✅ **Transparence totale** sur l'usage de vos données  
✅ **Sécurité maximale** (chiffrement, anonymisation)  
✅ **Respect absolu** de vos droits (suppression immédiate sur demande)  
✅ **Aucun usage commercial** (pas de vente, pas de pub)  
✅ **Éthique** : Votre bien-être avant tout

**Safe Space est un projet Tech for Good**. Nous existons pour vous aider, pas pour exploiter vos données.

---

<<<<<<< HEAD
## 14. RESSOURCES UTILES
=======
## 11. RESSOURCES UTILES
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb

**Aide d'urgence** :
- ☎️ **3919** - Violence Femmes Info (24/7, gratuit, anonyme)
- ☎️ **17** - Police Secours
- ☎️ **15** - SAMU
- ☎️ **114** - Urgence SMS (sourds, malentendants)

**Associations** :
- AVFT (Association européenne contre les Violences faites aux Femmes au Travail)
- Défenseur des droits
- Stop Harcèlement

**Informations RGPD** :
- CNIL : https://www.cnil.fr
- UE RGPD : https://ec.europa.eu/info/law/law-topic/data-protection

---

**Merci de votre confiance. Ensemble, pour un monde du travail plus sûr. 💙**

---

**Document établi conformément aux articles 12, 13 et 14 du RGPD**  
**Responsable** : Alix VEYRAT  
**Contact** : alixveyrat@gmail.com  
**Date** : 30/10/2025
