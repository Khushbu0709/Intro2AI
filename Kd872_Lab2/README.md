# Pizza Classifier

I created a pizza classifier that predicts whether I should order a pizza or skip it.

## Inputs and Labels

The classifier uses two inputs:

- Number of vegetable toppings
- Amount of cheese

The labels are **Order** and **Skip**.

## Improving the Page

The first version of the page did not have an evidence table. I asked Codex:

> A visitor should see some evidence—not only an answer.

The updated HTML page includes an evidence table showing the labeled examples, their distances from the visitor's pizza, and the closest matches used for the prediction. I reviewed the updated page, and it looks good.

## How to Open and Test

1. Open [pizza-classifier.html](pizza-classifier.html) in a browser.
2. Choose the number of vegetable toppings and the amount of cheese.
3. Click **What's the pizza verdict?** to see the prediction and evidence.
4. Try adding an example with **Label: Order** or **Label: Skip**, then test again.

The page works offline and requires no installation. Refreshing the page resets the examples.
