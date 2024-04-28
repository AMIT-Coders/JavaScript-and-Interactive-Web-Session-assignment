# AMIT Coders
## Full-Stack web development Bootcamp
### Milestone: 2 - Assignment


:warning: :warning: :warning: :warning: :warning: :warning: :warning:
```diff
- Implement the jQuery function(s) to create the game (Find the Carrot).
- You have to commit and push your code to GitHub at the end of your assignment.
```
:warning: :warning: :warning: :warning: :warning: :warning: :warning:
***
## Find The Carrot

How to play Carrot in a box: There are four boxes and there is a hidden carrot in one of them. The game aims to end up with the carrot. The player chooses a box and then the box will be unravelled. If the player guesses the box correctly add a point.

![image](https://github.com/AMIT-Coders/JavaScript-and-Interactive-Web-assignment/assets/60690890/606541c7-ce9e-4ee4-9910-f9d75e73ddc1)

> [!NOTE]  
> As shown above, the idea of the game is to randomize the location of the carrot in the boxes.


## How it works 
1. Set up your project.
  a. Create a folder for your project. Inside this folder, create the following files:
```
      index.html  
      styles.css  
      scripts.js
```
2. Write the HTML (index.html).
```
<h1>Find The Carrot</h1>
<button class="shuffle">Shuffle To Start</button>

<div class="container">
  <div class="card raddish"></div>
  <div class="card carrot"><i class="mdi mdi-carrot"></i></div>
  <div class="card lime"></div>
  <div class="card tomato"></div>
</div>


```
3. Style the HTML (styles.css)
```
body {
  display: flex;
  flex-direction: column;
  align-items: center;
  font-family: Montserrat;
  padding: 10em;
}

button {
  padding:20px 60px;
  outline: none;
  background-color: darkorange;
  border: none;
  border-radius: 5px;
  color: white;
  font-size: 14px;
  text-transform: uppercase;
  font-family: Montserrat;
  letter-spacing: 1px;
  cursor: pointer;
  &:hover {
    background: darken(darkorange, 2);
  }
}

.container {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100vw;
  margin-top: 5em;
 
}

.card {
  width: 200px;
  height: 200px;
  background: mediumvioletred;
  order: 1;
  margin: 1em;
  border-radius: 5px;
  border: 5px solid transparent;
  display: flex;
  align-items: center;
  justify-content: center;
  i {
    font-size: 5em;
    color: darken(darkorange, 10);
  }
  &:nth-child(2) {
    background: darkorange;
    order: 2;

  }
  &:nth-child(3) {
    background: limegreen;
    order: 3;
  }
  &:nth-child(4) {
    background: tomato;
    order: 4;
  }

  &.flip {
    background: #ccc;
    i {
      opacity: 0;
    }
  }
}

```
4. Add functionality with jQuery (scripts.js) - Your turn.


***

Update `README.md` todo list below:
- [ ] Find the carrot successfully in random manner.
- [ ] Test manually the functionality.
- [ ] Submit Find the Carrot game on GitHub.

:white_check_mark: Use `git status` to list all new or modified files that haven't yet been committed.

<p align="center">
  <b>Created by</b><br>
  <b>Mohamed Ibrahim Hany</b>
</p>
