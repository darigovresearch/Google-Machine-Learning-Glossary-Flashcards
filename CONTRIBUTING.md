# Contributing
To make this project extensible as far into the future as possible we are following certain rules which will also make it possible to programmatically generate new language pairs from existing translations.

Pull requests, corrections & fixes are welcome. Any contributions must be submitted under the same license that the original piece of work  (see below). Take a look at any open issues or submit new ones if there is something that needs to be fixed or added.

Watch our video on how to contribute to open source for a complete overview -> [https://www.youtube.com/watch?v=UWA4wyacY2A](https://www.youtube.com/watch?v=UWA4wyacY2A)

### Translating for other languages
Translations in all languages are welcome. Send a pull request or open an issue any time of day or night.

**Please prepend the tag `[lang-code]` to your issues and pull requests.** For example, `[fr]` for French. This will help everyone pick out things they care about.

We're happy for any contribution in any form, but if you're making more than one major change (i.e. translations for two different languages) it would be super cool of you to make a separate pull request for each one so that someone can review them more effectively and/or individually.

## Folder and Filename conventions
Every language has two files
- a .csv source files for each chapter
- and a .apkg file

The latter is for the output .apkg files after having imported and exported the .csv files via Anki.

**The name of each .csv file has two parts to it:**
1. Google Machine Learning Glossary
2. .csv

**Explanation**
1. is literally `Google Machine Learning Glossary` translated into the language that the flashcards are in,
2. is the extension file to make it readable by the correct text editors (here it is a csv file)

**The name of each .apkg file has three parts to it:**
1. Google Machine Learning Glossary
2. (Darigov Decks)
3. .apkg

**Explanation**
1. is literally `Google Machine Learning Glossary` translated into the language that the flashcards are in,
2. a way to designate that the Anki Flashcards comes from a larger body of work (Darigov Decks, see our other works),
3. is the extension file to make it readable by Anki-based software (here it is an Anki Package file)

## Requesting a new language
You can request a language via an issue request with the following title `[lang-code]: Language Request` and body text:

```
*New language has been requested, having the following title and words in *New language* to build out the source file would be helpful to begin the translation

1. Google Machine Learning Glossary
2. Introduction
```

Supplying the new language translations of all the above  means that we can create the corresponding .csv file to make it easier for you to just translate the content. In the future we hope to have code to auto generate the file structure for you but this is currently work in progress.

## File structure
In general each file has one row for each word or phrase separated by a `|` where the text on each side corresponds to the translation for the word/phrase and the explanation in that language.

The first card is an introductory card which is in the required language. Each card must have `Google Machine Learning Glossary` in the language for that deck appended in brackets on the front of the cards because if a user has more than one Google Machine Learning card in their Anki collection it will not be imported and the user will not know where they can find updates, corrections and improvements to the flashcards. For example `Introduction (Glossaire du Machine Learning de Google)` for the French flashcards.

## Steps for submitting a new translation
The general process for porting existing translations to make a new language pair is the following:
1. Make a fork of the latest version of the repository
2. Download it to your local computer
3. Copy the source files which contains definitions in a language that you speak
4. Rename the filename translating the correct words if required
5. Translate each word/phrase along with it's explanation, leaving the English word in brackets as this is what Google had chose to do when the were translating it into different languages
6. Check your work (it is much easier to make corrections before many people have downloaded your translated flashcards than after)
7. Generate the .apkg file with the correct filename in the app
    - Do so in a fresh desktop Anki profile to ensure that as many new words are imported as possible
8. Make a pull request

## Style Guidelines
- Do make sure punctuation is consistent across translations
    - This includes but is not limited to spaces, brackets, quotation marks, question marks, asterisks, exclamation points, ellipses etc.
- Do follow the naming conventions for file and folder names above
- Do keep the English version of the word in brackets on the left hand side of the `|` for consistency with the other pre-existing translations
- Do ensure that you are using the correct delimiter on each row
- Do not delete or combine multiple translations into one line
- Refrain from adding additional context to a translation as it may not be relevant
- Do not use any online translation tools or dictionaries to help with the translation
    - We want this project to be a human-led endeavour as people tend to understand the context of translation better than computer generated tools
