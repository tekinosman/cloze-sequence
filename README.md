# Cloze Sequence

Anki template for memorization of lists/enumerations/procedures, with the main features being:

- Cloze items are:
  - reviewed in the same session
  - toggled by directly clicking on them
- There is no order of review. Can be sequential or random.
- Custom delimiters.

## Installation

Download the [cloze-sequence package](cloze-sequence.apkg) and import it on Anki (*File > Import...* and select *Packaged Anki Deck/Collection* as the filetype). This will import the template/note type along with a sample card inside the Default deck.

## How to use

By default, a cloze is created by delimiting some text with @@@three at signs@@@, which can be changed by clicking on the Cards... button inside the editing screen, and editing the START, END, token values like this:

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

### Does it work on mobile?

Yes.

## Contributing

I'm not sure there's much to contribute code wise, but it's welcome nonetheless. Keep in mind the following before doing so.

### Submitting an issue

Issue submissions are for bug reports, questions and suggestions.

### Feature requests

Feature requests might be taken into consideration if they don't stray out of the template's scope.

## License

Licensed under the [MIT](LICENSE) license.
