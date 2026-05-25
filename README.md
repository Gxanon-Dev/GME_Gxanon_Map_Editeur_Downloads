# Gxanon Map Editor [ Remake AME ]

Gxanon Map Editor est un éditeur de maps orienté Dofus/SWF avec outils de calibration GFX, import/export, édition de cellules, traitement SQL/Lang, et intégration d'un helper Java pour les opérations SWF.

## Points clés
- Édition de maps, cellules, layers et zones
- Calibration GFX pour grounds, objects et nouveaux tiles
- Ouverture et traitement de maps SWF
- Outils SQL, Lang et géoposition
- Zoom unifié et overlays de calibration
- Mise à jour applicative via `update.exe`
- Workflow de publication protégé et packaging renforcé
- Multi-langue ( Francais / Anglais / Espagnole ).

## Modules principaux
- `GME_Gxanon\Main`: démarrage, UI principale, options globales, mises à jour
- `GME_Gxanon\MapEditor`: rendu map, cellules, interactions visuelles
- `GME_Gxanon\Calibration`: calibration GFX, sync SWF, réglages de draw
- `GME_Gxanon\Selector`: sélecteurs de maps, zones, GFX et palettes
- `GME_Gxanon\Patterns Dofus`: structures et traitement des données map
- `GME_Gxanon\SWF`, `GME_Gxanon\FFDec`, `GME_Gxanon\XMLInjections`: pipeline SWF
- `GME_Updater`: exécutable de mise à jour

## Fonctionnalités récentes
- Stabilité renforcée sur l'ajout de tiles SWF en calibration
- Correction du rendu des tiles `Nouveaux` et de l'édition de leurs positions
- Zoom calibration amélioré, prise en charge molette et plage étendue
- Chargement XML/options plus robuste face aux données invalides
- Rendu OpenSWF ajusté sur plusieurs cas de rotation/chargement
- Retrait du système de licence applicative
- Branding visible harmonisé vers `Gxanon`
- Pipeline de release protégé avec zip final automatisé
- panel Auto Tiles et PreScéne.
