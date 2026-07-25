Backlog S3 — Project A

HMW Définitif
Comment pourrions-nous automatiser le suivi des réparations et la gestion client de Judas pour lui faire gagner 2 heures par jour à consacrer à sa famille ?

User Stories MUST
(À construire obligatoirement en S3)

US-01
Story : En tant que Judas, je veux créer un dossier de réparation en 1 clic grâce à une note vocale afin d'enregistrer l'appareil en moins de 30 secondes sans saisie manuelle lourde.
Priorité : MUST
Outil : Dify (IA Agent Vocal) + Bolt.new (PWA)
Effort : Moyen
Adresse : Pain Reliever 2 & Contrainte 2 (Création < 30 sec / Zéro saisie)
Critère d'acceptation : Une note vocale de 10 secondes ("PC HP de Mamadou, écran cassé, 25 000 FCFA") est automatiquement transcrite et structurée sous forme de fiche client complète dans la PWA avec un identifiant unique.

US-02
Story : En tant que Judas, je veux utiliser le carnet de réparation en mode 100% hors-ligne afin de pouvoir gérer mes dossiers même sans connexion Internet à Colobane.
Priorité : MUST
Outil : Bolt.new (PWA / IndexedDB - Offline First)
Effort : Moyen
Adresse : Contrainte 1 (Fonctionnement 100% Offline-First)
Critère d'acceptation : L'application permet la création et la modification de statut de réparation sans réseau, puis met en file d'attente les données pour une synchronisation asynchrone dès le retour de la connexion.

US-03
Story : En tant que Judas, je veux associer une photo du matériel et un identifiant unique au dossier client afin de prévenir les contestations sur l'état de l'appareil.
Priorité : MUST
Outil : Bolt.new (Capture Caméra PWA)
Effort : Faible
Adresse : Pain Reliever 4 (Fiche de dépôt numérique & preuve photo)
Critère d'acceptation : Prendre une photo directe depuis la PWA joint le visuel au dossier du client sous un numéro d'identifiant unique rattaché à son numéro de téléphone.

US-04
Story : En tant que client de Judas, je veux consulter l'avancement de ma réparation via un lien de suivi web unique afin de ne plus avoir à appeler ou déranger Judas durant la journée.
Priorité : MUST
Outil : Bolt.new (Page Web Responsive / Low Data)
Effort : Faible
Adresse : Pain Reliever 1 & Gain Creator 1 (Réduction de 50% du support client)
Critère d'acceptation : Le client accède à une page web ultra-légère via son identifiant/lien pour voir le statut en direct ("Reçu", "En cours", "Prêt à être récupéré").

User Stories SHOULD
(À construire si le temps le permet)

US-05
Story : En tant que client de Judas, je veux recevoir un SMS/WhatsApp automatique contenant le récapitulatif de ma fiche de dépôt dès que mon appareil est enregistré afin d'avoir une preuve formelle.
Priorité : SHOULD
Outil : Dify + API SMS (Twilio/Infobip) / WhatsApp Web Gateway
Effort : Moyen
Adresse : Gain Creator 4 (Image de marque professionnelle)
Critère d'acceptation : Dès qu'une fiche est créée sur la PWA, le client reçoit instantanément un SMS/WhatsApp structuré avec son lien de suivi.

US-06
Story : En tant que Judas, je veux générer un lien de paiement Wave / Orange Money direct pour réclamer un acompte avant l'achat d'une pièce afin de sécuriser ma trésorerie.
Priorité : SHOULD
Outil : Bolt.new + Deep Links Wave/Orange Money
Effort : Moyen
Adresse : Pain Reliever 3 & Gain Creator 3 (Trésorerie fluide & Acomptes)
Critère d'acceptation : Un bouton dans la PWA génère un lien de paiement mobile money pré-rempli avec le montant de l'acompte à envoyer au client.

User Stories COULD
(Roadmap post-MVP)

US-07
Story : En tant que Judas, je veux qu'un répondeur automatique WhatsApp informe mes clients de mes horaires de fermeture après 19h afin de préserver ma vie de famille.
Priorité : COULD
Outil : Bot WhatsApp / Dify Workflow
Effort : Élevé
Adresse : Gain Creator 2 (Frontière étanche vie pro / vie perso)
Critère d'acceptation : Les messages reçus en dehors des heures d'ouverture déclenchent une réponse automatique renvoyant le client vers son lien de suivi web.

US-08
Story : En tant que Judas, je veux imprimer ou générer un étiquetage QR Code à coller sur l'appareil afin de retrouver instantanément la fiche du matériel dans l'atelier.
Priorité : COULD
Outil : Bolt.new (Générateur QR Code)
Effort : Faible
Adresse : Fit Check (Suivi du matériel en atelier)
Critère d'acceptation : Scanner le QR code collé sur le téléphone/PC ouvre directement le dossier de réparation dans la PWA FixIt.

Sprint S3 — Ce qu'on construit en priorité

Semaine 1 : [US-01 + US-02]
Semaine 2 : [US-03 + US-04]
Démo S6 : [Démonstration obligatoire de la création d'un dossier à la voix avec Dify en mode offline (US-01/US-02), de la capture photo de l'appareil (US-03) et de la consultation du statut par le client via le lien web (US-04)].
