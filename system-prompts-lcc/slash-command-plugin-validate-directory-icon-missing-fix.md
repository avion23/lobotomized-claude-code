<!--
name: 'Plugin validate: icon missing fix'
description: 'Fix: add a square PNG icon; requirements and one-time use.'
ccVersion: 2.1.305
-->
Add a square PNG to the plugin folder at .claude-plugin/icon.png, or set `icon` in plugin.json to the path of a square PNG or JPEG in the plugin: 512 to 2048 px on each side, under 2 MB. SVG and WebP are not accepted. That file may become the listing icon only once: the first time the plugin is saved or submitted in the developer portal. Adding or changing it later does not change the icon.
