# Juvem — programme de test Android

Portail public de GolApp Studio pour préparer et accompagner le test fermé de **Juvem** (`com.golappstudio.juvem`).

## Accès

- URL publique : https://shamsgolap.github.io/juvem-testing/ (accessibilité à vérifier après chaque modification)
- Dépôt : https://github.com/ShamsGolap/juvem-testing
- Confidentialité : https://shamsgolap.github.io/juvem-privacy/
- Application source (privée) : `ShamsGolap/juvem`, branche `develop`.

## Contenu

- Site statique en français, responsive, sans dépendance, JavaScript, analytics, formulaire ou cookie applicatif.
- Inscription volontaire par e-mail (le site n'envoie aucune donnée lui-même).
- Instructions pour rejoindre le **futur** test fermé Google Play, sans prétendre que les liens sont déjà disponibles.
- Parcours de recette centrés sur les humeurs, le journal, les pauses, les thèmes **système / clair / sombre**, les langues **système / français / anglais**, les grands caractères et l'accessibilité.
- Section **Juvem Preview** : quatre jeux de données fictifs (3, 14, 10 ou 90 humeurs) et tests d'export/import chiffré par mot de passe. La distribution de l'APK n'est pas encore ouverte.
- Prévention contre les partages de données sensibles et les faux appels d'urgence.
- Liens vers la politique de confidentialité et le site GolApp Studio.

## Hébergement et mise à jour

Site statique maintenu sur `main / (root)` de GitHub Pages. Une mise à jour du dépôt peut provoquer une publication automatique gérée par GitHub ; aucun workflow Actions personnalisé ne doit être introduit ou lancé. Vérifier le rendu public après chaque modification.

## Situation de Juvem Bêta 1 — 31 octobre 2026

Les PR #2, #3 et #4 sont intégrées à `develop` (`0.1.0-beta.1+1`). Les tests Flutter et la recette Android ne sont pas encore attestés. Le portail couvre la Preview isolée, les quatre jeux fictifs, le stockage local chiffré et les sauvegardes protégées par mot de passe. **Aucun lien Play Store ou APK n'est annoncé comme disponible.**

## Preview et Google Play

La Preview debug est construite séparément avec `flutter build apk --debug -t lib/main_preview.dart` : identifiant `com.golappstudio.juvem.preview`. Elle n'est pas compatible avec la fiche Google Play du package `com.golappstudio.juvem` sans une seconde application Play Console. Ne pas mélanger les deux parcours ni annoncer une publication non vérifiée.

## Quand le test sera disponible

1. Remplacer le message « test en préparation » par des liens Google Play **réellement générés** et vérifiés (opt-in + fiche), après ouverture du programme.
2. Ajouter la version et la date de sortie effectivement publiées.
3. Vérifier les consignes de test et l'e-mail de contact dans les paramètres Play Console.
4. Ne pas afficher de lien APK direct non signé ou non validé.

## Sécurité

Aucune donnée de santé ni extrait du journal ne doit être envoyé dans les retours des testeurs. Le fichier de site ne contient aucun jeton ni secret. Voir [SECURITY.md](SECURITY.md).
