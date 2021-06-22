<!--

  you will write dev strategies in this module basically the same as in Incremental Developments
  the only difference is that there are now more types of tasks, for example:
    `type: css`
    `type: html`
    `type: logic`
    `type: handlers`
    `type: procedures`
    `type: listeners`
    `type: init`
    `type: data`
    ...

  a single user story may require a little bit of code in each of these folders
  it will take some time and practice to get used to this

-->

## Data

```js
 {
   items : [
     { text : 'Item 1', isChecked : true } 

   ];
 }


 const words = {
  query: '',
  filtered: [],
  all: [],
  };
```

## Components

- [ ] Create item

```js
function createLi (toDoString, isChecked = false){ return newLi}
```

## List of items

### HTML

- [ ] unordered list <_ul_>
- [ ] items <_li_>

## Add item

### HTML

Input form

- [ ] <_input type="text"_>;
- [ ] <_input type="submit"_>;

### Listener

- [ ] target element "add-form", event - "submit", function - addItem;

### Handler

- [ ] create file add-item-handler.js;
- [ ] addItem function;
- [ ] should add the item to the list;

## Remove item

### HTML  

- [ ] button inside <_li_>, on the right.

### CSS  

- [ ] red color;
- [ ] rubbish bin icon;
- [ ] hover effect;

## Listener

- [ ] create remove-item-listener.js in folder listenesrs.
- [ ] access button and icon by classname "delete";
- [ ] "click" event;
- [ ] function removeItem;

### Handler

- [ ] create remove-item-handler.js in folder listenesrs.
- [ ] function removeItem;
- [ ] removes the targeted <_li_>.

## Edit item

### HTML

- [ ] button inside <_li_> on the right;
- [ ] <_span contentEditable="false"_>Item 1<_/span_> inside <_li_> to mark the text;

### CSS

- [ ] blue color;
- [ ] pen icon;
- [ ] hover effect;

- [ ] to change style of <_span_> when text is editable;

### Listener

- [ ] create file named edit-item-listener.js
- [ ] listening for class='edit';
- [ ] event - "click";
- [ ] function - editItem;

### Handler

- [ ] create file named edit-item-handler.js
- [ ] function - editItem;
- [ ] edit item by changing contentEditable to "true";

## Mark item done

### HTML  

- [ ] insert empty check-box icon inside <_li_> on the left of item;

### CSS

- [ ] icon changes to put tick when checked;
- [ ] text changes style to strikthrough;

### Listener

- [ ] create file check-item-listener.js;
- [ ] listening for class='check';
- [ ] event - "click";
- [ ] function - checkItem;

### Handler

- [ ] create file check-item-handler.js in handlers;
- [ ] function - checkItem;
- [ ] changes the icon to checked;
