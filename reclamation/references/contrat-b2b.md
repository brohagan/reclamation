# Contrat de prestation ou de location entre professionnels

Tiré d'un dossier réel : un vélo en location longue durée, quatre pannes en six semaines, un loueur qui renvoie vers son fournisseur et continue de prélever (voir `cas/velo-lld.md`). Vaut pour un abonnement, une location de matériel, une prestation non livrée, un logiciel qui ne marche pas.

## Ce qui change quand on est professionnel

Le Code de la consommation ne s'applique pas entre deux entreprises (même une EURL d'une personne). Pas de médiateur de la consommation, pas de délai de rétractation, pas de garantie légale de conformité. Reste le Code civil, qui suffit largement :

- **Art. 1719 et 1721** (location) : le loueur doit délivrer la chose en état de servir, l'entretenir, et garantir les vices qui empêchent l'usage.
- **Art. 1103** : le contrat fait loi entre les parties. Lis-le en entier, y compris ses clauses de résiliation, avant tout.
- **Art. 1199** : effet relatif des contrats. Le fournisseur du loueur, son transporteur, son sous-traitant ne nous sont pas opposables. « C'est notre fournisseur qui gère » n'est pas une réponse.
- **Art. 1219** : exception d'inexécution. On peut suspendre sa propre obligation (payer) quand l'autre n'exécute pas la sienne, à condition que l'inexécution soit suffisamment grave. Mieux vaut l'obtenir par écrit de l'adversaire (« nous suspendons les prélèvements ») que de la décider seul.
- **Art. 1224 à 1226** : résolution du contrat. Par notification, après mise en demeure restée infructueuse, « aux risques et périls » de celui qui notifie.
- **Art. 1231-1** : dommages-intérêts pour l'inexécution.

Le levier tiers : le Médiateur des entreprises (mediateur-des-entreprises.fr), gratuit, pour un litige entre deux entreprises. Puis le tribunal des activités économiques (ex-tribunal de commerce), en injonction de payer pour une créance non contestée (~40 €, sans avocat).

## Le parcours

1. **Signalement écrit** de la panne ou de l'inexécution, demande de suspension des paiements par écrit, deadline.
2. **Mise en demeure** (recommandé + email intégral à plusieurs personnes : le dirigeant, le support, le commercial) avec deux options : exécuter (remplacer, réparer) sous 15 jours, ou résoudre à l'amiable et rembourser. Délai 8 jours à réception. Voir `templates/mise-en-demeure.md`.
3. **Si aucune option n'est choisie** ou si la réponse esquive (« on relance le fournisseur ») : notification de résolution (art. 1226), aux torts exclusifs, à effet immédiat, avec le décompte de ce qui est dû, une date de virement, et l'annonce du cran suivant. Voir `templates/notification-resolution.md`.
4. **Médiateur des entreprises**, puis **injonction de payer**.

## Les pièges

**Lis les clauses de résiliation avant de notifier.** Une résolution unilatérale se fait aux risques et périls du créancier : si le contrat prévoit une indemnité de résiliation anticipée et que l'inexécution n'est pas jugée assez grave, on peut la devoir. Le dossier en face doit être solide : inexécution reconnue par écrit, plusieurs pannes documentées, mise en demeure restée sans choix, silence sur l'amiable. Sur le dossier réel, les clauses n'avaient pas été vérifiées avant de notifier ; ça s'est bien terminé, c'était un pari. Ne le refais pas.

**Le double canal.** Le recommandé fait la preuve, l'email fait le travail. Un recommandé non retiré (ils ne sont pas obligés) est présenté, c'est ce qui compte, mais l'email intégral envoyé à trois personnes le même jour est ce qui déclenche la réponse. Envoie toujours les deux.

**Les couches ne se parlent pas.** Le support relance le fournisseur le matin même où la direction reçoit la résolution. Recadre immédiatement, tout le monde en copie : ce n'est plus un dossier SAV.

**Le remboursement conditionné à la logistique.** « On rembourse quand on a récupéré le matériel », et la récupération dépend d'un tiers injoignable. Découple par écrit : le virement à telle date, quoi qu'il arrive ; l'enlèvement quand ils veulent, le matériel est disponible. Ça débloque en 24 heures.

**La contre-offre qui devient caduque.** Proposer de payer l'usage réel (six semaines sur douze) est honnête et crédible. Si l'adversaire laisse passer la deadline sans répondre, la contre-offre est déclarée caduque dans la notification suivante, et on revient au montant plein. Le silence lui a coûté la différence.

**Le prélèvement qui passe quand même.** Après un avoir ou une suspension écrite, un prélèvement peut encore partir. Vérifie le compte aux dates, et fais annuler le mandat de prélèvement côté banque si nécessaire.

## Ce qu'il faut obtenir par écrit, dans l'ordre

1. L'inexécution reconnue (« le matériel est actuellement inutilisable »).
2. La suspension des paiements.
3. Le principe du remboursement, puis son montant, puis sa date.
4. La confirmation de fin des prélèvements.
5. Après le virement : les avoirs, et une phrase de clôture : « contrat clos, aucune somme due de part et d'autre ».
6. À la restitution du matériel : photos, et un reçu signé par le transporteur.
