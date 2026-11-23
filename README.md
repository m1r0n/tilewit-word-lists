# Tilewit word lists

The word lists of the word game [Tilewit](https://tilewit.com): for each game language, the words the game accepts as
guesses (`allowed-guesses.txt`) and the secret answers of the easy, medium and hard tiers (`easy.txt`, `medium.txt`,
`hard.txt`), for 5 and 6 letters.

```text
<language>/<n>-letter/allowed-guesses.txt
<language>/<n>-letter/easy.txt
<language>/<n>-letter/medium.txt
<language>/<n>-letter/hard.txt
attribution.json
licences/
```

## How the lists are made

The lists are generated from the sources below; nothing is added by hand. The generator lowercases every word, folds
ligatures (œ to oe), strips accents except letters of the game keyboard (ñ, õ, ä, ö, ü), drops words with any other
character, and expands Hunspell dictionaries into their word forms. Answers are the allowed guesses that the frequency
source knows, ranked by frequency, minus inflected forms, proper nouns, foreign words and offensive or vulgar words. The
easy tier is the most frequent part of the medium tier, which is the most frequent part of the hard tier.

**The lists were changed from the sources:** filtered, folded, expanded and ranked. They are not the original source
files.

## Sources and licences

### English

| Source | Author | Licence | Used for |
| :--- | :--- | :--- | :--- |
| [ENABLE2K word list](https://github.com/dolph/dictionary) | Alan Beale, M. Cooper and contributors | [Public domain](https://creativecommons.org/publicdomain/mark/1.0/) | allowed-guesses, answer-filter |
| [SCOWL en_US Hunspell dictionary](https://wordlist.aspell.net/) | Kevin Atkinson and contributors | [SCOWL licence (MIT-like)](https://wordlist.aspell.net/scowl-readme/) | answer-filter |
| [SCOWL word lists up to size 80 (huge)](https://wordlist.aspell.net/) | Kevin Atkinson and contributors | [SCOWL licence (MIT-like)](https://wordlist.aspell.net/scowl-readme/) | allowed-guesses |
| [Wordnik Wordlist](https://github.com/wordnik/wordlist) | Wordnik | [MIT](https://github.com/wordnik/wordlist/blob/46e6215d0f90356afe9c8ba4be347e7e98cb425c/LICENSE) | allowed-guesses |
| [Wiktionary, English entries (Wiktextract extraction)](https://kaikki.org/dictionary/English/) | Wiktionary contributors; extracted by Tatu Ylonen's Wiktextract (kaikki.org) | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) | allowed-guesses |
| [FrequencyWords (OpenSubtitles 2018)](https://github.com/hermitdave/FrequencyWords) | Hermit Dave | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) | answer-ranking |
| [List of Dirty, Naughty, Obscene, and Otherwise Bad Words](https://github.com/LDNOOBW/List-of-Dirty-Naughty-Obscene-and-Otherwise-Bad-Words) | Shutterstock and contributors | [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) | profanity-filter |
| [Profanity List](https://github.com/dsojevic/profanity-list) | David Sojevic | [MIT](https://github.com/dsojevic/profanity-list/blob/c27924319aa9bd6f917e3782b4f4b6604a50b652/LICENSE) | profanity-filter |

Licences of the derived lists:

- Allowed guesses: CC BY-SA 4.0
- Answer tiers: CC BY-SA 4.0

### Estonian

| Source | Author | Licence | Used for |
| :--- | :--- | :--- | :--- |
| [Eesti sõnastik Hunspellile (et_EE)](https://github.com/LibreOffice/dictionaries/tree/master/et_EE) | Jaak Pruulmann, on the basis of the word list of the Institute of the Estonian Language (EKI) | [LGPL 2.1 + EKI licence](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) | allowed-guesses, answer-filter |
| [Vabamorf morphological lexicon](https://github.com/Filosoft/vabamorf) | Filosoft | [LGPL 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) | allowed-guesses, answer-filter |
| [Wiktionary, Estonian entries (Wiktextract extraction)](https://kaikki.org/dictionary/Estonian/) | Wiktionary contributors; extracted by Tatu Ylonen's Wiktextract (kaikki.org) | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) | allowed-guesses |
| [FrequencyWords (OpenSubtitles 2018)](https://github.com/hermitdave/FrequencyWords) | Hermit Dave | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) | answer-ranking |

Licences of the derived lists:

- Allowed guesses: CC BY-SA 4.0, LGPL 2.1, LGPL 2.1 + EKI licence
- Answer tiers: CC BY-SA 4.0, LGPL 2.1, LGPL 2.1 + EKI licence

### French

| Source | Author | Licence | Used for |
| :--- | :--- | :--- | :--- |
| [Dictionnaire orthographique français « Classique » 7.7 (Grammalecte)](https://grammalecte.net/) | Olivier R. and the Grammalecte contributors | [MPL 2.0](https://www.mozilla.org/MPL/2.0/) | allowed-guesses, answer-filter |
| [Dictionnaire orthographique français « Toutes variantes » 7.7 (Grammalecte)](https://grammalecte.net/) | Olivier R. and the Grammalecte contributors | [MPL 2.0](https://www.mozilla.org/MPL/2.0/) | allowed-guesses |
| [Wiktionary, French entries (Wiktextract extraction)](https://kaikki.org/dictionary/French/) | Wiktionary contributors; extracted by Tatu Ylonen's Wiktextract (kaikki.org) | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) | allowed-guesses |
| [Lexique 3.83](https://www.lexique.org/) | Boris New and Christophe Pallier | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) | answer-ranking |
| [List of Dirty, Naughty, Obscene, and Otherwise Bad Words](https://github.com/LDNOOBW/List-of-Dirty-Naughty-Obscene-and-Otherwise-Bad-Words) | Shutterstock and contributors | [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) | profanity-filter |

Licences of the derived lists:

- Allowed guesses: CC BY-SA 4.0, MPL 2.0
- Answer tiers: CC BY-SA 4.0, MPL 2.0

### Spanish

| Source | Author | Licence | Used for |
| :--- | :--- | :--- | :--- |
| [Diccionario es_ES para Hunspell (RLA-ES)](https://github.com/sbosio/rla-es) | Santiago Bosio and the RLA-ES project | [MPL 1.1](https://www.mozilla.org/MPL/1.1/) | allowed-guesses, answer-filter |
| [Diccionario es_GQ para Hunspell (RLA-ES)](https://github.com/sbosio/rla-es) | Santiago Bosio and the RLA-ES project | [MPL 1.1](https://www.mozilla.org/MPL/1.1/) | allowed-guesses |
| [Wiktionary, Spanish entries (Wiktextract extraction)](https://kaikki.org/dictionary/Spanish/) | Wiktionary contributors; extracted by Tatu Ylonen's Wiktextract (kaikki.org) | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) | allowed-guesses |
| [FrequencyWords (OpenSubtitles 2018)](https://github.com/hermitdave/FrequencyWords) | Hermit Dave | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) | answer-ranking |
| [List of Dirty, Naughty, Obscene, and Otherwise Bad Words](https://github.com/LDNOOBW/List-of-Dirty-Naughty-Obscene-and-Otherwise-Bad-Words) | Shutterstock and contributors | [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) | profanity-filter |

Licences of the derived lists:

- Allowed guesses: CC BY-SA 4.0, MPL 1.1
- Answer tiers: CC BY-SA 4.0, MPL 1.1

The full licence texts are in [`licences/`](licences/). `attribution.json` holds the same data as this README in a
machine-readable form; the app's licences screen shows it.

This is not legal advice. A list that is made from a share-alike source is available under that source's licence, as
listed above.

## Suggest a word

Missing a word, or found an answer that should not be one? [Open a word suggestion](https://github.com/m1r0n/tilewit-word-lists/issues/new?template=word-suggestion.yml). Say the language,
the word, and whether it should be added or removed and why.

Accepted suggestions change the lists in the next app release:

- An answer that should not be one goes on the game's answer blocklist. It stays a valid guess.
- A missing word, or a wrong word in the allowed guesses, is reported to the source dictionary listed above, so the fix
  reaches everyone who uses it, and comes into the game with the next source update.

Repository: https://github.com/m1r0n/tilewit-word-lists
