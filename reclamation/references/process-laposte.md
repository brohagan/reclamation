# Envoyer un recommandé sans imprimante (laposte.fr)

La lettre recommandée en ligne de La Poste : vous téléversez un PDF, La Poste l'imprime, le met sous pli et poste un recommandé papier classique avec accusé de réception. Pas d'imprimante, pas de file d'attente. Quatre pages recto-verso avec avis de réception : autour de 8,60 € TTC (tarif observé en 2026, à vérifier sur le site). Preuve de dépôt reçue par email dans les deux minutes qui suivent le paiement, avec le numéro de suivi et un PDF officiel.

Pas la lettre recommandée 100 % électronique (type AR24) : le destinataire doit avoir accepté ce canal, ce qui n'est jamais garanti pour une administration, une agence ou une association. Le recommandé papier ne pose pas cette question.

## Avant d'ouvrir le navigateur

1. Le courrier est relu et validé par l'utilisateur. Un recommandé ne se rappelle pas.
2. Génère le PDF du courrier, signé (l'utilisateur fournit une image de sa signature une fois, elle sert pour tous les courriers).
3. Fusionne les pièces jointes dans un seul PDF, dans l'ordre annoncé dans le courrier. Vérifie que chaque pièce annoncée est bien là.
4. Compresse si le total dépasse quelques mégaoctets ; les scans de courriers adverses sont souvent lourds.
5. Note dans le journal : date, destinataire, objet, liste des pièces.

## Sur laposte.fr, avec un agent qui pilote le navigateur

Le parcours « Lettre recommandée en ligne » demande un compte La Poste (l'utilisateur le crée ou se connecte lui-même si un mot de passe est demandé).

- Destinataire : nom, adresse. Pour un destinataire en TSA, CEDEX ou boîte postale (les assureurs, les médiateurs, les administrations), cocher « adresse professionnelle » : sinon les champs Code CEDEX et BP/CS/TSA n'apparaissent pas et le routage est faux.
- Expéditeur : l'utilisateur, adresse complète, c'est là que reviendra l'avis de réception papier.
- Options : avis de réception oui, recto-verso oui (le recto simple coûte plus cher et n'apporte rien), couleur non.
- Téléverser le PDF unique. Vérifier l'aperçu page par page.
- **S'arrêter à l'écran de paiement.** L'utilisateur paie lui-même. Il n'y a pas de droit de rétractation sur un recommandé en ligne, et ce n'est pas à l'agent de dépenser.

Contrainte connue avec Claude in Chrome : l'outil de téléversement n'accepte pas les chemins de fichiers de l'ordinateur de l'utilisateur ; le fichier doit être copié dans le dossier de sortie de la session avant d'être proposé au formulaire. Si le téléversement échoue, dis-le et laisse l'utilisateur glisser le PDF lui-même.

## Après le paiement

- L'email de La Poste (`notification@notif.laposte.fr` ou similaire) contient la preuve de dépôt en pièce jointe, avec le numéro de suivi. Archive-la dans le dossier, sous un nom daté, et note le numéro dans `notes.md` et `journal.md`. Ces emails tombent souvent dans les dossiers secondaires du client mail : va les chercher.
- Suivi : le numéro se suit sur laposte.fr. Première présentation, avis de passage, retrait ou retour. Un recommandé non retiré a quand même été présenté : c'est la présentation qui fait courir les délais, pas la lecture. Note la date de première présentation dans le journal.
- L'avis de réception papier revient par courrier une à deux semaines plus tard. Scanne-le, archive-le.
- Le même jour que le dépôt, envoie le contenu intégral par email aux personnes concernées, en mentionnant le numéro de recommandé. Le recommandé fait la preuve, l'email fait le travail.
