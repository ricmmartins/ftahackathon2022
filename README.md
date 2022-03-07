# FTA Hackathon 2022

1. Go to Azure Portal, search by "Deploy a custom template" 
2. Select template > Build your own template in the editor
3. Copy the content from [la-template.json](la-template.json), paste into the editor then save.
4. On Resource Group, create a new one then click to **Review + Create**
5. Repeat the steps 1-2, paste the content from [az-sentinel.json](az-sentinel.json) into the editor then save.
6. On **Resource group** choose the same proviously created, on **Workspace** give the name you prefer then click to **Review + Create**
7. Still on Azure Portal, search by "Deploy a custom template" 
8. Select template > Build your own template in the editor
9. Copy the content from  [environment-template.json](environment-template.json), paste into the editor then save
10. On **Resource group** and **Diagnostics Workspace Resource Group** choose the same proviously created, on **Diagnostics Workspace Name** type the name previously created and on **Diagnostics Workspace Subscription** insert your Subscription ID
11. Click to **Review + Create**
10. Setup Kali Linux following [this instructions](kali.md)
