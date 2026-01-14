This project demonstrates the fundamentals of CSS Grid using a simple HTML and CSS setup. It focuses on grid structure, spacing, alignment, and item positioning.

 Features Covered

CSS Grid container setup

Fixed-size grid columns and rows

Row and column gaps

Item alignment (horizontal & vertical)

Individual item alignment using align-self

Centering grid content inside the viewport

📂 Project Structure
css-grid-example/
│
├── index.html
└── README.md

🧱 HTML Structure
<div class="container">
    <div class="items item-4">1</div>
    <div class="items item-2">2</div>
    <div class="items">3</div>
    <div class="items item-4">4</div>
    <div class="items">5</div>
</div>


.container → Grid parent

.items → Grid children

.item-2 → Demonstrates individual item alignment

🎨 CSS Grid Explanation
.container {
    border: 2px solid black;
    display: grid;
    width: 80vw;

    grid-template-columns: repeat(4, 80px);
    grid-template-rows: repeat(4, 80px);

    row-gap: 10px;
    column-gap: 10px;

    justify-items: center;
    align-items: center;

    justify-content: center;
    align-content: center;

    height: 100vh;
}

.items {
    height: 55px;
    width: 55px;
    border: 2px solid red;
}

.item-2 {
    align-self: self-end;
}

🔍 Key Concepts Used
1. Grid Container
display: grid;


Turns the container into a grid layout.

2. Grid Columns & Rows
grid-template-columns: repeat(4, 80px);
grid-template-rows: repeat(4, 80px);


Creates a 4×4 grid with fixed sizes.

3. Grid Gaps
row-gap: 10px;
column-gap: 10px;


Adds spacing between grid cells.

4. Item Alignment

justify-items: center; → Horizontal alignment

align-items: center; → Vertical alignment

5. Grid Alignment Inside Container

justify-content: center;

align-content: center;

Centers the entire grid within the viewport.

6. Individual Item Control
align-self: self-end;


Overrides alignment for a single grid item.

🚀 How to Run

Clone the repository

Open index.html in any modern browser

Resize the window to observe grid behavior

📖 Best For

CSS Grid beginners

Frontend practice

Interview preparation

Learning layout alignment concepts

📜 License

This project is open-source and free to use for learning purposes.
