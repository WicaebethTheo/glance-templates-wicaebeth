# glance-templates-wicaebeth
![image](https://github.com/user-attachments/assets/f6a52861-b9d1-40db-b432-2df662283cfa)

![image](https://github.com/user-attachments/assets/95719fee-0efa-4589-a787-998e6402933f)

![image](https://github.com/user-attachments/assets/ea9d33a5-2c5a-4aba-bc16-a9175025e21b)


# Glance Dashboard Configuration

Ce dépôt contient les fichiers de configuration pour le tableau de bord Glance.

## Fichiers templates

Les fichiers avec l'extension `.template` sont des versions des fichiers de configuration avec les clés API et informations sensibles remplacées par des placeholders.

### Comment utiliser les templates

1. Copiez le fichier template que vous souhaitez utiliser (par exemple `homelab.template` → `homelab.yml`)
2. Remplacez tous les placeholders (YOURAPIKEY, YOUREMBYAPIKEY, setyouripservicehere, etc.) par vos propres informations
3. Ajustez les URLs et autres configurations selon vos besoins

### Placeholders à remplacer

Les templates contiennent les placeholders suivants qui doivent être remplacés par vos propres informations:

- `YOURAPIKEY` - Votre clé API Proxmox (format: `root@pam!glance=xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx`)
- `YOUREMBYAPIKEY` - Votre clé API Emby (chaîne de caractères longue)
- `YOURTAILSCALEAPIKEY` - Votre clé API Tailscale (commence par `tskey-api-`)
- `setyouripservicehere` - Vos adresses IP pour les différents services (remplacez par l'IP ou le nom d'hôte approprié)

## Structure des fichiers

- `glance.template` - Configuration principale qui inclut les autres fichiers
- `homelab.template` - Configuration de la page Homelab
- `stargate.template` - Configuration de la page Stargate

## Mise à jour de votre configuration

Pour mettre à jour votre configuration avec les modifications de ce dépôt:

1. Comparez les fichiers template avec vos fichiers YML
2. Intégrez les modifications en préservant vos clés API et personnalisations

original sources from Aylabs : https://github.com/AyLabsCode/glance-templates/tree/main
