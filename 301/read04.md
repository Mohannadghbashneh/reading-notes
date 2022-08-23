## What is a ‘Controlled Component’?

An input form element whose value is controlled by React in this way is called a “controlled component”.

## Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

We Should update the user responsees as soon as they enter them, to apply making the React state the source of truth.
______________________________________________________________________________
## How do we target what the user is entering if we have an event handler on an input field?

 When you need to handle multiple controlled input elements, you can add a name attribute to each element and let the handler function choose what to do based on the value of event.target.name.

## Why would we use a ternary operator?

 to write an if statement with only one line of code.

## Rewrite the following statement using a ternary statement: if(x===y){ console.log(true); } else { console.log(false); }

solution:

x===y ? console.log(true) : console.log(false);