 ### Code:


function setup() {
  createCanvas(1280, 917);
  background(0);
}

let x = 0;
let y = 0;
let spacing = 10;

function draw() {
  let randomNum1 = random(1);
  let randomNum2 = random(1);
  if (randomNum1 < 0.333)
  {
    stroke(255, 0, 0);
  }
  else if (randomNum1 > 0.667)
  {
    stroke(0, 0, 255);
  }
  else
  {
    stroke(0, 255, 0);
  }
  
  if (randomNum2 > 0.5)
  {
    line(x, y, x+10, y+spacing);
  }
  else
  {
    line(x, y+spacing, x+spacing, y);
  }
  x += spacing;
  if (x > width)
  {
    x = 0;
    y += spacing;
  }
}

### Image:

![Imgur]([Imgur](https://i.imgur.com/dpgmvqX.png) "Pattern 1")
