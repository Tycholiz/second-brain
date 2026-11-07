
A hierarchy of decks can be created by separating the deck names with `::`
- ex. name a new deck `Languages::French::Verbs`

## Terminology
### Notes/Cards/Fields
A *note* is a set of information from which *cards* can be made

Imagine we had the following 3 *fields*:
```
Bonjour
Hello
  Page #12
```
- these 3 fields together combine to make up a *note*. Order of the fields does not matter, because we cannot review a *note*. Notes only exist so that we can create cards from them.

From this we can make a single card (ie. Basic), we can make 2 cards (ie. Basic and Reversed) etc.

Imagine we wanted 2 cards:
```
Q: Bonjour
A: Hello
   Page #12
```
And:
```
Q: Hello
A: Bonjour
   Page #12
```

To do this, we just need to make 1 note with 3 fields

### Card Type
For Anki to create cards based on our notes, we need to give it a *card type* (ie. a blueprint), which tells it which fields to display on the front and back of each card.

Each type of note can have one or more card types; when you add a note, Anki will create one card for each card type.

Once a card type has been created, every time you add a new note, a card will be created based on that card type. 
- Card types make it easy to keep the formatting of your cards consistent and can greatly reduce the amount of effort involved in adding information. 
- They also mean Anki can ensure related cards don’t appear too close to each other

To add and edit card types, click the “Cards…​” button while adding or editing notes.

Each card type has two 'templates', one for the question and one for the answer.

For example, if we wanted to make a card:
```
Q: Bonjour
A: Hello
   Page #12
```

We could set the template to:
```
Q: {{French}}
A: {{English}}<br>
   Page #{{Page}}
```

Then we could generate 2 cards from 2 card types: `English-French` and `French-English`