# Pizza Classifier

I created a pizza classifier that predicts whether I should order a pizza or skip it.

## Inputs and Labels

The classifier uses two inputs:

- Number of vegetable toppings
- Amount of cheese

The labels are **Order** and **Skip**.

## Development Log

1. **Choosing the idea:** I chose a pizza preference classifier with vegetable toppings and cheese as inputs. My starter examples used 3 toppings with high cheese labeled **Order** and 3 toppings with low cheese labeled **Skip**.
2. **Building the first page:** I asked Codex to create a simple, playful HTML page. It let visitors choose inputs, get a prediction, and label new examples to teach the classifier.
3. **Adding visible evidence:** The first page did not have an evidence table, so I asked for “some evidence—not only an answer.” Codex added a table showing each example's label and distance, with the closest matches highlighted. I reviewed the updated page, and it looks good.

## How to Open and Test

1. Open [pizza-classifier.html](pizza-classifier.html) in a browser.
2. Choose the number of vegetable toppings and the amount of cheese.
3. Click **What's the pizza verdict?** to see the prediction and evidence.
4. Try adding an example with **Label: Order** or **Label: Skip**, then test again.

The page works offline and requires no installation. Refreshing the page resets the examples.
