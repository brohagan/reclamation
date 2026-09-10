<h1 align="center">Réclamation</h1>

<p align="center">
  <b>Un skill pour agents IA qui mène vos litiges du quotidien, en français, sans avocat.</b>
</p>

<p align="center">
  Parce que l'assureur, l'agence et le loueur comptent sur votre fatigue. Le skill, lui, ne se fatigue pas.
</p>

<p align="center">
  <a href="https://github.com/marge-now/reclamation/blob/main/LICENSE"><img src="https://img.shields.io/badge/licence-MIT-blue" alt="MIT"></a>
  <img src="https://img.shields.io/badge/langue-fran%C3%A7ais-lightgrey" alt="français">
  <a href="https://marge.now"><img src="https://img.shields.io/badge/un%20projet-Marge-F2B41A" alt="Marge"></a>
</p>

---

## Qu'est-ce que c'est ?

Réclamation est un skill pour agents IA ([Claude Code](https://claude.com/product/claude-code), [Claude Cowork](https://claude.com/product/cowork), et tout agent capable de lire un dossier de fichiers Markdown) qui prend en charge un litige de particulier ou de petite entreprise : une assurance qui refuse de rembourser, un bailleur qui laisse traîner un danger, un prestataire qui ne livre pas et prélève quand même.

Il fait ce qu'un ami juriste et organisé ferait pour vous, dans l'ordre :

1. **L'assessment** : quel est vraiment le problème, ce que ça coûte, ce qu'on peut récupérer, ce que ça demande, et si ça vaut le coup d'y aller. Vous décidez.
2. **Le dossier** : un brain du litige (parties, chronologie, pièces, deadlines) et un journal des envois avec preuves, tenus à jour à chaque épisode.
3. **Les courriers** : réclamation, mise en demeure, relance d'escalade, saisine du médiateur, signalement à la mairie, résolution de contrat. Rédigés dans un registre précis, vérifiés juridiquement, relus pour ne pas sentir l'IA.
4. **L'action** : le recommandé déposé sur laposte.fr sans imprimante, le dossier monté sur le site du médiateur, les drafts prêts dans votre boîte mail. Vous payez, vous uploadez, vous envoyez. Jamais lui.
5. **L'escalade** : un cran à la fois, annoncé dans le courrier précédent, exécuté à la date dite.

Il est né de trois vrais dossiers menés à l'été 2026 avec Claude, racontés dans [`cas/`](cas/) : une exclusion à vie posée par un assureur animalier sur un chiot de 8 mois, un vélo en location longue durée tombé en panne quatre fois, un balcon condamné par une agence qui envoyait des menuisiers réparer du verre. Zéro avocat, trois recommandés à 8,60 €, un remboursement intégral et deux dossiers qui avancent.

---

## Installation

Copiez-collez dans votre agent :

```
Installe le skill du repo github https://github.com/marge-now/reclamation
puis lance un assessment sur mon litige
```

Ou à la main : copiez le dossier `reclamation/` dans le dossier de skills de votre agent (`~/.claude/skills/` pour Claude Code) et créez un dossier `dossiers/` à côté pour vos litiges.

Le skill est du Markdown. Pas de dépendance, pas de script, pas de clé API. Le dépôt du recommandé et le formulaire du médiateur demandent un agent capable de piloter un navigateur (Claude in Chrome, ou le navigateur intégré de Cowork).

---

## Exemples

```
> Mon assureur a posé une exclusion sur mon chien pour un épisode de diarrhée antérieur à la souscription. Est-ce que ça vaut le coup de contester ?

> Voilà le contrat de location de mon vélo et les emails du loueur. Le vélo est en panne depuis 3 semaines, ils continuent à prélever. Fais-moi l'assessment.

> Mon agence m'interdit l'accès à mon balcon depuis 2 mois « en attendant l'assurance ». Rédige la mise en demeure.

> Le médiateur n'a pas répondu depuis 6 semaines. Qu'est-ce qu'on fait ?

> Ils ont répondu, voilà leur mail. Cran suivant ou on accepte ?

> Prépare le recommandé sur laposte.fr, je paierai moi-même.
```

---

## Ce que le skill sait faire, et ce qu'il refuse

**Il sait** : lire vos contrats et conditions générales en entier, connecter un courrier de l'adversaire à l'article qui le contredit, tenir la chronologie et les deadlines, écrire dans le registre qui fait bouger un service réclamations, et préparer chaque action jusqu'au dernier clic avant paiement ou envoi.

**Il refuse** : de citer un article de loi qu'il n'a pas vérifié à la source, d'envoyer un courrier ou un email à votre place, de payer, de menacer de publier quelque chose sous condition de paiement (c'est la ligne du chantage), et de vous pousser dans un combat dont l'assessment dit qu'il ne vaut pas le coup.

Le curseur d'agressivité a trois positions, **doux**, **moyen**, **épicé**. Vous choisissez le départ, le skill ajuste d'après les faits : deadlines ignorées, aveux écrits, temps écoulé. Trop agressif, on est ridicule. Trop soumis, on se fait marcher dessus.

---

## Structure

```
reclamation/
  SKILL.md            le routeur : prérequis, échéances, domaine → référence, structure de réponse
  references/         la méthode, le registre, le droit par domaine, les process
  templates/          brain de dossier, journal, et les courriers
  evals/              cas de test au format anthropics/skills
cas/                  trois litiges réels, anonymisés, du premier mail à l'issue
dossiers/             vos litiges (jamais commités)
```

---

## Avertissement

Ce skill a été écrit par un non-juriste, pour des non-juristes, à partir de dossiers réels. Il aide à comprendre un litige, à l'organiser et à écrire juste. Il ne remplace pas un avocat, il vous dit quand il en faut un : montant important, procédure engagée contre vous, adversaire représenté, ou tout ce qui touche au pénal.

Chaque article cité est vérifié sur Légifrance au moment de l'écriture du courrier. Le droit français bouge, le skill le sait, et il le signale quand il n'est pas sûr.

---

## Un projet Marge

[Marge](https://marge.now) est un cabinet de conseil en IA agentique pour les entreprises françaises de 50 à 1 000 salariés. Réclamation est notre premier projet open source : la méthode qu'on applique en entreprise (un brain, un journal, des skills qui lisent, écrivent et agissent), appliquée à la paperasse qui pourrit la vie de tout le monde.

Inspiré par [paperasse](https://github.com/romainsimon/paperasse), qui a montré que des skills en Markdown pouvaient faire le travail d'un cabinet.

Contributions bienvenues, voir [CONTRIBUTING.md](CONTRIBUTING.md). Licence MIT.
