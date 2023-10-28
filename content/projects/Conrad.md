+++
title = "Conrad's Game of Life"
slug = "conrad"
+++

This is my personal project implementing Conrad's game of life. This project uses Java and works closely with the Java AWT library.

### Github

https://github.com/stevenzhujr/Conrad/tree/main

### Abstract

This personal project consists of code that simulates Conrad's Game of Life using Java.The main goal of this project is to demonstrate my familiarity with Java as well as learn more about working with graphics.

### Rules

The universe of the Game of Life is an infinite two-dimensional orthogonal grid of square cells, each of which is in one of two possible states, alive or dead, or "populated" or "unpopulated". Every cell interacts with its eight neighbours, which are the cells that are horizontally, vertically, or diagonally adjacent. At each step in time, the following transitions occur:

1. Any live cell with fewer than two live neighbours dies, as if caused by underpopulation.

2. Any live cell with two or three live neighbours lives on to the next generation.

3. Any live cell with more than three live neighbours dies, as if by overpopulation.

4. Any dead cell with exactly three live neighbours becomes a live cell, as if by reproduction.

### Design

In a grid of 10 by 10 cells, each cell is represented by a square. The cell is alive if the square is black, and dead if the square is white.

### How to play

**Changing cells**: Clicking one of the cells will change it from dead to alive and alive to dead. It is possible to change it while the simulation is running, however, it is recommended to pause before changing the board.

**Speed**: Enter an integer from 0-50 into the speed textfield to determine how fast each "turn" is. 0 is the slowest and 50 is the fastest.

**Scramble**: Clicking the scramble button will scramble the board, each square will be randomly set to alive or dead with equal chance for each.

**Pause**: Clicking the pause button will stop the simulation on the turn you are on. Clicking the button again will resume the simulation.

### Demo

``` java
public void renderMarkdown(String md) {
  String html = txtmark.Processor.process(md);
  JEditorPane editor = ...;
  editor.setContentType("text/html");
  editor.setText(html);
}

renderMarkdown("Hey, *this seems* not __too difficult__");
```