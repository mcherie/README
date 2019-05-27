### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces.

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript

function whatToDoForLunch(hungry, availableTime) {
  if (hungry == true ) {
    if ( availableTime < 20 ) {
    console.log("Pick something up and eat it in the Lab.") }
        else if ( availableTime <= 30 ) {
      console.log("Try a place nearby, like Gastown.") }
        else if (availableTime > 30) {
          console.log("Hmm how come? You're in bootcamp so maybe you should reconsider! Pick something up and get back in the lab!")
        }
    }
     if (hungry == false ) {
      console.log("Continue working and wait until you're hungry to think about lunch.") }
  }

console.log("I'm hungry and I have 20 minutes for lunch.");
whatToDoForLunch(true, 20);
console.log("---");

console.log("I'm hungry and I have 50 minutes for lunch.");
whatToDoForLunch(true, 50);
console.log("---");

console.log("I'm not hungry and I have 30 minutes for lunch.");
whatToDoForLunch(false, 30);
console.log("---");

console.log("I'm hungry and I have 15 minutes for lunch.");
whatToDoForLunch(true, 15);

```