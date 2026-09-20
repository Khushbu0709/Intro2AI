# Pizza Classifier

I created a pizza classifier that predicts whether I should order a pizza or skip it.

## Inputs and Labels

The classifier uses two inputs:

- Number of vegetable toppings
- Amount of cheese

The labels are **Order** and **Skip**.

## How to Open and Use the Page

1. Find `pizza-classifier.html` in the `Kd872_Lab2` folder and double-click it to open it in a browser. You can also use this [link to the page](pizza-classifier.html).
2. Choose the number of vegetable toppings and the amount of cheese.
3. Click **What's the pizza verdict?** to see the prediction and evidence.
4. Try adding an example with **Label: Order** or **Label: Skip**, then test again.
5. Click **Reset examples** to return to the two starter examples.

The page works offline and requires no installation. Refreshing the page resets the examples.

## How It Makes a Prediction

The classifier remembers pizzas I have already labeled. It starts with these examples:

| Vegetable toppings | Amount of cheese | Label |
| --- | --- | --- |
| 3 | High | Order |
| 3 | Low | Skip |

When a visitor builds a pizza, the classifier compares its toppings and cheese with each labeled example. It combines the differences into a distance score, giving both inputs equal weight across their ranges. A smaller distance means a closer match; zero means the inputs match exactly.

The classifier uses the label of the closest example as its prediction. This approach is called **nearest neighbor**. If equally close examples have different labels, it shows a tie. The evidence table displays the distances and highlights the closest matches so visitors can see the reason for the result. Adding a labeled example can change future predictions.

## One Limitation

The two starter examples are not enough to cover every preference. For example, a pizza with 3 vegetable toppings and medium cheese is equally close to the **Order** and **Skip** examples, so the classifier shows a tie. Labeling that pizza gives it more information.

## Development Log

1. **Choosing the idea:** I chose a pizza preference classifier with vegetable toppings and cheese as inputs. My starter examples used 3 toppings with high cheese labeled **Order** and 3 toppings with low cheese labeled **Skip**.
2. **Building the first page:** I asked Codex to create a simple, playful HTML page. It let visitors choose inputs, get a prediction, and label new examples to teach the classifier.
3. **Improving the explanation:** I asked for “some evidence—not only an answer,” and Codex added a table showing labels, distances, and closest matches. Later, based on my classmate's feedback, I asked Codex to clarify the introductory instructions so visitors know what to choose and which button to click.
