# ipa-dict-dsl - IPA Dictionaries in DSL format

This repository makes available a collection of IPA dictionaries in DSL format derived from the [IPA Dictionary](https://github.com/open-dict-data/ipa-dict) project. This makes it easy to look up the IPA pronunciation of words in a variety of languages using your favourite dictionary program.

![ipa](https://cloud.githubusercontent.com/assets/9295750/20906588/af21d25c-bafd-11e6-9832-0c70138142b7.gif)

## Format

ABBYY Lingvo DSL is a flexible dictionary format that can be read by dictionary applications such as [Goldendict](https://github.com/goldendict/goldendict) and converted to other formats using tools such as [pyglossary](https://github.com/ilius/pyglossary). There are also a number of tools for creating DSL format dictionaries available in the [dsl-tools](https://github.com/dohliam/dsl-tools) project.

DSL files *must* be saved as UTF-16 to be usable by dictionary programs. The raw source files in this repository are saved in UTF-8 format, which is both significantly smaller in terms of file size, and also readable (and diffable) by git. However, there are fully encoded and compressed `.dsl.dz` dictionaries ready for use available in the [Releases](https://github.com/open-dsl-dict/ipa-dict-dsl/releases) section.

You can also use the `rezip_dsl.rb` and `unzip_dsl.rb` [scripts](https://github.com/dohliam/dsl-tools/tree/master/zip_unzip) provided by the [dsl-tools](https://github.com/dohliam/dsl-tools) repo to encode/compress and decode/uncompress the dictionaries yourself either individually or as a group.

## Data

The data directory contains the dictionaries listed according to [ISO language code](http://en.wikipedia.org/wiki/ISO_639-1).

The basic filename pattern is `[ISO]_ipa.dsl`, with `[ISO]` being the source language ISO code. A list of all available languages is [below](#available-languages).

## Available languages

Filename | Language
-------- | --------
`de_ipa.dsl` | German
`en_US_ipa.dsl` | English (General American)
`eo_ipa.dsl` | Esperanto
`es_ES_ipa.dsl` | Spanish (Spain)
`es_MX_ipa.dsl` | Spanish (Mexico)
`fi_ipa.dsl` | Finnish
`fr_ipa.dsl` | French
`ja_ipa.dsl` | Japanese
`jam_ipa.dsl` | Jamaican Creole
`ma_ipa.dsl` | Malay (Malaysian/Indonesian)
`nb_ipa.dsl` | Norwegian (Bokmål)
`sv_ipa.dsl` | Swedish
`sw_ipa.dsl` | Swahili
`yue_ipa.dsl` | Cantonese
`zh_hans_ipa.dsl` | Mandarin (Simplified)
`zh_hant_ipa.dsl` | Mandarin (Traditional)

## Statistics

### Dictionary size

Language | # of entries
-------- | ------------
`es_ES` | 595899
`es_MX` | 595888
`de` | 278915
`fr` | 245150
`ja` | 221421
`en_US` | 125927
`fi` | 94385
`yue` | 57149
`sw` | 48308
`zh_hant` | 48241
`zh_hans` | 44781
`ma` | 28215
`eo` | 23517
`sv` | 21106
`nb` | 10139
`jam` | 1701

## License

MIT.
