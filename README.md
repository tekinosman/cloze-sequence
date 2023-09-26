# Cloze Sequence

Anki template for reviewing lists, enumerations and procedures.

## Features

- All items on a given card are reviewed in the same session and can be shown/hidden by directly clicking on them.
- The review order can be sequential or random.
- Support for custom delimiters.

## Installation

1. Download the [cloze-sequence package](https://github.com/tekinosman/cloze-sequence/raw/main/cloze-sequence.apkg)
2. Import it to Anki. On desktop, go to *File > Import...* and select *Packaged Anki Deck/Collection* as the filetype. On mobile (Ankidroid), tap on the three dots, then on *Import* and select the cloze-sequence package.

This will import the template/note type along with a sample card inside the Default deck.

## Usage

To create an item, the text needs to be enclosed with *@@@three at signs@@@* by default. For example:

    The three main types of rocks are @@@igneous@@@, @@@sedimentary@@@ and @@@metamorphic@@@.

The delimiters can be changed by clicking on the *Cards...* button inside the editing screen, and editing the START/END/type values to suit your needs:

```JavaScript
    delimiter = {
        START: "{{", // To use {{}}
        END: "}}",    // as
        type: "token"   // delimiters
    }
```
    
or this:

```JavaScript
    delimiter = {
        START: "b", // To use <b></b>
        END: "b",    // HTML tags
        type: "tag"   // as delimiters
    }
```

## FAQ

### Why is @@@ used as the default delimiter?

Because it is unlikely to conflict with other symbols or formats.

## Contributing

If you want to contribute, you can submit an issue or a pull request. Follow these guidelines before doing so.

### Submitting an issue

Issues are for reporting bugs, asking questions or suggesting new features.

### Feature requests

Feature requests might be taken into consideration, but they should be within the scope of the template.

## License

Licensed under the [MIT](LICENSE) license.
