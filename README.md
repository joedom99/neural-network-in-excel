# Building a Neural Network from First Principles in Excel

![Excel](https://img.shields.io/badge/Microsoft-Excel-217346?logo=microsoftexcel&logoColor=white)
![No Code](https://img.shields.io/badge/code-none-success)
![No Macros](https://img.shields.io/badge/VBA%20%2F%20macros-none-success)
![Spreadsheet](https://img.shields.io/badge/works%20in-Excel%20%7C%20Sheets%20%7C%20Numbers%20%7C%20Calc-blue)
![License](https://img.shields.io/badge/license-MIT-green)

A working neural network built entirely in Excel formulas — no Python, no PyTorch, no VBA, no macros. Every weight, activation, and gradient lives in a cell you can click on and inspect.

This workbook is the companion to the article **Building a Neural Network from First Principles in Excel** on the [Marketing Data Science blog](https://blog.marketingdatascience.ai).

## What's Inside

The workbook (`neural_network_in_excel.xlsx`) has five tabs:

| Tab | What it does |
|-----|--------------|
| **README** | Orientation, color key, and the six equations behind the network. |
| **AND_OR_NOT** | A single perceptron solving the linearly separable logic gates AND, OR, and NOT. |
| **XOR_Forward** | A pre-trained 2-2-1 network (two inputs, two hidden neurons, one output) that solves XOR. Forward pass only — every step is a visible formula. |
| **XOR_Training** | The same network trained from random starting weights by gradient descent, one epoch per row, 1,000 rows deep. Includes a loss curve chart. |
| **Playground** | Type in your own weights and watch the predictions update live. Try to solve XOR by hand, or paste in the trained weights and verify they work. |

## How to Use It

Download `neural_network_in_excel.xlsx` and open it in Excel, Google Sheets, Apple Numbers, or LibreOffice Calc. The formulas are standard and should work in any modern spreadsheet program. Start with the AND_OR_NOT tab and work left to right through the tabs.

Click on any cell to see the formula behind it. There is no hidden code — the entire network, including training, is ordinary spreadsheet formulas.

## The Math

The whole workbook is built from six equations:

- **Sigmoid function** — squashes any number to a value between 0 and 1
- **Sigmoid derivative** — the slope, needed for gradient descent
- **Hidden neuron** — weighted sum of inputs, plus bias, through the sigmoid
- **Output neuron** — the same operation, one layer later
- **Loss (mean squared error)** — how wrong the prediction was
- **Update rule** — gradient descent, nudging each weight toward a lower loss

The README tab inside the workbook lists all six in full.

## Related Articles

- [Marketing with Neural Networks: What They Are and How to Use Them](https://blog.marketingdatascience.ai/marketing-with-neural-networks-what-they-are-and-how-to-use-them-3e0114771c40)
- [Neural Networks Explained from First Principles in R](https://blog.marketingdatascience.ai/neural-networks-explained-from-first-principles-in-r-795bc158cf37)

## License

Released under the [MIT License](LICENSE). Free to use, share, and adapt.

## Author

**Joe Domaleski** — [Marketing Data Science blog](https://blog.marketingdatascience.ai)
