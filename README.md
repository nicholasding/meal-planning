Meal Planning
=============

It is often frustrating to plan ahead meals for a week. I am trying to automate the process by introducing a meal planning algorithm.

Problem Statements
------------------

* I want to generate a meal plan for a week or a month
* I want to optimize the cost of ingredients and achieve more diversity on meal
* The following constraints need to be satisfied
 * Same meal can't appear on adjacent days
 * Meals should show an uniform distribution during given time period

Something nice to take into consideration

* Fruits
* Seasonality (affects type of ingredients)
* Cooking time (complexity)

Algorithm Design
----------------

DataSet

```
INGREDIENTS = { 'Onion', 'Cabbage', 'Lamb', 'Beef' ... }
RECIPES = { Recipe('红烧肉', ['Pork']), Recipe('羊肉火锅', ['Lamb', 'Cabbage', 'Corn']) ... }
```

API

```
plan = MeanPlanner(RECIPES)
plan.ingredients # List of ingredients to buy
plan.meals       # List of recipes
```
