Alignement HMW — Backlog S3 — [Project A]

HMW Définitif
HMW Définitif — FixIt HMW Draft S1 Comment pourrions-nous aider Judas à réduire sa charge de travail pour dégager du temps pour sa famille ?
HMW Définitif S2 Comment pourrions-nous automatiser le suivi des réparations et la gestion client de Judas pour lui faire gagner 2 heures par jour à consacrer à sa famille ?
Ancrage : Réparateur d'ordinateurs · Feature : Ordinateurs & Téléphones portables.
Résiste au Chapeau Noir : * Un outil digital trop complexe ou nécessitant une saisie manuelle lourde augmentera la charge mentale de Judas au lieu de la réduire.
Le manque de connexion Internet stable ou le coût du forfait data en zone urbaine/périurbaine peut freiner l'adoption quotidienne de la solution.
💡 3 Solutions Actionnables L'Agent Vocal Intégré + Dify (Low-Data & Zero Saisie)
Principe : Directement dans l'application FixIt, Judas enregistre simplement des notes vocales (ex: "Réparation téléphone de Sarah finie, écran remplacé, 15 000 FCFA").
Résultat : L'agent Dify transcrit la note, met à jour le dossier dans l'application et prévient le client par SMS automatique. Aucune saisie manuelle lourde, très économique en data.
Le Système d'Auto-Suivi par QR Code & SMS (Zéro Interruption)
Principe : À la dépose de l'appareil (PC ou téléphone), l'application FixIt génère un reçu avec un QR Code ou envoie un lien SMS au client.
Résultat : Le client consulte l'avancement de sa réparation en autonomie via une page web simple. Cela élimine les appels et messages incessants des clients pendant la journée.
Le Carnet de Bord PWA "1-Click" (Offline-First)
Principe : L'application FixIt intègre une interface ultra-simplifiée qui fonctionne sans connexion Internet. Judas change les statuts en un clic ("Reçu", "En cours", "Prêt").
Résultat : Les données se synchronisent automatiquement dès qu'un réseau est disponible, garantissant un usage fluide sans coupures réseau.
🚀 Ce que ce HMW guide en S3 Cadrage S3 (Reformulé) : « Concevoir un assistant virtuel Dify au cœur de l'application FixIt qui permet à Judas de gérer ses réparations et d'informer ses clients à la voix, sans taper de texte et même avec un faible réseau Internet. »

Tableau d'Alignement des User Stories

US-01 — Enregistrement de note vocale Dify (mise à jour dossier + SMS client automatique)
Cette story obtient le score maximal de 6/6, avec 2 points pour l'alignement Persona, 2 points pour le Problème adressé, et 2 points pour le Contexte. Décision : CONSTRUIRE.

US-02 — Mise à jour des statuts en 1-click avec synchronisation Offline-First (PWA)
Également notée 6/6 (2 points sur chacun des trois critères : Persona, Problème, Contexte), cette story est validée pour la construction. Décision : CONSTRUIRE.

US-03 — Génération de reçu avec QR Code / lien SMS pour auto-suivi client
Avec un score de 5/6 (1 point pour Persona, 2 points pour Problème, 2 points pour Contexte), cette story reste dans le périmètre à construire. Décision : CONSTRUIRE.

US-04 — Tableau de bord analytique des revenus et statistiques mensuelles de réparation
Cette story n'obtient que 3/6 (2 points pour Persona, mais 0 point pour Problème et seulement 1 point pour Contexte), ce qui indique un alignement insuffisant avec les besoins identifiés. Décision : REPORTER.

US-05 — Module de paiement en ligne intégré pour les pièces de rechange
Avec le score le plus faible, 1/6 (1 point pour Persona, 0 point pour Problème, 0 point pour Contexte), cette story montre un décalage important avec les priorités actuelles. Décision : REPORTER.


Sprint S3 — Ordre de construction
US-01 — Enregistrement vocal Dify & SMS auto — Score : 6/6 US-02 — Carnet de bord PWA Offline-First 1-Click — Score : 6/6 US-03 — Auto-suivi client QR Code & SMS — Score : 5/6 

User Stories Reportées
US-04 → Score 3/6 → Raison : Le HMW vise la réduction de la charge de travail immédiate et le gain de temps quotidien, pas la comptabilité analytique complexe. US-05 → Score 1/6 → Raison : Hors périmètre MVP, n'adresse ni le gain de temps direct ni les contraintes de faible connexion Internet. 

Décision de sprint
En S3, l'équipe Project A construira 3 user stories dans cet ordre. La démo S6 prouvera le HMW si US-01 fonctionne en live avec une note vocale enregistrée sur un réseau à faible débit.
