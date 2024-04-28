# WordBox release

WordBox is a small RN-application for learning words by [Leitner system](https://en.wikipedia.org/wiki/Leitner_system) ([rus](https://ru.wikipedia.org/wiki/Система_Лейтнера)).

Current repository contains release files in 'release' folder and example of used data in 'data' folder.
Release version for Android compiled for sdk-version 34 with minimal sdk-version 21.

Visit 'screenshots' folder to look how the apps should look:

<div align="center">
    <img src="/screenshots/image1.jpg" width="200px"</img>
    <img src="/screenshots/image2.jpg" width="200px"</img>
</div>

## Data

I recommend collect all your words in excel-file and then export it to <kbd>\*.csv</kbd> file for importing to application.
Data format should be by next row:

1. id (string)
2. word (string)
3. definition (string),
4. tags (string with tags separated by comma)

Id is an identifier of word and very important and unique string. For example, if you want to update word or its definition, you can do it in your excel file, then export to <kbd>\*.csv</kbd> file and import to application. In this case your word will be update with keeping the progress and new words (with new ids) wil be added.

Example of the data you can find in 'data' folder – <kbd>LatineWordsV1.csv</kbd>.

## Backup

You can create backup with your progress of learning and all words. It will be saved as <kbd>WordBox-#{current-date}.json</kbd> file. Then you can upload this file again.
