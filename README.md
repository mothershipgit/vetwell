# VetWell

Spoke Theme code changes history (changelog): https://github.com/mothershipgit/vetwell/wiki 

### How to update the theme

Shopify can only have one source of truth for the theme code.
If someone was to make changes in this repository and also in the
shopify theme editor then there would be a conflict of two versions
of the same code.

When making changes to the theme code the best approach is to use 
the development store https://vetwell-scientific-dev.myshopify.com/

And there's two ways to make changes to the theme code, via the
shopify theme editor or via an external code editor such as VSCode. 
Either way, the most important thing is to make sure any changes in 
the theme code are saved in this github repository, it will contain
the updated theme code files that will then be used in the live store.

GitHub integration with Shopify Guide: https://shopify.dev/themes/tools/github#how-it-works

![Diagram](https://cdn.shopify.com/s/files/1/0611/4770/9678/files/diagram-2.jpg?v=1642496925)
### Making changes in the Shopify Code Editor

In the shopify theme (https://vetwell-scientific-dev.myshopify.com/), we use a Github app that connects the theme to
this repository, meaning that any changes done via the Shopify theme editor
will be saved in this repository.

Read more about connecting Github with the store: https://shopify.dev/themes/tools/github

In this page, if you click on the commits "commit" link:
![Screenshot 2022-02-03 at 13 41 20](https://user-images.githubusercontent.com/97894133/152344928-a85a314e-c70c-4abc-95f2-d026fc1bbf34.jpg)


You will then see any changes made in the theme editor in Shopify being saved into this repository. This way we will always make sure the code is saved after any updates.
![Screenshot 2022-02-03 at 13 39 29](https://user-images.githubusercontent.com/97894133/152344572-ec6d8bb5-c2f5-44f0-8478-6d70413141f2.jpg)


Read Shopify's documentation on making changes via the code editor: https://shopify.dev/themes/tools/code-editor

### Making changes in an external code editor (VSCode, Webstorm...)

The best approach to making changes to the theme code is to do it
directly in this repository using an external code editor and connecting 
it to the Shopify store, any changes made will be saved in Shopify directly 
and also in this repository.

To get started read SAhopify's documentation: https://shopify.dev/themes/tools/theme-kit/getting-started

To put any code changes into the development store automatically use 
this command in the terminal:
```angular2html
theme watch --allow-live
```

Note: pushing changes automatically will not trigger the github app installed
in the store to store the changes in this repo. You will have to push
the changes via git

### Publishing the new theme into production

These are the steps to put the update theme code live:

1. Download the code files from this repository by clicking in the "Code" tab, then click on "Code" > "Download Zip"
![Screenshot 2022-02-03 at 13 43 52](https://user-images.githubusercontent.com/97894133/152345178-a775f001-9f11-46bb-bf94-6a5df7e185f3.jpg)

2. Log in to the production store (https://vetwell-scientific.myshopify.com/admin/themes?channel=true)
3. Go to the "Theme Library" section and click "Add Theme" > "Upload zip file"
![Screenshot 2022-02-03 at 13 45 08](https://user-images.githubusercontent.com/97894133/152345377-bfb98efa-c4c1-44fd-9cf4-d4f7e8879d57.jpg)
4. Rename the theme to the latest version following this rule `V0122.0 (01=month, 22=year, .0=version)`
5. Publish the theme

### Give access to a developer to make changes to the code

Give a developer access to the development store using Theme Kit Access:
https://apps.shopify.com/theme-kit-access

In the github account for "@mothershipgit" add the developers email to 
the repository so that they can gain access and commit any changes to the 
theme. https://github.com/mothershipgit/vetwell/



