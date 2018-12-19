# Commcare Translation Analyzer and Copier Tool

#### Intro

•	This is an excel VB macro tool that uses exported commcare app latest translation and a previously exported translated excel file as an input and do various analysis, logs erroneous entries (mismatched <output..),identifies and logs changed label keys and changed default English, identifies and logs missing translations and performs coping for correct entries.

•	Allows us not to freeze commcare application building process while translation is in  progress.

•	This tool Allows us to partially update commcare translation in the future with ease. The hectic task of doing translation can happen at different time along the lifeline of app building.

•	Works Great for a huge app with many labels

#### What it does

•	Identify and logs label keys that are not found on the translated excl doc  which are created on the app while translation were on progress.

•	Identify and logs changed or different default English labels found while translation were on progress.

•	Identify and logs  labels with no translation entries for languages which are Amharic, oromiffa and tigregna.

•	Checks on all translated labels input placeholders like <output../> and create a log if there are any mismatch.

•	By Going through all the modules keys if the keys are found on the translated doc and the default English is not changed and translated labels are found for the three languages , the tool copies the translated labels to the exported sheet and creates log entry under "copied log" sheet with the total count on top

#### How to use
Very very simple..

1.	Download this file “Commcare Translation Analyzer and Copier Tool.xlsm” excel document.
2.	Export the latest app translation excel open it via and save it as a format of xlsm. Rename it to Exported_translation.xlsm
3.	open the translated excel file and save it in a format xlsm then name it Translated.xlsm.
4.	Open all three files and enable macro use
5.	Press the button named “Analyze and copy Translations” and wait till finish which is a dialog appearing informing you the finalization. 

#### Log types
1.	Copy Log
2.	ERROR on Placeholder
3.	Keys Not Found
4.	Keys Found but dt English
5.	No Amharic Translations Found
6.	No Oromifa Translations Found
7.	No Tigregna Translations Found

