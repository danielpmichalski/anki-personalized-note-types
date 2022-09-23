# anki-personalized-note-types
This repo holds Anki SRS personalized note types as Anki deck export file

## How to use?
1. Import the `tmp.apkg`
2. Delete the imported `tmp` deck
3. Use newly imported note types

## Fields description
- **front**: used for front side of cards
- **back**: used for back side of cards
- **question**: same as `front`, but used by note types without reverse cards
- **answer**: same as `back`, but used by note types without reverse cards
- **text**: field used by Cloze type of notes
- **source**: used for specifying the source of information included in the note

## Note types
- **basic-with-context** (fields: {question, answer} + tags as context)
- **basic-with-context-source** (fields: {question, answer, source} + tags as context)
- **basic-reversed-with-context** (fields: {front, back} + tags as context)
- **basic-reversed-with-context-source** (fields: {front, back, source} + tags as context)
- **cloze-with-context** (fields: {text} + tags as context)
- **cloze-with-context-source** (fields: {text, source} + tags as context)

## Conventions
- for code/programming related cards: use HTML's &lt;code&gt; tag, e.g. &lt;code&gt;testMe()&lt;/code&gt; -> <code>testMe()</code>
