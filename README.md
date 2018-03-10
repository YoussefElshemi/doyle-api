# Generate docs using jsDoc
## A example
To use this API, we can apply this example to all of the different methods except the trivia.

```js
const api = require('doyle');
const Doyle = new api()

console.log(Doyle.joke()) // returns the object with a lot of data.
```

An example of the joke:
```js
{ link: 'https://www.reddit.com/r/Jokes/comments/3vwu15/three_blondes_are_walking_through_a_forest/',
  score: 4215,
  part1: 'Three blondes are walking through a forest',
  mature: false,
  author: 'Evertak',
  part2: '...when they spot tracks on the ground. The first blonde says: "Look, those are deer tracks."   The second blonde looks at them and says: "No you\'re wrong, those tracks obviously belong to wolves."   The third blonde thinks for a minute and says: "You\'re both wrong, these are hog tracks, I\'m sure."   They were still arguing when the train hit them.' }
```

For trivia:
```js
const api = require('doyle');
const Doyle = new api()

console.log(await Doyle.trivia()) // returns the object with the stuff
```

An example:

```js
{ category: 'History',
  type: 'multiple',
  difficulty: 'easy',
  question: 'Which famous world leader is famed for the saying, \'Let them eat cake\', yet is rumored that he/she never said it at all?',
  correct_answer: 'Marie Antoinette',
  incorrect_answers: [ 'Czar Nicholas II', 'Elizabeth I', 'Henry VIII' ] 
}
  ```
