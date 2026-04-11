# GME_Gxanon_Map_Editeur_Downloads
Public binary releases for GME Gxanon Map Editor (no source code).
v1.0.1 
Ce que j’ai ajouté :
  - Multi-application du type (Object / Ground / New) sur toutes les tuiles sélectionnées en mode
    Nouveaux.
  - Multi-application de la Destination sur toutes les tuiles sélectionnées en
    mode Nouveaux.
  - Les tuiles impactées passent en Modified=True et leur texte devient rouge (comme avant, mais en
    batch).

v1.1.2
Release notes:
  - Amélioration réelle des performances au démarrage (traitement de données optimisé, sans lazy mode).
  - Chargement des maps optimisé:
    - Scan des fichiers `.gme/.ame` en un seul passage.
    - Suppression des rescans de dossiers pour construire l’arbre UI.
    - Déduplication en O(1) (HashSet) pendant le chargement.
    - Réutilisation du `DataContractSerializer` pour réduire le coût CPU.
  - Chargement XML optimisé:
    - Suppression du double parsing systématique.
    - Désérialisation directe des fichiers.
    - Réparation automatique conservée uniquement en cas d’XML concaténé invalide.
  - Suppression du `GC.Collect()` forcé au démarrage pour éviter le gel initial.
