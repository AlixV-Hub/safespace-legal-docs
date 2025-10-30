# ANNEXE 1 : REGISTRE DES TRAITEMENTS DE DONNÉES

**Organisme** : Safe Space  
**Responsable de traitement** : Alix VEYRAT  
**Contact DPO** : alixveyrat@gmail.com  
**Date de création** : 30/10/2025  
**Dernière mise à jour** : 30/10/2025

---

## Conformité RGPD

Ce registre est établi conformément à l'article 30 du Règlement Général sur la Protection des Données (RGPD - UE 2016/679).

---

<<<<<<< HEAD
## TABLE DES MATIÈRES

1. [Traitement 1 : Collecte de données pour entraînement IA](#traitement-1)
2. [Traitement 2 : Gestion des comptes utilisateurs](#traitement-2)
3. [Traitement 3 : Traitement des signalements](#traitement-3)
4. [Traitement 4 : Gestion du coffre-fort de preuves](#traitement-4)
5. [Traitement 5 : Modération des contenus](#traitement-5)
6. [Traitement 6 : Géolocalisation des ressources](#traitement-6)

---

=======
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb
## TRAITEMENT 1 : Collecte de données pour entraînement IA {#traitement-1}

### Finalité
Constituer un dataset d'entraînement pour le modèle de classification automatique des témoignages de violences au travail.

### Base juridique
- **Article 6.1.a RGPD** : Consentement explicite
- **Article 9.2.a RGPD** : Consentement explicite pour données sensibles (santé, opinions, orientation sexuelle révélées par témoignages)

### Catégories de données collectées
- **Données obligatoires** :
  - Témoignage textuel (description de faits de violence)
  - Catégorie de violence (harcèlement moral, sexuel, discrimination, etc.)
<<<<<<< HEAD
  - Contexte (secteur d'activité, ancienneté, taille entreprise)
  
- **Données facultatives** :
  - Région géographique (niveau département, pas de ville)
  - Tranche d'âge (18-25, 26-35, etc.)
  - Genre ressenti
=======
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb

### Catégories de personnes concernées
- Victimes de violences au travail
- Témoins de violences au travail
- Contributeurs volontaires

### Destinataires des données
- **Internes** : Équipe développement Safe Space (accès restreint)
- **Externes** : Aucun (données strictement confidentielles)

### Durée de conservation
- **Durée active** : Jusqu'à fin du projet (02/02/2026)
- **Archivage** : 3 ans (pour amélioration continue du modèle)
- **Suppression définitive** : Après 3 ans ou sur demande

### Mesures de sécurité
- ✅ Anonymisation automatique (suppression noms, entreprises, lieux précis)
- ✅ Stockage chiffré (Google Sheets avec accès restreint)
- ✅ Pas de collecte d'adresse IP
- ✅ Pas de collecte d'identifiants personnels (nom, prénom, email)
- ✅ NER (Named Entity Recognition) pour supprimer entités nommées

### Transferts hors UE
❌ Aucun transfert hors Union Européenne

### Droits des personnes
- ✅ Droit d'accès (demande par email)
- ✅ Droit de rectification
- ✅ Droit à l'effacement (suppression immédiate sur demande)
- ✅ Droit d'opposition (retrait du consentement)
- ✅ Droit à la portabilité (export des données)
<<<<<<< HEAD

---

## TRAITEMENT 2 : Gestion des comptes utilisateurs {#traitement-2}

### Finalité
Permettre l'authentification et la gestion des accès à la plateforme Safe Space.

### Base juridique
- **Article 6.1.b RGPD** : Exécution du contrat (CGU acceptées)
- **Article 6.1.f RGPD** : Intérêt légitime (sécurité de la plateforme)

### Catégories de données collectées
- **Données d'identification** :
  - Email (ou pseudonyme anonyme si compte anonyme)
  - Mot de passe (haché avec BCrypt)
  - Rôle (Victime, Témoin, Modérateur, Admin)
  
- **Données techniques** :
  - Date de création compte
  - Date dernière connexion
  - Adresse IP (logs de connexion - 6 mois max)
  - User-Agent (navigateur)

### Catégories de personnes concernées
- Utilisateurs inscrits (victimes, témoins, modérateurs, admins)

### Destinataires des données
- **Internes** : Équipe Safe Space (support technique)
- **Externes** : Aucun sauf obligation légale

### Durée de conservation
- **Compte actif** : Tant que compte non supprimé
- **Après suppression** : Anonymisation immédiate (conservation logs anonymisés 6 mois pour sécurité)

### Mesures de sécurité
- ✅ Chiffrement mots de passe (BCrypt cost 12)
- ✅ Authentification JWT (tokens courts : 15min)
- ✅ Protection contre attaques (rate limiting, CAPTCHA)
- ✅ HTTPS/TLS 1.3
- ✅ 2FA optionnelle

### Transferts hors UE
❌ Aucun (serveurs en UE uniquement)

### Droits des personnes
- ✅ Droit d'accès (export données compte)
- ✅ Droit de rectification (modification profil)
- ✅ Droit à l'effacement (suppression compte)
- ✅ Droit d'opposition
- ✅ Droit à la portabilité

---

## TRAITEMENT 3 : Traitement des signalements {#traitement-3}

### Finalité
Permettre aux victimes de signaler des violences au travail et obtenir une qualification juridique automatique.

### Base juridique
- **Article 6.1.b RGPD** : Exécution du contrat
- **Article 9.2.f RGPD** : Défense de droits en justice
- **Article 9.2.a RGPD** : Consentement explicite pour données sensibles

### Catégories de données collectées
- **Données du signalement** :
  - Description des faits (texte chiffré)
  - Date des faits
  - Catégorie de violence (générée par IA)
  - Qualification juridique (articles de loi)
  - Réponses aux questions IA (JSON)
  - Niveau de gravité (automatique)

- **Métadonnées** :
  - Date de création
  - Statut (brouillon, soumis, validé)
  - Identifiant victime (chiffré)

### Catégories de personnes concernées
- Victimes de violences au travail

### Destinataires des données
- **Internes** : 
  - Équipe modération (validation signalements)
  - Service IA (amélioration continue)
- **Externes** (UNIQUEMENT avec consentement ou réquisition) :
  - Avocats (partage volontaire)
  - RH entreprise (consentement explicite)
  - Autorités judiciaires (réquisition)

### Durée de conservation
- **Phase active** : 6 ans (prescription pénale)
- **Après résolution** : Archivage 3 ans ou suppression immédiate sur demande
- **Si prescription** : Suppression automatique

### Mesures de sécurité
- ✅ Chiffrement end-to-end (AES-256-GCM)
- ✅ Clés uniques par signalement (KMS)
- ✅ Horodatage certifié (RFC 3161)
- ✅ Audit logs complets (qui accède, quand, pourquoi)
- ✅ Anonymisation automatique (suppression entités nommées)

### Transferts hors UE
❌ Aucun

### Droits des personnes
- ✅ Droit d'accès (export signalement)
- ✅ Droit de rectification
- ✅ Droit à l'effacement (suppression immédiate)
- ⚠️ Droit d'opposition limité (si procédure judiciaire en cours)

---

## TRAITEMENT 4 : Gestion du coffre-fort de preuves {#traitement-4}

### Finalité
Stocker de manière sécurisée les preuves de violences (documents, photos, enregistrements).

### Base juridique
- **Article 6.1.b RGPD** : Exécution du contrat
- **Article 9.2.f RGPD** : Défense de droits en justice

### Catégories de données collectées
- **Fichiers** :
  - Documents (PDF, DOCX, emails)
  - Images (screenshots, photos)
  - Audio (enregistrements - avec avertissement légal)
  - Vidéo (avec avertissement légal)

- **Métadonnées** :
  - Hash SHA-256 (intégrité)
  - Date d'upload
  - Timestamp certifié (horodatage légal)
  - Propriétaire (victime ou témoin)
  - Tags/catégories

### Catégories de personnes concernées
- Victimes (propriétaires de preuves)
- Témoins (contributeurs de preuves)
- Tiers identifiés dans les preuves (agresseurs, collègues)

### Destinataires des données
- **Internes** : Propriétaire uniquement
- **Externes** (consentement ou réquisition) :
  - Victimes (si preuve partagée par témoin)
  - Avocats (partage volontaire)
  - Autorités (réquisition judiciaire)

### Durée de conservation
- **Phase active** : Tant que utilisateur conserve
- **Après suppression compte** : Suppression immédiate fichiers
- **Maximum absolu** : 10 ans (prescription civile)

### Mesures de sécurité
- ✅ Chiffrement AES-256-GCM avec clés uniques
- ✅ KMS (Key Management Service)
- ✅ Horodatage certifié RFC 3161
- ✅ Watermarking invisible (traçabilité)
- ✅ Rate limiting téléchargements (10/heure/user)
- ✅ Logs d'accès détaillés

### Transferts hors UE
❌ Aucun (stockage cloud UE uniquement)

### Droits des personnes
- ✅ Droit d'accès (download preuves)
- ✅ Droit à l'effacement (suppression immédiate)
- ⚠️ Droit d'opposition limité (si procédure judiciaire)

---

## TRAITEMENT 5 : Modération des contenus {#traitement-5}

### Finalité
Valider les signalements, détecter les cas critiques, améliorer la qualification IA.

### Base juridique
- **Article 6.1.f RGPD** : Intérêt légitime (sécurité, qualité du service)

### Catégories de données collectées
- **Données de modération** :
  - Signalements en attente
  - Corrections catégorisation IA
  - Détection mots-clés critiques (viol, suicide, menaces)
  - Décisions modérateurs (validation/rejet)
  - Raisons corrections

### Catégories de personnes concernées
- Victimes (auteurs de signalements)
- Modérateurs (professionnels formés)

### Destinataires des données
- **Internes** : Équipe modération uniquement
- **Externes** : Aucun sauf urgence vitale (autorités)

### Durée de conservation
- **Historique modération** : 3 ans (amélioration IA)
- **Logs modérateurs** : 5 ans (audit)

### Mesures de sécurité
- ✅ Accès restreint (ROLE_MODERATOR)
- ✅ Formation modérateurs (psycho-trauma)
- ✅ Logs d'actions traçables
- ✅ Détection cas critiques automatique (< 1h)

### Transferts hors UE
❌ Aucun

### Droits des personnes
- ✅ Droit d'accès (décisions modération)
- ✅ Droit de rectification (contestation décision)

---

## TRAITEMENT 6 : Géolocalisation des ressources {#traitement-6}

### Finalité
Orienter utilisateurs vers ressources d'aide (avocats, associations, psychologues).

### Base juridique
- **Article 6.1.f RGPD** : Intérêt légitime (aide aux victimes)

### Catégories de données collectées
- **Localisation utilisateur** (facultative) :
  - Coordonnées GPS (non stockées, calcul temps réel)
  - Ville/Département (pour recherche)

- **Ressources** :
  - Nom, adresse, coordonnées (professionnels)
  - Spécialités, tarifs, langues

### Catégories de personnes concernées
- Utilisateurs cherchant aide
- Professionnels référencés (consentement)

### Destinataires des données
- **Internes** : Service de recherche géospatiale (PostGIS)
- **Externes** : Aucun

### Durée de conservation
- **Localisation** : Non stockée (calcul éphémère)
- **Historique recherches** : Anonymisé, 1 an max

### Mesures de sécurité
- ✅ Pas de stockage localisation GPS
- ✅ Requêtes PostGIS sécurisées
- ✅ Demande permission géolocalisation navigateur

### Transferts hors UE
❌ Aucun

### Droits des personnes
- ✅ Droit d'opposition (refus géolocalisation)

---

=======
---
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb
## OBLIGATIONS ET PROCÉDURES

### Exercice des droits

**Contact** : alixveyrat@gmail.com  
**Délai de réponse** : 1 mois maximum

**Procédure** :
1. Demande par email avec justificatif identité
2. Vérification identité
3. Réponse sous 1 mois

### Violation de données (Data Breach)

**Procédure** :
1. Détection (monitoring automatique)
2. Notification CNIL sous 72h
3. Information utilisateurs si risque élevé
4. Mesures correctives immédiates

### Analyses d'impact (DPIA)

**DPIA obligatoire pour** :
- Traitement signalements (données sensibles)
- Coffre-fort preuves (chiffrement, horodatage)
- Modération automatique (décisions IA)

**DPIA réalisée** : ✅ Oui (30/10/2025)

---

<<<<<<< HEAD
## SOUS-TRAITANTS

**Hébergement** :
- **Nom** : À définir (OVH, Scaleway, Heroku)
- **Localisation** : Union Européenne uniquement
- **Certifications** : ISO 27001, HDS (Hébergeur Données de Santé)
- **Contrat** : DPA (Data Processing Agreement) signé

**Service IA** :
- **Nom** : Aucun (modèle auto-hébergé)
- **Alternative LLM** : OpenAI, Anthropic (si utilisé, DPA requis)
=======

**Service IA** :
- **Nom** : Aucun (modèle auto-hébergé)
>>>>>>> b3a6cfac5e77293fa4e55b63792b579dbfaaa8eb

---

## HISTORIQUE DES MODIFICATIONS

| Date | Version | Modifications |
|------|---------|---------------|
| 30/10/2025 | 1.0 | Création registre initial |

---

**Document établi conformément à l'article 30 du RGPD**  
**Responsable** : Alix VEYRAT  
**Contact** : alixveyrat@gmail.com
