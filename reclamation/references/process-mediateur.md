# Saisir un médiateur en ligne

Le parcours décrit est celui de la Médiation de l'Assurance (mediation-assurance.org), le plus fréquent. Les autres médiateurs sectoriels (énergie, télécoms, tourisme, banque, Médiateur des entreprises) fonctionnent sur le même modèle : un formulaire, des pièces, un récépissé, puis un délai de recevabilité.

## Avant de saisir

Vérifie les deux conditions de recevabilité, sinon la saisine est irrecevable et personne ne le dira tout de suite :

1. Une réclamation écrite a été adressée au professionnel, avec une date et un destinataire identifiable (le service réclamations, pas le service sinistres ni le commercial).
2. Soit 2 mois se sont écoulés sans réponse, soit une réponse écrite insatisfaisante a été reçue. Moins d'un an s'est écoulé depuis la réclamation.

Et vérifie que le litige est dans le champ du médiateur (le site le dit ; certains médiateurs excluent les litiges déjà portés devant un juge, ou les professionnels).

## Les pièces, dans l'ordre

1. La réclamation écrite au professionnel, elle-même, pas seulement l'accusé de réception.
2. L'accusé de réception ou la preuve d'envoi.
3. La réponse du professionnel si elle existe.
4. Le contrat et les conditions générales.
5. Les pièces du litige (factures, attestations, courriers).
6. Un exposé en une page : les faits datés, ce qu'on demande, pourquoi (les observations juridiques, présentées comme telles).

Un seul PDF par pièce, nommé avec la date et le contenu (`2026-06-01_Reclamation_assureur.pdf`). Le formulaire limite souvent le nombre et le poids des pièces : compresse les scans.

## Le formulaire, avec un agent qui pilote le navigateur

L'agent peut créer le compte, remplir le formulaire, rédiger l'exposé et le déposer. Sur un dossier réel, il a monté tout le dossier pendant que l'utilisateur était en réunion. Deux choses restent à l'utilisateur :

- Le téléversement des pièces, si le formulaire refuse le fichier proposé par l'agent (voir la contrainte dans [process-laposte.md](process-laposte.md)). L'agent prépare les fichiers, nomme les pièces, et dit lesquelles glisser.
- La validation finale et l'envoi. L'agent s'arrête à l'écran de récapitulatif.

Archive le récépissé (email ou capture) dans le dossier, note le numéro dans `notes.md` et `journal.md`.

## Ce qui se passe après, et les pièges

**Le récépissé n'est pas l'ouverture du dossier.** La Médiation de l'Assurance donne d'abord un numéro de demande (format DEM-xxxxxx-année). Ce n'est pas un identifiant de dossier : il ne permet pas de se connecter à l'espace réclamant, dont l'identifiant a un autre format (ABR, PRE ou VIE). Tant qu'on n'a pas reçu ce second identifiant, le dossier n'est pas ouvert, rien n'est instruit, et la prescription n'est pas suspendue (la Charte du médiateur suspend la prescription à compter de la notification de recevabilité, pas de la demande).

**Le délai de recevabilité est de 21 jours.** Passé ce délai sans nouvelle, relance par trois canaux le même jour : le formulaire de contact du site (choisir « autre motif » si le suivi de réclamation exige un numéro qu'on n'a pas), un email à l'adresse de traitement (pour la Médiation de l'Assurance : Le.Mediateur@mediation-assurance.org ; jamais l'adresse noreply), et un recommandé au siège avec le récépissé de saisine. Sur un dossier réel, ce triple canal a débloqué en 3 jours un dossier muet depuis 6 semaines.

**Le médiateur réclame la pièce qui manque.** Le plus souvent la réclamation écrite au professionnel, avec sa date d'envoi et son destinataire. Envoie-la à l'adresse de traitement, en rappelant le numéro de dossier, et vérifie que la pièce jointe est bien partie.

**La saisine prématurée.** Si la saisine a été faite avant les 2 mois, ne pas la retirer : régulariser dès que la condition est remplie (délai échu, ou réponse écrite insatisfaisante reçue entre-temps), et présenter la transmission des pièces comme une régularisation à la date du jour.

**Le silence du professionnel pendant la médiation.** Il arrive que le professionnel réponde enfin, par écrit, pendant que le médiateur instruit. Cette réponse règle la question de recevabilité (il existe désormais une réponse insatisfaisante) et contient souvent la phrase qui fera gagner (voir [assurance.md](assurance.md), la bonne foi). Transmets-la au médiateur avec l'observation qui va avec.

**Les emails tombent dans les dossiers secondaires** du client mail. Va les chercher, à chaque échéance.

## Une fois recevable : le mémoire, en un seul tour

La notification de recevabilité change tout : le médiateur demande les pièces contractuelles (police, conditions générales, questionnaire de souscription, correspondances), donne les codes de l'espace réclamant, et précise que sa position clôt la procédure. Il n'y a pas d'aller-retour : tout ce qui doit être lu part dans le même envoi.

Avant d'écrire une ligne, récupérer les pièces contractuelles sur l'espace client du professionnel (elles n'y sont presque jamais dans le dossier de l'utilisateur). Lire la police en entier : elle dit ce qui a été souscrit, et souvent ce qui n'y figure pas (une réserve qui n'apparaît que dans un courrier n'est pas dans le contrat). Lire les conditions générales : elles reproduisent souvent la loi mot pour mot, et deviennent la meilleure pièce contre leur auteur.

Le mémoire (voir `templates/saisine-mediateur.md` pour l'exposé court ; le mémoire est sa version longue) :

1. Les parties, les références, la chronologie datée.
2. Les faits, pièce par pièce, numérotées (P01, P02...), chaque affirmation renvoyant à sa pièce.
3. Les observations juridiques, en non-juriste, avec les citations exactes des conditions générales et du courrier de l'adversaire.
4. La demande principale, puis les demandes subsidiaires, dans le même document. Un médiateur qui ne peut pas accorder le principal doit avoir une position de repli à proposer, sinon il ne propose rien.
5. La pièce que l'adversaire est seul à détenir (le questionnaire de souscription, l'expertise interne) : demander au médiateur de l'exiger, avec horodatage, plutôt que de faire comme si elle n'existait pas.

Sur l'espace réclamant, les documents se déposent par zone (médical ou non médical, selon les médiateurs) : seules les pièces d'une zone sont transmises à l'autre partie. Choisir en connaissance de cause. Puis vérifier dans « Documents transmis » que chaque fichier apparaît avec son horodatage. Une pièce complémentaire pendant l'instruction reste possible, déposée seule avec un commentaire de deux lignes qui la rattache au point du mémoire concerné. Pas de second mémoire.

Le dépôt lui-même (identifiants, téléversement) est fait par l'utilisateur. L'agent assemble le dossier, numérote et nomme les fichiers comme dans le mémoire, et rédige le commentaire de dépôt.

## Les délais

| Étape | Délai | Levier |
|---|---|---|
| Recevabilité | 21 jours | Relance triple canal |
| Avis | 90 jours à compter de la recevabilité selon la Charte ; 7,5 mois en moyenne réelle annoncée par la Médiation de l'Assurance en 2026 | Message via l'espace réclamant à 9 mois si silence, puis CECMC (commission qui contrôle les médiateurs de la consommation) |
| Après l'avis | Chaque partie a un mois pour accepter ou refuser ; le silence de l'assureur vaut acceptation (Charte) | Juge si refus |

Le vrai délai se dit à l'assessment. Une médiation est un engagement de six mois à un an, pas de trois mois.

## Mode de gestion : passif

Une fois le dossier complet et recevable, il n'y a rien à faire pendant des semaines. Ne relance pas hors des dates ci-dessus, ne renvoie pas de pièces, ne résilie pas le contrat. Le silence n'est pas un signal sur la solidité du dossier. Dis-le à l'utilisateur, une fois, et note la prochaine date dans le journal.
