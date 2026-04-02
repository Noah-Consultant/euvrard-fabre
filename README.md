# euvrard-fabre
Landing page interactive avec simulateur ROI pour une offre de consulting commissaires-priseurs — rapprochement bancaire post-vente. HTML/CSS/JS, fichier unique, zéro dépendance.


# Sprint Rapprochement Bancaire — Landing Page

Landing page interactive pour une offre de consulting dédiée aux commissaires-priseurs : structurer et fiabiliser le rapprochement bancaire post-vente.

---

## Contexte

Les études de commissaires-priseurs consacrent un temps considérable au rapprochement bancaire après chaque vente aux enchères. Ce process, souvent manuel et non documenté, repose entièrement sur la dirigeante — source de charge mentale, de fragilité opérationnelle et de difficulté à déléguer.

Cette page présente un **sprint de 6 semaines** dont l'objectif est de réduire de 50 % le temps passé sur ce rapprochement, en structurant le process, en l'outillant et en le rendant transmissible.

## Fonctionnalités

- **Simulateur ROI interactif** — 5 paramètres ajustables (heures/vente, nombre de ventes, réduction visée, valeur horaire, budget mission) avec calcul en temps réel du gain de temps, de la valeur créée et du délai d'amortissement.
- **Animations au scroll** — Révélation progressive des sections via Intersection Observer.
- **Responsive** — Adapté desktop, tablette et mobile.
- **Fichier unique** — HTML, CSS et JS dans un seul fichier, aucune dépendance serveur.

## Stack

| Élément | Choix |
|---|---|
| Structure | HTML sémantique |
| Style | CSS custom properties, pas de framework |
| Typographie | Cormorant Garamond + DM Sans (Google Fonts) |
| Interactions | Vanilla JS |
| Build | Aucun — fichier statique autonome |

## Lancer le projet

Ouvrir `sprint-rapprochement-euvrard-fabre.html` dans un navigateur. C'est tout.

Pour un serveur local (optionnel) :

```bash
# Python
python3 -m http.server 8000

# Node
npx serve .
```

## Structure du fichier

```
sprint-rapprochement-euvrard-fabre.html
│
├─ <style>        → Variables, layout, composants, responsive
├─ <body>         → Hero, 3 axes, simulateur ROI, avant/après,
│                   dispositif 6 semaines, livrables & offre, CTA
└─ <script>       → Navigation sticky, scroll reveal, simulateur ROI
```

## Personnalisation

| Paramètre | Où le modifier |
|---|---|
| Adresse email du CTA | Attribut `href` du lien `mailto:` dans la section CTA final |
| Hypothèses par défaut du simulateur | Attributs `value` des `<input type="range">` |
| Plage du budget mission | Attributs `min` / `max` du slider `#input-budget` |
| Palette de couleurs | Variables CSS dans `:root` |
| Nom de l'étude / destinataire | Textes dans le `<footer>` et le hero |

## Licence

Usage privé — projet réalisé dans le cadre d'une mission de consulting.
