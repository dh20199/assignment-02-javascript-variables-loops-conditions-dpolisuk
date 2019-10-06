# Reflection

## Question 1 (50 words)
#### When and why should you use a function like `carefulSubract` rather than `subtract`? 

Before subtracting the parameters, `carefulSubtract` checks to make sure they are both in fact numbers. `subtract` uses its parameters without firstly checking their data types. Since it checks, `carefulSubtract` will always run regardless of the data types given as parameters but `subtract` will crash if it is not given numbers. You would therefore use a function such as `carefulSubtract` when you are unsure what data types it will recieve as its parameters.

## Question 2 (100 words)
#### What are `data types`, and how does data typing work in JavaScript? Name at least 4 built-in data JS data types. 

`data types` refer to the type of information varibales can hold. In JavaScript, `data types` are dynamic. This means that if you intially declare a variable as a `number`, you can redefine it to be a `string` for example. Four built-in JavaScript `data types` are `number`, `string`, `object`, and `boolean`. `number` represents a quantity with or without decimals, `string` refers to a list of characters, `boolean` refers to a true or false value, and `object` refers to a list of different variables and their values. For example, `1` is a `number`, `'hello'` is a `string`, `true` is a `boolean`, and `date = {month:'October', day:8}` is an `object`.

## Question 3 (100 words)
#### What is the advantage to storing information as an object (`{firstName: 'Italo', lastName: 'Calvino', profession: 'novelist' }`) rather than as an array (`['Italo', 'Calvino', 'novelist']`)? Are there any disadvantages?

The advantage to storing information as an object as oppose to an array is that each element is clearly defined. For example, to access the first name of the novelist in the object you would use `object.fistName` and in the array you would use `array[0]`. Using the object version makes the code more readeable to other people who are reading or developing your code. Another human would easily understand what `object.firstName` represents but would have a more difficult time figuring out what `array[0]` represents. However, the disadvantage to storing information in objects is that it takes up more space and therefore takes longer to process. Another disadvantage to storing information as an object is that it becomes less dymanic. It only makes sense to use `object.fistName` to hold first name information but `array[0]` can hold other information later on.

## Question 4 (150 words)
#### The function `sentences` transforms a data structure (in this case, a list of object literals) into a sequence of sentences. If the data structure were less predictable (e.g., if some properties of each object were occasionally missing, or if their data type was not always the same), what programming techniques could you use to ensure that your function produced a coherent output? Also, can you think of a more interesting "transform" that could be done with the same data structure?

In order to ensure that the function produced a coherent output, I could have tested the data types of the parameters. I could cheack that each element in `list` does in fact have a `fullName`, `party`, `to`, and `from`. I could also check that `fullName` and `party` are both a `strings` and that `to` and `from` are both four digit `numbers` between 1867 and present. In order to do this, I would use the built-in function `typeof` to check the data types and `if` statements to see if the variables are in range.

You can use the data in the list of Prime Ministers to sort the Prime Ministers by time in office. This is interesting since it can teach historians about the time period. For example, William Lyon Mackenzie King was Canada's longest serving Prime Minister and he served during the Second World War. This information can be used to build an argument that Canadians wanted political stability while fighting the war.