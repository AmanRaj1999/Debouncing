# Debouncing
## In this example, we have an input field where a user can perform a search. As the user types in the input, we want to perform a search operation. However, instead of triggering the search function on every keystroke, we debounce it to avoid excessive searches.

## The debounce function is a utility function that takes a function and a delay as parameters. It returns a debounced version of the function that will only execute after the specified delay of inactivity.

## The performSearch function is the actual search logic that will be executed after the debounce period. In this example, it simply takes the value from the input field and displays it in a results list.

## Finally, we attach the debounced version of performSearch to the 'input' event of the search input field. This means that when the user types, the debounced function will be called, but it will only execute the search logic once the user has stopped typing for 300 milliseconds (0.3 seconds).

## This way, we avoid performing unnecessary searches during rapid typing and ensure that the search operation is only triggered after a brief pause in input activity.
