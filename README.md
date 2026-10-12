# Portfolio — Malick Kamara (BTS SIO, option SISR)

Portfolio statique en HTML/CSS/JS pur, hébergé sur GitHub Pages.

Ce portfolio est conçu pour l'**épreuve E5 — Support et mise à disposition de services
informatiques** (coefficient 4, oral 40 min), conformément au dossier remis par le professeur
(*Dossier élève — Construire son portfolio professionnel, BTS SIO, session 2026-2027*).
Il doit démontrer, à travers des réalisations documentées, les 6 compétences du Bloc 1
(C1 à C6).

> **Octobre 2026 — migration depuis Wix.** Ce dépôt reprend l'intégralité du contenu qui
> était publié sur le portfolio Wix (`malickkamara13.wixsite.com/2-me-portfolio`), qui peut
> désormais être supprimé. Les fichiers qui y étaient hébergés (CV, documentation) ont été
> rapatriés dans `assets/`.

## Structure du site

```
index.html                                  → toute la page, organisée selon les rubriques attendues :
                                               Accueil, Profil, Compétences, Réalisations, Veille, Stage,
                                               Formation, Projets, Documentation, Projet professionnel, Contact
style.css                                   → styles
script.js                                   → menu mobile, année du footer, bouton retour en haut
cv-malick-kamara.pdf                        → CV (lien "Télécharger mon CV")
documentation-installation-serveur-web.pdf  → documentation liée à la fiche de réalisation n°1
photo-profil.png                            → image de la section Profil
```

Tous les fichiers sont à la racine, c'est volontaire : le site tient en six fichiers et reste
modifiable directement depuis l'interface web de GitHub, sans avoir à naviguer dans des dossiers.

## Contenu actuellement en ligne

| Section | État |
|---|---|
| Profil | Complet |
| Compétences | Complet (6 compétences du Bloc 1, tableau de couverture, compétences techniques) |
| Réalisations | 1 fiche complète : mise en place d'un serveur web (C1, C4) |
| Veille technologique | 1 fiche complète : hausse des licences VMware et migration vers Proxmox, 7 sources |
| Stage | Complet : La Bureautique, 26 mai — 25 juin 2026 (pfSense, Active Directory, Zabbix) |
| Formation | Complet |
| Projets | 3 missions ESN : Active Directory, réseau Cisco, serveur DNS/DHCP |
| Documentation | 1 document : installation d'un serveur web |
| Projet professionnel | Complet |
| Contact | Email, téléphone, GitHub |

## Ce qu'il reste à faire

- **Réalisations** : ajouter les fiches n°2 et n°3 (le tableau de couverture des compétences
  les attend déjà), puis cocher les compétences C1 à C6 correspondantes.
- **Veille** : ajouter la fiche n°2 (deux fiches sont attendues par cycle, séance 7).
- **Projets** : ajouter les liens vers les dépôts GitHub de chaque mission, si elles sont versionnées.
- **LinkedIn** : le bouton a été retiré du site, le lien du Wix pointait vers l'accueil de
  LinkedIn et non vers un profil. À remettre avec la vraie URL.
- **CV** : la ligne « Portfolio : [adresse du site Wix] » du PDF doit être remplacée par
  l'adresse GitHub Pages de ce site.
- **Cohérence CV / site** : les dates de formation et de stage diffèrent entre le CV et le site
  (voir plus bas).
- **Dépôt Git** (section Profil) : le lien pointe vers ce dépôt. À mettre à jour si le site
  est republié sur le compte GitHub de Malick.
- **Barres de progression** (section Compétences) : les pourcentages sont des estimations,
  à ajuster ou à retirer.

### Écarts à trancher entre le CV et le site

| Information | Sur le site | Sur le CV |
|---|---|---|
| Dates du stage | 26 mai — 25 juin 2026 | 25 mai — 26 juin 2026 |
| BTS SIO | 2024 — 2026 | 2025 — 2027 |
| Baccalauréat | 2020 — 2024 | 2024 |

## Ajouter une fiche

Duplique un bloc `<div class="fiche-card">...</div>` existant dans `index.html` (section
Réalisations ou Veille) et remplace le contenu des `<dd>`. Les champs correspondent à ceux
du dossier officiel : contexte, besoin, objectif, environnement, technologies, travail
personnel, difficulté, diagnostic, solution, tests, résultats, documentation, compétences, bilan.

À l'oral, le jury interroge sur le travail **personnellement** réalisé (« qu'avez-vous fait ? »,
« comment avez-vous diagnostiqué le problème ? »), donc chaque fiche doit décrire des actions
réellement effectuées.

## Aperçu en local

```bash
python3 -m http.server 8000
```

puis `http://localhost:8000`.

## Déploiement

GitHub Pages, branche `main`, dossier `/ (root)` — `Settings` → `Pages`.
