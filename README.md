# Site E&C IMMO

Site vitrine destiné à convaincre des **propriétaires bailleurs** de confier leur appartement
à E&C IMMO (bail civil + sous-location meublée courte durée sur Airbnb / Booking.com / Abritel).

## État actuel

- `index.html` : page unique, autonome (HTML/CSS/JS inline, seule dépendance externe = Google Fonts).
- Pas de framework, pas de build step. S'ouvre directement dans un navigateur.
- Design : fond encre (#122038) / laiton (#a9824c) / papier (#efece2), polices Fraunces (display) + Inter (corps) + IBM Plex Mono (chiffres/labels).
- Élément signature : graphique en hero comparant "loyer classique" (interrompu par la vacance) vs "loyer E&C IMMO" (fixe).
- Sections : hero → chiffres clés → le modèle (bail civil) → 6 avantages (chacun référence une vraie clause du bail) → secteurs gérés (icônes, pas de fausses photos) → FAQ → équipe → contact.

## Contexte business (pour éviter de tout réexpliquer)

- E&C IMMO, SAS, RCS Paris 989 829 213, siège 101 rue Mademoiselle, 75015 Paris.
- Associés : Édouard Toulet et Christopher Malmezac.
- Modèle : bail civil (pas loi 89, pas bail commercial) signé avec le propriétaire, qui autorise
  explicitement la sous-location commerciale. E&C IMMO devient seul locataire, sous-loue en meublé
  de courte durée, verse un loyer fixe au propriétaire quel que soit le taux d'occupation.
- 9 appartements actuellement gérés, secteurs : Asnières-sur-Seine, Pantin, Massy, Bezons.
- Clientèle cible : corporate housing en priorité, Airbnb en complément (remplissage des vacances).
- Contact affiché : contact@ec-immo.fr (pas de numéro de téléphone fiable disponible pour l'instant).
- Le formulaire de contact utilise actuellement un fallback `mailto:` — pas de vrai backend.

## À faire / pistes d'évolution

- [ ] Brancher le formulaire de contact sur un vrai service (Formspree, ou autre) pour recevoir les
      soumissions sans mailto.
- [ ] Ajouter un vrai numéro de téléphone une fois confirmé.
- [ ] Remplacer les icônes de secteurs par de vraies photos des appartements si/quand disponibles.
- [ ] Déploiement : GitHub Pages (comme le projet checklist existant : github.com/edmarsht/checklist-ecimmo)
      ou l'hébergeur actuel de ec-immo.fr.
- [ ] Éventuellement passer à plusieurs pages (une par secteur, page "actualités"...) si le contenu grossit.

## Contraintes de contenu

Toute affirmation sur le fonctionnement juridique du bail (durée, préavis, assurances, sous-location...)
doit rester fidèle au contrat réel signé par E&C IMMO — ne pas inventer de clauses ni de chiffres
commerciaux (taux de satisfaction, % de revenus, etc.) qui ne sont pas fournis explicitement.
