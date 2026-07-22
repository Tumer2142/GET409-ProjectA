Préparation Jury — HMW — FixIt+

HMW Définitif
Draft S1 : Comment pourrions-nous aider Judas à réduire sa charge de travail pour dégager du temps pour sa famille ?

Définitif S2 : Comment pourrions-nous automatiser le suivi des réparations et la gestion client de Judas pour lui faire gagner 2 heures par jour à consacrer à sa famille ?

Ancrage : Réparateur d'ordinateurs · Feature : Ordinateurs & Téléphones portables.

Résiste au Chapeau Noir : * Un outil digital trop complexe ou nécessitant une saisie manuelle lourde augmentera la charge mentale de Judas au lieu de la réduire.

Le manque de connexion Internet stable ou le coût du forfait data en zone urbaine/périurbaine peut freiner l'adoption quotidienne de la solution.

💡 3 Solutions Actionnables :

L'Agent Vocal Intégré + Dify (Low-Data & Zero Saisie) : Directement dans l'application FixIt, Judas enregistre simplement des notes vocales. L'agent Dify transcrit la note, met à jour le dossier et prévient le client par SMS automatique. Aucune saisie manuelle lourde, très économique en data.

Le Système d'Auto-Suivi par QR Code & SMS (Zéro Interruption) : À la dépose de l'appareil, l'application génère un reçu avec un QR Code ou envoie un lien SMS. Le client consulte l'avancement en autonomie via une page web simple, éliminant les appels incessants.

Le Carnet de Bord PWA "1-Click" (Offline-First) : L'application intègre une interface ultra-simplifiée qui fonctionne sans connexion Internet. Judas change les statuts en un clic. Les données se synchronisent automatiquement dès qu'un réseau est disponible.

🚀 Ce que ce HMW guide en S3 : « Concevoir un assistant virtuel Dify au cœur de l'application FixIt qui permet à Judas de gérer ses réparations et d'informer ses clients à la voix, sans taper de texte et même avec un faible réseau Internet. »

Les 5 Questions Probables
Question 1
Le jury demande : "Comment êtes-vous passés d'un HMW très général sur la réduction de la charge de travail à un HMW mesurable axé sur le gain de 2 heures par jour ?"

Ce qu'il teste : La rigueur de la démarche de design thinking et la capacité à passer d'un besoin flou à une métrique d'impact concrète et évaluable.

Votre réponse : "En S1, notre HMW restait trop vaporeux sur la notion de charge de travail. Lors de la session S2, nous avons quantifié l'impact : les interruptions téléphoniques et la gestion répétitive de la relation client représentent à elles seules plus de deux heures perdues par jour pour un artisan comme Judas. En ciblant spécifiquement l'automatisation du suivi client via le vocal et les SMS, nous avons défini un KPI clair et vérifiable sur le terrain."

Fichier à ouvrir : docs/hmw-definitif.md — section HMW Définitif S2

Question 2
Le jury demande : "Comment votre solution garantit-elle son adoption face aux problèmes d'instabilité du réseau Internet et au coût de la data à Dakar ?"

Ce qu'il teste : L'ancrage territorial de la solution et la prise en compte explicite des contraintes d'infrastructure du marché ouest-africain.

Votre réponse : "Nous avons intégré cette contrainte dès la phase de stress-test du Chapeau Noir. C'est pourquoi notre architecture repose sur une PWA Offline-First avec mise à jour en un clic et synchronisation différée dès qu'un réseau est capté. De plus, pour le client final, la notification passe par SMS classique ou page web ultra-légère, ce qui élimine le besoin d'un forfait data permanent pour les deux parties."

Fichier à ouvrir : docs/hmw-definitif.md — section Résiste au Chapeau Noir

Question 3
Le jury demande : "Pourquoi avoir choisi une interface vocale avec Dify plutôt qu'un formulaire classique de saisie de données ?"

Ce qu'il teste : L'adéquation entre l'expérience utilisateur (UX), les usages réels des artisans locaux et la prévention de la fatigue cognitive.

Votre réponse : "Un formulaire classique exige de saisir du texte au clavier dans un environnement d'atelier souvent encombré et pendant des manipulations techniques, ce qui ajoute de la charge mentale au lieu de la réduire. La note vocale est l'usage naturel le plus répandu via WhatsApp en Afrique de l'Ouest. L'assistant Dify permet à Judas d'actualiser ses dossiers à la voix en quelques secondes, garantissant une saisie à zéro friction."

Fichier à ouvrir : docs/hmw-definitif.md — section 3 Solutions Actionnables (Solution 1)

Question 4
Le jury demande : "Nous constatons des fonctions de paiement mobile et de comptabilité dans votre VPC, mais pas dans votre HMW. Comment expliquez-vous cet écart ?"

Ce qu'il teste : La capacité d'auto-critique et la traçabilité intellectuelle entre la phase d'idéation (6 Chapeaux) et le cadrage du MVP.

Votre réponse : "C'est une divergence exacte que nous avons identifiée lors de notre analyse de cohérence. Le VPC intégrait une sur-conception transactionnelle (paiements Wave, marges sur pièces) qui n'émanait pas de la session des 6 Chapeaux et risquait de complexifier le produit. Conformément à notre HMW, nous avons fait le choix stratégique de recentrer notre MVP S3 sur la décharge mentale et le suivi client, en réservant les fonctionnalités financières à une validation ultérieure sur le terrain."

Fichier à ouvrir : docs/vpc-connections.md — section Synthèse de Cohérence

Question 5
Le jury demande : "Sur quelles bases vous appuyez-vous pour affirmer que la peur de perdre sa clientèle fidèle est un frein majeur pour Judas ?"

Ce qu'il teste : La traçabilité des besoins émotionnels et sociaux de l'utilisateur (Jobs To Be Done) issus des outils méthodologiques.

Votre réponse : "Cette donnée provient de la phase d'analyse par le Chapeau Rouge, qui a mis en évidence le job social de Judas : préserver sa réputation de 'gars sûr' auprès de sa communauté. L'automatisation par QR code et SMS a été précisément conçue pour professionnaliser son image sans rompre le lien de confiance, en rassurant le client par un suivi transparent et continu."

Fichier à ouvrir : docs/vpc-connections.md — section Profil Client — Origines (Jobs To Be Done)

Les 2 Questions Pièges
Piège 1
Le jury demande : "Vous prétendez faire gagner 2 heures par jour à Judas avec des SMS et du vocal, mais si le client ne sait pas lire ou préfère quand même l'appeler au téléphone, votre système s'écroule, non ?"

Pourquoi c'est un piège : Le jury cherche à vous pousser dans vos retranchements sur les réalités socioculturelles locales (analphabétisme, culture de l'appel direct) pour voir si vous avez sur-estimé la technologie.

Stratégie de réponse : Ne pas nier le comportement client, mais recadrer l'usage : le système n'est pas exclusif, il éduque progressivement la clientèle tout en déchargeant la majorité des demandes répétitives.

Phrase d'ouverture : "C'est une excellente remarque qui touche au cœur des habitudes de communication à Dakar, et nous n'avons pas conçu FixIt+ pour changer brusquement la culture locale, mais pour filtrer les interruptions."

Développement : "Lors de la dépose, la remise du recu avec QR code et l'envoi du SMS s'accompagnent d'un message court explicitant au client qu'il recevra une alerte dès que l'appareil sera prêt. Pour les clients ne sachant pas lire, l'enregistrement vocal Dify permet à Judas d'envoyer une note vocale automatique en Wolof ou en Français, éliminant ainsi le besoin de passer 10 minutes au téléphone pour de simples mises à jour."

Piège 2
Le jury demande : "Votre projet ressemble à une juxtaposition de technologies (Dify, PWA, QR Code, SMS). N'avez-vous pas créé une usine à gaz pour un simple réparateur de quartier ?"

Pourquoi c'est un piège : Le jury teste la pertinence technique de votre architecture par rapport au niveau de maturité digitale de la cible (risque de over-engineering).

Stratégie de réponse : Valider le risque soulevé par le jury (en faisant référence à votre analyse Chapeau Noir) puis démontrer que l'ambition technique est masquée derrière une interface utilisateur extrêmement minimaliste ("complexité sous le capot, simplicité en surface").

Phrase d'ouverture : "Nous partageons exactement cette crainte, et c'est précisément le premier risque d'échec identifié par notre Chapeau Noir."

Développement : "Pour Judas, la complexité est totalement invisible : l'interface se résume à trois boutons et un enregistreur vocal '1-Click'. Dify et la PWA fonctionnent en arrière-plan pour traiter la donnée de manière transparente. Ce n'est pas une usine à gaz pour l'utilisateur, mais une infrastructure robuste pensée pour que Judas n'ait jamais à 'apprendre' à utiliser un logiciel complexe."

Réflexe en soutenance
Si vous ne savez pas répondre : "C'est une excellente question sur un point critique de notre cadrage. Si vous permettez, nous allons rouvrir le document docs/vpc-connections.md pour vous montrer exactement comment nos données terrain et nos arbitrages méthodologiques répondent à cette contrainte."
