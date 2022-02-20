# Fish and Veggie Fusion

In this project, you are going to build a purchasing pipeline for a bargain fusion restaurant in your city that specializes in fish and vegetables.

There are 5 different actors in this system, and you will write functions in multiple modules of code to have them share data, and in the end, the restaurant will make its final purchases.

1. **Fishing Boat** - This is the source of the fish. The boat catches the fish and makes the fresh catch available to purchasers.
1. **Vegetable Farm** - This is the source of the vegetables. As each crop is haarvested, the farm will sell in bulk to distributors and grocers.
1. **Fishmonger** - The fishmonger purchases fresh fish off the boat, and head chefs around the city visit every morning to get fish for their daily menus.
1. **Grocer** - The grocer purchases bulk vegetables from the farm and resells them to the general public, including chefs from local restaurants.
1. **Fusion Restaurant** - The chefs at Veggish Fusion restaurant purchase fresh vegetables from the grocer, and fresh fish from the fishmonger every day. To keep their prices low, they purchase lower cost food and combine them in tasty ways that people might not expect.

## Project Setup

Run the following commands to create the directory structure and files for the project.

```sh
cd ~/workspace
mkdir veggish
cd veggish
touch main.js fishingBoat.js fishMonger.js farm.js grocer.js veggish.js
```

Then initialize your Git repository and make your first commit.

```sh
git init
git add main.js fishingBoat.js fishMonger.js farm.js grocer.js veggish.js
git commit -m "Initial commit"
```

Then open the project directory in Visual Studio Code.

## The Fishing Boat

Create a branch to design and implement the algorithm for the fishing boat.

```sh
git checkout -b fishing-boat
```

Time to set up the fishing boat. First, you need to think about your data structures.

1. The boat will have many fish.
1. Each fish will be represented by an object.
1. Here are the properties of each fish.
    1. Species
    1. Weight
    1. Price _(prices range from $3.00 to $10.00 per fish)_
    1. Amount _(how many of this species were caught today)_

Open your `fishingBoat.js` module and write some comments describing the data structures that need to be created.

Next, the fishing boat must have a function that the other modules can invoke in order to see today's catch.

1. What would be a good name for a variable to store this function?
1. Does the function need any input to do its job, or does it have access to all the information it needs without a parameter?
1. What would this function return?
1. Make sure you put the `export` keyword in front of the function definition so that other modules can import the function and invoke it.
    ```js
    // Example
    export const functionVariable = (goodParameterName) => {

    }
    ```

Once you have the algorithm defined, commit it.

```sh
git add fishingBoat.js
git commit -m "Fishing boat algorithm defined"
```

Now implement the algorithm as best you can. You won't know if you have the right algorithm until you build out other modules, but that's ok. Professional software developers know to start small with the knowledge that the algorithm is a living thing and will likely have to be adjusted as the project grows.

Perfectionists struggle with this, so if that's you, start adjusting the way you think about your work.
