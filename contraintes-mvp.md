Contraintes MVP — [Project A]

Persona
judas, réparateur d'ordinateur, Dakar, téléphone portable et ordinateur

Contraintes Non Négociables

Contrainte 1
Critère : Le MVP DOIT fonctionner à 100% hors-ligne et synchroniser les données de manière asynchrone avec une consommation de data minimale.
Origine : Chapeau Noir
Élimine : Les architectures imposant une connexion Internet permanente et le rechargement en temps réel d'interfaces web lourdes.

Contrainte 2
Critère : Le MVP DOIT permettre l'enregistrement d'une demande de réparation en moins de 30 secondes ou 3 clics maximum.
Origine : Chapeau Noir
Élimine : Les formulaires de saisie complexes, les champs obligatoires multiples et les workflows administratifs lourds.

Contrainte 3
Critère : Le MVP DOIT fournir une vue centralisée unique des requêtes et un historique client rattaché à un seul identifiant (ex: numéro de téléphone).
Origine : Chapeau Blanc
Élimine : La dispersion du suivi des réparations sur des carnets papier, des conversations WhatsApp isolées ou des fils SMS séparés.

Contrainte 4
Critère : Le MVP NE DOIT PAS dépasser un poids de téléchargement/chargement initial minimal ou nécessiter une application native volumineuse.
Origine : Chapeau Noir
Élimine : Les applications mobiles natives lourdes (ex: APK volumineux) gourmandes en stockage et en forfait data lors de l'installation ou des mises à jour.

Fonctionnalités Éliminées
Formulaires de diagnostic détaillés et multi-étapes → éliminés parce qu'ils imposent une saisie manuelle lourde qui augmente la charge mentale de Judas.
Synchronisation et notifications cloud en temps réel → éliminées parce qu'elles échouent en cas de connectivité instable et consomment trop de forfait data.
Application native lourde à télécharger sur les stores → éliminée parce que le coût du forfait data et le stockage limité du smartphone freinent son adoption.
Processeur de suivi multi-canaux automatisé complexe (API WhatsApp/SMS dédiées payantes) → éliminé parce qu'il alourdit la structure du MVP avant de valider la centralisation de base.

Critère de Validation Final
Le MVP est valide si et seulement si Judas parvient à enregistrer et retrouver l'historique complet d'une réparation en moins de 30 secondes sans dépendre d'une connexion Internet stable.
