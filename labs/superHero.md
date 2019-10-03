In this Task creat a repository of your favourite superheros and displayed them on the console. Applying the functional programming principles we learnt yesterday.

### Ready to get started?

In this Task, we will make an IIFE for a superheros repository and make sure you have the most basic functionality needed to return all data and add data.

### Directions

Step 1:  Create a folder `superheros` In the “scripts.js” file of your project, wrap your repository array in an IIFE to avoid accidentally accessing the global state.

Step 2: Inside that IIFE, before anything else, create a new repository variable to hold what your IIFE will return.

Assign the IIFE to superHeroesRepository.
Since this is now going to be your Pokémon repository, move the repository variable and the entire array assigned to it inside the IIFE assigned to pokemonRepository.
The IIFE should return an object with the following public functions assigned as keys:
getAll: return all items. (superHeroesRepository.getAll(); should return an array of Pokémon.)
add: add a single item. (superHeroesRepository.add(item); should add the item (technically, a superhero).)
Make sure both functions are defined separately with the function keyword and that the return keyword returns only an object with the same names for keys as values.

Step 3: Outside of and below the IIFE, you should already have a `for loop` that iterates over each Super Hero in the repository; however, since you’ve limited access to the repository array that’s inside the IIFE (so that it’s only accessible through one of the two functions returned by the IIFE), you need to update the loop code to cope with the new changes. Essentially, you need to use one of the two functions returned by the IIFE in order to retrieve the repository array.

If all has gone well, console.log your respository and you should see a list of all superheros. It’s also much more stable and ready to grow into a real app!

Step 4: Submit the link to your GitHub repository here. Feel free to share additional thoughts or ask questions on your submissions page.

### Task 2

Want even more practice? You may have noticed that the add() function lets you add anything to the repository. You can even add strings or numbers. That’s not good. In a real application, you’d want to make sure a repository can only be modified with the correct type of data. Inside the add function, you can check if the `typeof` parameter is an object. In combination with a conditional, make sure you can only add the parameter to the repository if it’s an object.
In addition to the type, you can also validate whether all `Object.keys()` of the parameter are equal to the specific keys you expect.

If you’re feeling truly adventurous, you can take a look at how `filterByName()` works and create a whole new public function for superHerosRepository that allows you to find specific superhero only by name.

Also `filterByPower()` receives a string and searches and `console.log` the output. 

