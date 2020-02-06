# Azure theme replacement if theme is not used

This package removes the unused OXID Azure theme package from the shop and prevents conflicts in later updates.

## Install

if the Azure theme is not used and should be removed from the shop installation

* Activate an other theme as the Azure theme (and its childs) in the shop backend.
* Run this composer statement in your shop. Adjust this instruction if your installation requires it.

    `composer require d3/oxid-azure-theme-replacement --update-no-dev`
    
* Manually remove the files from source/Application/views/azure and source/out/azure.

## Uninstall

if the Azure theme is to be used again

* Manually clean up the replacement module entry (d3/oxid-azure-theme-replacement) from the vendor/composer/installed.json and composer.lock files.
* Run this composer statement in your shop. Adjust this instruction if your installation requires it.

    `composer remove d3/oxid-azure-theme-replacement --update-no-dev`
