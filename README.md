# WoW-crafting-profits
R script to calculate profits on alchemy and other crafting professions

This is a basic R markdown file designed to calculate profits from a crafting profession, based on Trade Skill Master 4's account export feature, and display that information in an interactive table and graph. 

Setup:
1) Download the R markdown file
2) Export your TSM accounting data through the TSM desktop app. You need the purchases and sales files.
2) Edit the raw.sales and raw.expenses objects to read your sales and purchases .csv files from step 2.
3) Run the document.

Currently, the script is set up to calculate alchemy profits for WoW Classic, but it can be customized for other professions by changing the crafts and reagents objects to include item strings from other professions.

Known inaccuracies:
1) If you purchase herbs to turn into potions for your own consumption, those herbs are calculated as purchases alongside the herbs you use for crafting/selling. This biases profits downwards.
2) The script does not account for deposit costs on failed auctions. This biases profits upwards.

Package dependencies: dplyr, tidyverse, pander, lubridate, janitor, Hmisc
