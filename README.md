# Cloze Sequence

Anki template for memorization of lists, enumerations and procedures.

## Features

- Cloze items are reviewed in the same session and can be toggled by directly clicking on them.
- The review order can be sequential or random.
- Support for custom delimiters.

## Installation

Download the [cloze-sequence package](https://github.com/tekinosman/cloze-sequence/raw/main/cloze-sequence.apkg) and import it to Anki:

### Desktop

	 Go to *File > Import...* and select *Packaged Anki Deck/Collection* as the filetype. 

### Mobile (Ankidroid)

	Tap on the three dots, then on *Import* and select the cloze-sequence package. 

This will import the template/note type along with a sample card inside the Default deck.


## How to use

By default, a cloze is created by delimiting some text with @@@three at signs@@@, which can be changed by clicking on the Cards... button inside the editing screen, and editing the START/END/type values like this:

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
When reviewing, clozes get toggled by clicking/tapping on them.

## FAQ

### Why is @@@ used as the default delimiter?

Because it is the delimiter with the least chances of being used for other purposes.

## Contributing

I'm not sure there's much to contribute code wise, but it's welcome nonetheless. Keep in mind the following before doing so.

### Submitting an issue

Issue submissions are for bug reports, questions and suggestions.

### Feature requests

Feature requests might be taken into consideration if they don't stray out of the template's scope.

## License

Licensed under the [MIT](LICENSE) license.
