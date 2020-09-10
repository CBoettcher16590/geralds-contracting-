
# Geralds Contracting Application
![Gerald]

---

## How to Use this Application
To Run a calculation, pass in two parameteres
*  The width of the House (Preceesing by the `-w` flag)
*  The length of the House (Preceesing by the `-l` flag)

Example:

```
node dist/index.js -w 8 -l 8 
```
---

## Developing Instructions
Downlaod this from Github:

```
git clone git@github.com:CBoettcher19590/geralds-contracting-.git
```

---

## Summary 
This assignment is designed to have you demonstrate your newly learned skills from your first two
classes in the “Developing Software: Introduction” course. You will be using all of the live coding skills
that you were taught.

## Outcome 
The finished project will be a small command line interface (CLI) program, written in TypeScript,
compiled to JavaScript. Once you have completed your program, compress the contents of your working
folder (the folder you wrote your program in) by turning it into a .zip file (or other compression type)
which will be submitted as the result of the assignment in teams.

## Senario
Gerald owns a construction company and builds single room homes. He can quickly create a rectangular
house, usually within one day. He has found, however, that he spends a good amount of time calculating
how much lumber he needs to buy for the walls.

Each corner of the house has a single 4x4 beam that walls can be nailed into and the trusses for the roof
come pre-assembled. The only materials that Gerald needs to bring with him are the 2x4’s.

Gerald has decided to commission you to build him a simple application to calculate the number of 2x4’s
he needs to buy so that he doesn’t have to make two trips to the store, but doesn’t buy too much. He’s
given us the following information to help us calculate:

  * Each wall has 2x4’s flat against the floor for the length of the edge of a wall
  * Each wall has vertical 2x4’s spaced 16 inches apart (measured from outside edge of a board to
the next outside edge; the board is included in the 16 inches)
  * Each wall has 2x4’s flat against the ceiling for the length of the edge of a wall
  * Gerald buys 10% MORE than a perfect calculation to account for waste
  * Gerald notes that you can’t purchase a partial piece of lumber, so round up a decimal in the final calculation
  * 2x4’s are actually 1.5" x 3.5”
  * 4x4’s are actually 3.5” x 3.5”
  * Gerald only buys 8’ 2x4’s

  Gerald gave us an example with the expected output as well, using an 8’ by 8’ house: 
 
  * Each wall is the same size in this case
  * Each wall has two beams, totaling 7”, so the space in between is 7’ 5”.
  * Each wall required one 2x4 on the top, bottom, and sides
  * The remaining space across, broken into 16” sections, is 5.56, rounded up to 6.
  * Total: 10 boards per wall, 40 boards for this house

---

| House Measurements | Studs Required | Application Returns | Last Test Run By |
| ------------------ | -------------- | ------------------- | ---------------- |
| 8 x 8              | 40             |  44                 | Colby Boettcher  |
|18 x 8              | 66             |  66                 | Colby Boettcher  |


---



## Note to Developers

I used the [Yargs Package] for the processing of the command line parameters. For more information on that package go to the [Yargs Package] website.  

[Yargs Package]: https://www.npmjs.com/package/yargs
[Gerald]: https://images.unsplash.com/photo-1567615882203-818c7a0508e2?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=788&q=80 

 