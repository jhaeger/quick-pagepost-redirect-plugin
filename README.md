# Quick Page/Post Redirect Plugin security patch
This is a patched version of the no-longer-supported Quick Page/Post Redirect Plugin. 

## Error Discovery
The security vulnerability was originally reported by NinTechNet here: 
https://blog.nintechnet.com/authenticated-settings-change-vulnerability-in-wordpress-quick-page-post-redirect-plugin-unpatched/

## What This Patch Does
This wrapes the database modification calls in a conditional that checks for admin capabilities of user calling the action. 

This means that users MUST be an admin in order to create or delete redirects using this plugin. 

## Instructions
Download the .zip file (click this => https://github.com/jhaeger/quick-pagepost-redirect-plugin/raw/master/quick-pagepost-redirect-plugin.zip), and upload via the Upload Plugin feature at /wp-admin/plugin-install.php
