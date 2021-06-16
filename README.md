let canvasDiv;

let canvas;

let buttonDiv;

let clearButton;

let sliderDiv;

let slider;

let minSpan;

let maxSpan;
// create canvas UI

canvasDiv = createDiv();

canvas = createCanvas(640, 480);

background(65, 60, 88);
canvas.mousePressed(drawEllipse);
canvas.parent(canvasDiv);
// create button UI

buttonDiv = createDiv();

clearButton = createButton("Clear Canvas");
clearButton.mousePressed(function() {

  background(65, 60, 88);

});
clearButton.parent(buttonDiv);
fill("#f00");
ellipse(mouseX, mouseY, 100);