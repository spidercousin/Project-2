## 2.3: Complex Programming Decisions

### Overview

In this class, students will advance their Python proficiency by exploring match case statements, and refining their ability to make complex programming decisions. They will delve into dictionaries, including nested variants, and apply these data structures to real-world scenarios, enhancing their versatility in Python application development. Furthermore, they'll grasp list comprehensions for efficient list creation and gain practical experience in code refactoring to optimize applications, thereby boosting their industry-valuable skill set.

### Class Objectives

By the end of today's class, the students will be able to:

* Refactor an existing if-elif-else statement into a match case structure.

* Create and manipulate Python dictionaries and effectively iterate through them using `items()`, `keys()`, and `values()`.

* Demonstrate the ability to iterate through complex nested data structures, such as lists within lists and lists of dictionaries.

* Extract specific information from nested dictionaries.

* Use list comprehension and list operations to process data and perform calculations.

---

### Instructor Notes

This module catapults students into the deeper aspects of Python programming, focusing on complex decision-making structures and data manipulation. Prepare to guide students through the newly-introduced match case statements&mdash;a versatile feature for handling multiple match conditions. Knowledge of dictionaries, a crucial Python data structure for intricate data storage, will be introduced in depth. Expect to instruct on generating, accessing, and modifying dictionaries, including nested ones.

Moreover, this module introduces list comprehensions&mdash;a compact and intuitive mechanism to create and modify lists. By module-end, students should feel confident employing these advanced Python topics in their projects. As the course emphasizes practical application, you'll facilitate exercises aiming to resolve realistic challenges, like designing an interactive food truck menu.

In this module, we use Anaconda environments. This curriculum has been tested with Python 3.10, but updates to packages and variances in student machines can still cause conflicts to occur. If a student has an error that you believe to be related to Python 3.10, at your discretion you can instruct them to create a new environment using a different Python version. If you believe that an update has introduced a bug at a curriculum level, attempt to find a suitable workaround for the moment and submit a report using the Boot Camp Feedback Form.

* Students should have installed Anaconda in the previous module. Today, the students will be using Python from their Anaconda installation. Take a moment to ensure that everyone has installed Anaconda.

* Students may find themselves frustrated by some of the quirks of Python. It’s important that you maintain a positive tone and are prepared to help the class fix whatever bugs they encounter.

* Try to identify confused students who may be reluctant to raise their hands and ask for assistance. Also, regularly encourage the class to ask questions whenever they are confused, and reassure them that confusion is simply part of the learning process.

**Important:** Match statements, which are covered in today's class, require a Python environment of at least version 3.10, when match statements were introduced. If you need to brush up on match statements, you may use the [official documentation](https://docs.python.org/3/reference/compound_stmts.html#match) and [Python tutorial](https://docs.python.org/3/tutorial/controlflow.html#match-statements) to do so.

As debugging and troubleshooting are critical skills for students to learn, take advantage of the errors that come up naturally during class in either your code or your students’ code whenever possible. Encourage students to analyze the problem and suggest solutions to each other. Time constraints can make it difficult to troubleshoot every error that arises, especially with larger class sizes. Encourage students to screenshot their code and the error they are getting as soon as something goes wrong. Have them post the screenshots in the “live” channel in Slack, and have TAs and students who are already finished with the activity attempt to troubleshoot the problem. Have your TAs call out any errors that may deserve dedicated class time for troubleshooting.

Even with these best practices in place, some students will have errors that can’t be solved during class time. Make sure TAs are encouraging students to attend office hours for any debugging that they still need help with at the end of class.

---

### Class Slides

The slides for this lesson can be viewed on Google Drive here: [Lesson 2.3 Slides](https://docs.google.com/presentation/d/17y9Uh9dp_jAivYrTiScu29WYkzRK0J9DlVG7O-WNNr8/edit?usp=sharing).

To add the slides to the student-facing repository, download the slides as a PDF by navigating to File, selecting "Download as," and then choosing "PDF document." Then, add the PDF file to your class repository, along with other necessary files. You can view instructions for this [here](https://docs.google.com/document/d/1XM90c4s9XjwZHjdUlwEMcv2iXcO_yRGx5p2iLZ3BGNI/edit).

**Note:** Editing access is not available for this document. If you wish to modify the slides, create a copy by navigating to File and selecting "Make a copy...".

---

### Time Tracker

| Start Time | Number | Activity                                           | Duration |
| ---------- | ------ | -------------------------------------------------- | -------- |
| 6:30 PM    | 1      | Everyone Do: Rock Paper Scissors Warm Up           | 0:10     |
| 6:40 PM    | 2      | Instructor Do: Match Case                          | 0:10     |
| 6:50 PM    | 3      | Students Do: Refactor Rock Paper Scissors          | 0:10     |
| 7:00 PM    | 4      | Review: Refactor Rock Paper Scissors               | 0:05     |
| 7:05 PM    | 5      | Instructor Do: Dictionaries                        | 0:15     |
| 7:20 PM    | 6      | Students Do: Understanding Dictionaries            | 0:10     |
| 7:30 PM    | 7      | Review: Understanding Dictionaries                 | 0:05     |
| 7:35 PM    | 8      | Instructor Do: Iterating Nested Data Structures    | 0:10     |
| 7:45 PM    | 9      | Students Do: Exploring the Nest                    | 0:15     |
| 8:00 PM    | 10     | Review: Exploring the Nest                         | 0:05     |
| 8:05 PM    | 11     | BREAK                                              | 0:15     |
| 8:20 PM    | 12     | Instructor Do: Nested Dictionaries                 | 0:15     |
| 8:35 PM    | 13     | Students Do: Printing a Menu                       | 0:20     |
| 8:55 PM    | 14     | Review: Printing a Menu                            | 0:05     |
| 9:00 PM    | 15     | Instructor Do: List Comprehension                  | 0:10     |
| 9:10 PM    | 16     | Students Do: Guest List                            | 0:10     |
| 9:20 PM    | 17     | Review: Guest List                                 | 0:05     |
| 9:25 PM    | 18     | Instructor Do: Class Wrap Up                       | 0:05     |
| 9:30 PM    |        | END                                                |          |

---

### 1. Everyone Do: Rock Paper Scissors Warm Up (10 min)

**Corresponding Activity:** [01-Evr_Rock_Paper_Scissors](Activities/01-Evr_Rock_Paper_Scissors/)

Briefly recap what was learned in the previous class and explain that we will practice these coding skills together in a group activity. This includes:

* Lists
* `while` loops
* If-elif-else statement
* Nested conditionals
* Logical, membership, and conditional operators

Open up the unsolved file and ask the students to volunteer to provide the code for each step, filling in the unsolved file as you go. If students are struggling to answer, the solution code can be used as a guide.

Briefly point out that the `random` module is being imported into this script. Up until now, we have not imported any modules, but since we are covering module imports and functions in next week's class, you can just use this as an introduction to what the students will be learning more about soon. Simply explain how the code imports a module called `random`, which will allow the computer to make a choice randomly from a list of actions.

When you finish writing the script with the students, run it from the command line to demonstrate it in action. Then, tell the students that they will be refactoring this code in the next student activity, after learning the next concept (match case).

Ask the students if they have any questions and send out the solution, which they can use as a reference for the upcoming refactoring student activity, before moving on to the next demonstration.

---

### 2. Instructor Do: Match Case (10 min)

**Corresponding Activity:** [02-Ins_Match_Case](Activities/02-Ins_Match_Case/)

Continue using the slideshow to accompany this demonstration.

Introduce students to match statements with the following talking points:

* Match statements were only introduced in Python in version 3.10 in 2021, so it is pretty new in Python but adapted from older programming languages’ equivalent switch case statements.

* They are a kind of conditional that checks which of a list of particular cases has been met.

    * Think of a multiple choice question that requires a different response for each answer, either congratulations or specific corrections. Match case checks whether the student inputs a, b, c, or d, and completes the relevant action for the result.

* Match statements can always be written as `if-elif-else` statements instead, but may be preferred to reduce the complexity of the statement. For example, rather than having to write the same variable multiple times in each if/elif line, you can use it in a single match line and then include a case line for each value you want to match.

* There are various complex ways of using match statements, but for the purpose of this class, students only need a basic understanding, matching a single variable.

    * Note that while we’ll only be using what would be the equivalent of the `==` comparison operator, it is possible to use other comparison operators in a match case statement along with an `if` statement. Encourage students looking for an extra challenge to go out and explore this on their own.

* Of course, it is possible that the input isn’t accounted for in any of the specified cases. Here underscore is used as a “catchall” final line if you want the statement to do something when no matches are found.

* The match statement is completed and exited upon the first match. If the `break` keyword is used inside any of the cases, that will break from a loop when the match statement is inside a loop.

* Each `case` line should be nested/indented under the `match` line.

Demonstrate the use of a match case statement by opening up the solution to this activity in VS Code and go over the example:

```python
# Provide exit option
while True:
    # Ask the customer if they would like to order anything else
    keep_ordering = input("Would you like to keep ordering? (Y)es or (N)o ")

    # Check the customer's input
    match keep_ordering.lower():
        # Customer chose yes
        case 'y':
            # Keep ordering
            place_order = True
            # Exit the keep ordering question loop
            break
        # Customer chose no
        case 'n':
            # Complete the order
            place_order = False
            # Since the customer decided to stop ordering, thank them for their order
            print("Thank you for your order.")
            # Exit the keep ordering question loop
            break
        # Customer typed an invalid input
        case _:
            # Tell the customer to try again
            print("I didn't understand your response. Please try again.")
```

Run the script from the command line to demonstrate each case in action.

Ask the students if they have any questions and send out the solution before moving on to the next activity.

---

### 3. Students Do: Refactor Rock Paper Scissors (10 min)

**Corresponding Activity:** [03-Stu_Refactor_Rock_Paper_Scissors](Activities/03-Stu_Refactor_Rock_Paper_Scissors/)

Continue through the slideshow, using the next slides as an accompaniment to this activity.

Before introducing the activity to students, explain code refactoring to them as a process of making improvements on existing code, whilst maintaining the same functionality.

Let students know that they will need to apply their knowledge of nested if-else statements to create nested match statements in order to complete this activity.

This activity will give students practice with refactoring code by converting existing if-elif-else statements into match statements.

---

### 4. Review: Refactor Rock Paper Scissors (5 min)

**Corresponding Activity:** [03-Stu_Refactor_Rock_Paper_Scissors](Activities/03-Stu_Refactor_Rock_Paper_Scissors/)

Open the solution, share the file with the students, and go over it with the class, answering whatever questions students may have. It may be useful to do a side-by-side comparison of the original and refactored code in VS Code to highlight the improvements made.

Cover the following key points during the discussion:

* The first match statement allows us to set the variable `user_full_choice` as the full word of the user's choice so that we can use it in print statements to print out the user's choice. In the original version of the code, this word was hard-coded in each `elif` statement, and the only time the variable was used was when the computer and user choices resulted in a tie.

* Since there are only three options that the `user_choice` variable could be, given that we first check if the choice is in the `options` list, we can use the underscore in place of the third option.

* The second match statement is nested, first checking the user's choice, and then under each user option, the computer choice is matched before deciding what to print. Given that we have taken out the scenarios when the user and computer tie, we only need to include cases where the computer choice does not match the user choice.

Time permitting, ask the students if they can see any other repetition in the code output that could be refactored further. If they don't answer, point out that the result strings and the computer choice strings are used at least twice each, and could be saved as variables, which could then be used when needed.

Note that this learning block was designed to prime students for more complex coding concepts. In the previous lessons, they were introduced to the basic logic of working in Python and now we are beginning to delve into more sophisticated applications of the same rules, first with more sophisticated decision-making trees, as introduced in the block above, and next with more complex data structures in the case of dictionaries.

Ask the students if they have any questions before moving on to the next activity.

---

### 5. Instructor Do: Dictionaries (15 min)

**Corresponding Activity:** [04-Ins_Dictionaries](Activities/04-Ins_Dictionaries/)

Continue using the slideshow to accompany this demonstration, along with the solution code.

There are two solution files used in this demonstration. The first one is `dictionaries_solution.py` to demonstrate how to create dictionaries and access information in them. The second, `dictionary_methods_solution.py`, is used for demonstrating the dictionary methods `keys()`, `values()`, and `items()`.

Stress the importance of understanding dictionaries. Many datasets available to us that we can use when developing machine learning applications will come in a format called JSON or JavaScript Object Notation, which are formatted like Python dictionaries. Let the students know that they will be working with JSON objects and learning how to access them in an upcoming module. Dictionaries are also frequently used when creating and modifying Pandas DataFrames, another topic we will cover in depth soon.

Follow the slides to introduce students to dictionaries.

First cover the following points:

* Dictionaries are a Python data type that stores a collection of data, similar to a list or a tuple.

* Unlike a list or tuple, dictionaries don’t store data just in a particular position but according to a key-value pair.

    *The key is an immutable object that can be used to call its associated value. It is usually a string, but can also be an integer or float. Keys cannot be lists or any other type of mutable object.

    * Real-life dictionary example: The words in the dictionary would be considered the keys, and the definitions of those words would be the values.

* There cannot be duplicate keys in a dictionary. If a value is assigned to the same dictionary key twice in the creation of the dictionary, only the last value assigned is used.

* Values in a dictionary can be objects of any type: 

    * Integers
    * Floating-point decimals
    * Strings
    * Booleans
    * Datetime objects
    * Lists
    * Other dictionaries

Empty dictionaries can be initialized in one of two ways:

* `actors = {}`
* `actors = dict()`

Items can be added to dictionaries initially by creating a key, following it with a colon, and then placing the desired value after the colon. For readability, and following PEP8 conventions, the colon should be right next to the key without a space, but a space should separate the colon and the value.

```python
actors = {"name": "Tom Cruise"}
```

Similarly, those values can be called by referring to the key for the desired value. Call attention to the format being similar to referencing list values, except instead of using the list index value, we use the dictionary's key:

```python
print(f'{actors["name"]}')
```

Items can also be added the same way you would assign a variable. Declare the dictionary name and key by placing the key inside square brackets, and then assigning a value with the equals sign. After this the value can also be changed by assigning a new value to the relevant key:

```python
actors["name"] = "Denzel Washington"
```

The following code captures an example of the use of a list within a dictionary:

```python
# A list of actors
actors_list = [
    "Tom Cruise",
    "Angelina Jolie",
    "Kristen Stewart",
    "Denzel Washington"]

# Overwrite the value, "Denzel Washington", with the list of actors.
actors["name"] = actors_list
```

Items in a list in a dictionary can be accessed by calling the key and then using indexing to access the item. Assure students that they only need a basic understanding of this for now; when they get into APIs, they will get a lot more practice!

```python
# Print the first actor
print(f’{actors["name"][0]}’)
```

Dictionaries can contain multiple pairs and multiple types of information, with each key-value pair separated by a comma. PEP8 conventions suggest it is best to declare each key-value pair on a separate line:

```python
# A dictionary can contain multiple pairs of information
actress = {
    "name": "Angelina Jolie",
    "genre": "Action",
    "nationality": "United States"
}

# A dictionary can contain multiple types of information
another_actor = {
    "name": "Sylvester Stallone",
    "age": 62,
    "married": True,
    "best movies": [
        "Rocky",
        "Rocky 2",
        "Rocky 3"
    ]
}
print(f'{another_actor["name"]} was in {another_actor["best movies"][0]}')
```

* Point out the formatting with the nested items. Each item is indented as per the next block level, and the opening and closing braces (curly braces `{ }` for the dictionary and square brackets `[ ]` for the list) are on different lines. Unlike the necessity of indentation for code, the actual format of indentation within data structures is less strict, though PEP8 does have some guidelines about where to close the brackets in the section on [indentation](https://peps.python.org/pep-0008/#indentation).

Dictionaries can even contain other dictionaries. Demonstrate how to create these dictionaries and reference nested values.

```python
# A dictionary can even contain another dictionary
film = {
    "title": "Interstellar",
    "revenues": {
        "United States": 360,
        "China": 250,
        "United Kingdom": 73
    }
}
print(f'{film["title"]} made {film["revenues"]["United States"]}'" million dollars in the US.")
```

Now that students know how to reference individual pieces of information within a dictionary, demonstrate how to access the contents of a dictionary when they may not know all of the keys contained within it, or the structure of the dictionary. Large dictionaries could be too complex to print out in full in order to discern this information, so there are methods that you can use to access the keys, values, and key-value pairs. These methods can be used to print together, or they can be used to iterate through each one within a loop.

Highlight that `keys()`, `values()`, and `items()` return a list:

* `keys()` returns a list of the key names.

* `values()` returns a list of the values in whatever data type or data structure they’re stored as.

* `items()` returns a list of tuples in the format [(key, value)].

Demonstrate these methods in the solution code provided, both printing them out directly and iterating through them.

Explain that because the `items()` method creates a list of tuples, we need to be able to refer to each part separately when iterating through them. We can do this by what's known as **unpacking** the tuple. This means separating the tuple into its individual components. For example, `key, value = ("name", "Michelle Yeoh")` creates a variable called `key` with the value of `"name"` and a variable called `value` with the value of `"Michelle Yeoh"`. 

Reinforce the importance of unpacking tuples, as it is commonly used in machine learning applications, particularly when separating data into testing and training sets.

Ask the students if they have any questions and send out the solution before moving on to the next activity.

---

### 6. Students Do: Understanding Dictionaries (10 min)

**Corresponding Activity:** [05-Stu_Dictionaries](Activities/05-Stu_Dictionaries/)

Continue through the slideshow, using the next slides as an accompaniment to this activity.

This activity will allow students to practice creating dictionaries and accessing information from them, both directly and iterating through them.

---

### 7. Review: Understanding Dictionaries (5 min)

**Corresponding Activity:** [05-Stu_Dictionaries](Activities/05-Stu_Dictionaries/)

Open the solution, share the file with the students, and go over it with the class, answering whatever questions students may have.

Cover the following key points during the discussion:

* A variable called `my_info` stores the primary dictionary, as noted by the curly braces.

* The keys are `"name"`, `"age"`, `"hobbies"`, and `"wake-up"`; their corresponding values are stored after the colons, with each new key-value pair separated by a comma.

* The `"hobbies"` key stores a list and the `"wake-up"` key stores a dictionary.

* We use a second set of square brackets to access information stored in the nested list and dictionary.

* When iterating through a dictionary's keys and values, we can use a variable name that indicates what information is stored in the dictionary. For example, in the `"wake-up"` dictionary, the key is a reference for the day, and the value indicates the time, so we can use `day` and `time` as the name for the variable when iterating through `keys()` and `values()`, as shown in the following code:

    ```python
    # Use a loop to print out the keys of the wake-up dictionary
    for day in my_info["wake-up"].keys():
        print(day)

    # Use a loop to print out the values of the wake-up dictionary
    for time in my_info["wake-up"].values():
        print(time)
    ```

* When iterating through a nested dictionary, we can refer to that dictionary by the original dictionary's name and its associated key in square brackets before calling the method to iterate through.

Ask the students if they have any questions before moving on to the next activity.

---

### 8. Instructor Do: Iterating Nested Data Structures (10 min)

**Corresponding Activity:** [06-Ins_Nested_Data_Structures](Activities/06-Ins_Nested_Data_Structures/)

Continue using the slideshow to accompany this demonstration.

Call students attention back to what they have learned about data structures and nesting and explain that data structures can also be nested, e.g., a list of lists, a list of dictionaries, and a dictionary with nested dictionaries (this will be covered after the break).

Remind students that they've already encountered a nested data structure when using the list of tuples from the `items()` method.

This section will include examples of nested lists and a list of dictionaries, along with a demonstration of how to iterate through or utilize the data in them.

Example of a list of lists:

```python
[
    ["James", "Noor", "Ayoka"],
    [65, 72, 80],
    ["Washington", "Kuala Lumpur", "Abuja"]
]
```

Example of the same information as a list of dictionaries:

```python
[
    {
        "name": "James",
        "score": 65,
        "city": "Washington"
    },
    {
        "name": "Noor",
        "score": 72,
        "city": "Kuala Lumpur"
    },
    { 
        "name": "Ayoka",
        "score": 80,
        "city": "Abuja"
    }
]
```

Point out that each nested data structure is separated by a comma, the same way you would separate variables in a regular list or dictionary.

Next, open VS Code and demonstrate how to use information stored within these nested data structures, and iterate through them.

#### List of Lists

A list of lists may include the column headings for the first list, with the subsequent lists being individual rows, and each value in the list associated with the heading in the first list. Show this using the example of stock market prices.

```python
table_data = [
    ["Ticker", "Open", "Close"],
    ["AAPL", 363.25, 363.4],
    ["AMZN", 2756.0, 2757.99],
    ["GOOG", 1409.1, 1408.2]
]
```

Demonstrate how to select all of the information for "AMZN". First, remind the students that Python lists use zero-based indexing. The first item in the list is at index position 0, so that means the third item in the list&mdash;in this case, "AMZN"&mdash;is at index position 2.

Explain that we can use normal list indexing to retrieve and print that data, and demonstrate as follows:

```python
amazon_data = table_data[2]
print(amazon_data)
```

The following should appear when the code is run: `['AMZN', 2756.0, 2757.99]`

Next, ask the students if they can figure out what they would need to do to get just the opening price for Amazon. Some students may be able to figure out what to do, as we used a similar method to extract nested information from dictionaries earlier.

If you don't get an answer from the students, you can walk them through it:

* The opening price is at index position 1, so we can simply retrieve the opening price from the inner list, as follows:

    ```python
    amazon_data = table_data[2]
    amazon_opening_price = amazon_data[1]
    print(amazon_opening_price)
    ```

* Explain that Python allows us to take this further and combine these two steps so that we get the value in a single line, like the following example:

    ```python
    amazon_opening_price = table_data[2][1]
    print(amazon_opening_price)
    ```

Running both of the snippets should output `2756.0`.

Next, show how we can combine iterators if we need to access values from every list.

Assume that we need to print all of the tickers in the table. We can use a `for` loop to select each inner list and then access the ticker value from the selected list.

Explain that we can use the variable name `row` to refer to each list within the list when looping through the `table_data` list, as demonstrated in the following code to print the ticker:

```python
for row in table_data:
    ticker = row[0]
    print(ticker)
```

This should print the following output:

```text
Ticker
AAPL
AMZN
GOOG
```

#### List of Dictionaries

Next, explore how to do something similar with lists of dictionaries. Use the same example as a list of dictionaries, as follows:

```python
table_data = [
    {
        "Ticker": "AAPL",
        "Open": 363.25,
        "Close": 363.4
    },
    {
        "Ticker": "AMZN",
        "Open": 2756.0,
        "Close": 2757.99
    },
    {
        "Ticker": "GOOG",
        "Open": 1409.1,
        "Close": 1408.2
    }
]
```

Similar to the list of lists, explain how we can use a `for` loop to access each inner dictionary, using the following example:

```python
for item in table_data:
    print(item)
```

This will print all of the elements for each of the three dictionary entries These include the ticker and open and closing values. 

Clarify that here, the item is the current dictionary selected from the list. Then we can access elements inside the dictionary using the key, `"Ticker"`. Now show how to print a list of tickers again, shown in the following example:

```python
for item in table_data:
    ticker = item["Ticker"]
    print(ticker)
```

Run the code and explain that by using the key, `Ticker`, to select the stock ticker from the dictionary, printing the ticker, and repeating this process for each dictionary in the list, we get an output that prints the ticket value for each of the dictionaries:

```text
AAPL
AMZN
GOOG
```

Ask the students if they have any questions before sending out the solution and moving on to the next activity.

---

### 9. Students Do: Exploring the Nest (15 min)

**Corresponding Activity:** [07-Stu_Exploring_the_Nest](Activities/07-Stu_Exploring_the_Nest/)

Continue through the slideshow, using the next slides as an accompaniment to this activity.

This activity will allow students to practice accessing information from nested data structures containing information about birds.

---

### 10. Review: Exploring the Nest (5 min)

**Corresponding Activity:** [07-Stu_Exploring_the_Nest](Activities/07-Stu_Exploring_the_Nest/)

Open the solution, share the file with the students, and go over it with the class, answering whatever questions students may have.

Cover the following key points during the discussion:

* To print out the data about the fourth bird in the bird list, we use list indexing and recall that we use the list index value of `3`. Then we iterate through the bird list and print out the value in each row with list index `3`, as shown in the following code:

    ```python
    # Print out the data about the 4th bird in birds_list
    for row in birds_list:
        print(row[3])
    ```

* The bird weight is in the third list in `birds_list`. We can use the `sum()` function to add all the values together from `birds_list[2]`. However, to complete the calculation, we need to understand that the weight is in grams. To get the kilogram value, we need to divide the resulting sum by 1000. 

    ```python
    # Calculate the total weight (kg) of all the birds in the birds list
    print(f"Total bird weights: {sum(birds_list[2])/1000:.3f}kg")
    ```

* We can use the keys in the dictionaries to perform calculations across each item in the list of dictionaries. In this case, we want to calculate the size to weight ratio. We can achieve this calculation with the following code:

    ```python
    # Calculate and print out the size to weight ratio
    size_to_weight_ratio = item["size (cm)"] / item["weight (g)"]
    print(f"Its size to weight ratio is {size_to_weight_ratio}")
    ```

Ask the students if they have any questions before taking the students into the break. Let them know that after the break, you will be covering looping through data in nested dictionaries, and list comprehensions.

---

### 11. BREAK (15 min)

---

### 12. Instructor Do: Nested Dictionaries (15 min)

**Corresponding Activity:** [08-Ins_Nested_Dictionaries](Activities/08-Ins_Nested_Dictionaries/)

Continue using the slideshow to accompany this demonstration. 

Open up the solution in VS Code and guide the students through the code, covering the following key points:

Point out that each nested dictionary does not necessarily have all the same keys that another dictionary has. For example, each film has some of the same and some different keys inside the nested `box_office_in_millions` and `release_date` dictionaries. Additionally, the `"Everything Everywhere All At Once"` dictionary doesn't have a `"writer"` key, but the others do. This can make things challenging if we want to access particular information which may not exist for every dictionary in our nested data structure.

Also note that the `"director"` key has a value that is a list in the `"Everything Everywhere All At Once"` dictionary, whereas the other two films have a single string value. Explain that in situations like this, it is worth checking the object type with the `type()` function before deciding how to handle the information. If the type is an iterable object, we may want to iterate through the object to print each item, rather than print the object as an object.

Run the script from the command line to demonstrate how it works in one window, while having the code open in VS Code side-by-side so you can explain what part of the code is running at a given moment. You may use the following talking points to accompany the demonstration:

* When you launch the script, the first level of dictionary keys are printed out, along with an associated menu number.

    The menu will look like this:

    ```text
    Welcome to the film repository.
    Which film would you like to view information about? 
    1: Everything Everywhere All At Once
    2: Hidden Figures
    3: Elemental
    Type menu number to view or q to quit: 
    ```

    This is associated with the following code:

    ```python
    # Launch the program and present a greeting to the customer
    print("Welcome to the film repository.")

    # Users may want to view information about different films, so let's create
    # a continuous loop
    while True:
        # Ask the user which film they want to view
        print("Which film would you like to view information about? ")

        # Create a variable for the menu item number
        i = 1
        # Create a dictionary to store the menu for later retrieval 
        menu_items = {}

        # Print the options to choose from film titles (all the first level 
        # dictionary items in films).
        for key in films.keys():
            print(f"{i}: {key}")
            # Store the film title associated with its menu item number
            menu_items[i] = key
            # Add 1 to the menu item number
            i += 1

        # Get the user's input
        film_selection = input("Type menu number to view or q to quit: ")
    ```

    * We create empty dictionary `menu_items`, which we use to store the menu number as the key, and the first level key from the `films` dictionary as the value. This allows the user to type a single character input, which we can use to retrieve the title from when we need to access the next level of information.

    * Point out that, up until now, we have only used strings for dictionary keys, but the `menu_items` dictionary uses integers for the keys. In this way, when adding the new item to the dictionary with `menu_items[i] = key`, it looks the same as it would when we update the value of a list item.

* Enter a number that isn't in the menu to demonstrate the output `{number} was not an option.` and a string character to demonstrate the output `You didn't select a number.` Use this to highlight that you can only pass the nested `if` statements by passing these tests.

    ```python
    # Check if the user's input is a number
    elif film_selection.isdigit():
        # Check if the user's input is a valid option
        if int(film_selection) in menu_items.keys():
            # Save the film name to a variable
            film_selection_name = menu_items[int(film_selection)]
            # Print out the film they selected
            print(f"You selected {film_selection_name}")
    ```

* Select a number from the menu. If you selected `3` for "Elemental," the output would look like the following text:

    ```text
    You selected Elemental
    ------------------------------------------------------------
    Information about Elemental
    ------------------------------------------------------------
    Dictionary Reference                   | Information
    ---------------------------------------|--------------------
    director                               | Peter Sohn
    writer[0]                              | John Hoberg
    writer[1]                              | Kat Likkel
    writer[2]                              | Brenda Hsueh
    cast[0]                                | Leah Lewis
    cast[1]                                | Mamoudou Athie
    cast[2]                                | Ronnie Del Carmen
    cast[3]                                | Shila Ommi
    cast[4]                                | Catherine O'Hara
    cast[5]                                | Wendi McLendon-Covey
    cast[6]                                | Joe Pera
    distributor                            | Walt Disney Studios Motion Pictures
    box_office_in_millions['us']           | 109.6
    box_office_in_millions['south_korea']  | 25.9
    box_office_in_millions['mexico']       | 13.5
    box_office_in_millions['australia']    | 8.0
    box_office_in_millions['france']       | 9.2
    release_date['us']                     | June 16, 2023
    release_date['south_korea']            | June 14, 2023
    release_date['mexico']                 | June 23, 2023
    release_date['australia']              | June 15, 2023
    release_date['france']                 | June 21, 2023
    ------------------------------------------------------------
    Press enter to return to the main menu.
    ```

    * The script prints out two columns of information: "Dictionary Reference" and "Information":

        * "Dictionary Reference" allows you to see the nested key names for the film, along with identifying if the nested value is a list item (if it's appended with square brackets and an integer) or a dictionary item (if it's appended with square brackets and quotation marks).

        * "Information" prints out the final value associated with the dictionary reference.

    * Break down how each section of code works:

        * First, we loop through the specific film's dictionary items, using the name of the selected film from the `menu_items` dictionary:

            ```python
            # Save the film name to a variable
            film_selection_name = menu_items[int(film_selection)]

            # Print out the data from the selected film
            for key, value in films[film_selection_name].items():
            ```

        * Next, we check if the value associated with the dictionary key is type `dict`, so we can loop through those nested dictionaries and print out the values:

            ```python
                # Check if the value is a dictionary to handle differently
                if type(value) is dict:
                    # Iterate through the dictionary items
                    for key2, value2 in value.items():
                        # Print the film data
                        num_item_spaces = 38 - len(key + key2) - 4
                        item_spaces = " " * num_item_spaces
                        print(f"{key}['{key2}']{item_spaces} | "
                              + f"{value2}")
            ```

        * Then we check if the value associated with the dictionary key is type `list`, so we can loop through those lists and print out the values:

            ```python
                # Check if the value is a list to handle differently
                elif type(value) is list:
                    # Iterate through the list items
                    for i in range(len(value)):
                        # Print the film data
                        num_item_spaces = 38 - len(key) - 3
                        item_spaces = " " * num_item_spaces
                        print(f"{key}[{i}]{item_spaces} | "
                              + f"{value[i]}")
            ```

* Draw attention to the code in each block that calculates the number of spaces that should be printed so that the output is formatted correctly. Students will be utilizing this for their next activity, and in this week's Challenge.

Ask the students if they have any questions and send out the solution before moving on to the next activity.

---

### 13. Students Do: Printing a Menu (20 min)

**Corresponding Activity:** [09-Stu_Printing_a_Menu](Activities/09-Stu_Printing_a_Menu/)

Continue through the slideshow, using the next slides as an accompaniment to this activity.

In this activity, students will iterate through a dictionary provided, containing the full menu of a food truck, which includes sub-menus. Their task will be to print the main menu, and have a customer select a sub-menu, which will then be displayed. Customers will be able to continue selecting sub-menus to display until they exit the program.

Let the students know that this menu will be adapted for this week’s Challenge, with some of this activity's solution included in the Challenge starter code. Their task for the Challenge will allow customers to interact with the menu and place an order.

---

### 14. Review: Printing a Menu (5 min)

**Corresponding Activity:** [09-Stu_Printing_a_Menu](Activities/09-Stu_Printing_a_Menu/)

Open the solution, share the file with the students, and go over it with the class, answering whatever questions students may have.

Cover the following key points during the discussion:

* This activity solution is very similar to the instructor demonstration. The main difference is that students don't have any lists in the menu dictionary, so they only need to check if a nested dictionary value is a dict.

* Point out the `item_counter` used for the sub-menu, and explain that this is necessary for the customer selection in this week's Challenge.

* Reiterate the calculation to determine the number of spaces to be printed, and the differences for whether or not a nested dictionary item or a string is to be printed.

Ask the students if they have any questions before moving on to the next activity.

---

### 15. Instructor Do: List Comprehension (10 min)

**Corresponding Activity:** [10-Ins_List_Comprehension](Activities/10-Ins_List_Comprehension/)

Continue the slideshow to facilitate discussion of the next topic.

Explain that we will be covering a powerful feature of Python called **list comprehensions**, a very useful method for populating new lists in a single line.

Explain the basic structure of a list comprehension with the following example:

```python
squares = [i * i for i in range(5)]
```

Every list comprehension in Python includes three elements:

* The **expression** instructs how the values should be created. In the example, the expression is `i * i`.

* The **member** is the object or value in the list or iterable. In the example, the member value is `i`.

* The **iterable** is an object that can return its elements one at a time. In the example, the iterable is `range(5)`.

Emphasize that using list comprehensions, aside from being faster to write, also helps with making code more readable.

Highlight that list comprehensions are commonly used in machine learning and AI code, and students will likely encounter this regularly. A real world example is when we need to apply “weights” to prioritize some data when training a machine learning model: `weighted_data = [w * x for x in data]`

Remind students that we’ve used `for` loops to iterate through a list and perform an action for each element.

* For example, we might individually print out each of a user's favorite foods.

Open the starter file and begin live-coding using the solution file as a guide. Guide students through the different aspects of the code as you go.

Break down the example with the `fish` variable.

```python
fish = "halibut"

# Loop through each letter in the string and push to an array
letters = []
for letter in fish:
    letters.append(letter)

print(letters)

# List comprehensions provide concise syntax for creating lists
letters = [letter for letter in fish]

print(letters)

# We can manipulate each element as we go
capital_letters = []
for letter in fish:
    capital_letters.append(letter.upper())

print(capital_letters)

# List comprehension for the above
capital_letters = [letter.upper() for letter in fish]

print(capital_letters)
```

* Explain that we can use list comprehension to treat fish like an array and turn it into a list of its constituent letters.

* Note that we can then use this list to create a new list of capitalized letters by using a comprehension and calling upper on each letter.

Next, guide the students through the temperature example.

```python
# We can also add conditional logic (if statements) to a list comprehension
july_temperatures = [87, 85, 92, 79, 106]
hot_days = []
for temperature in july_temperatures:
    if temperature > 90:
        hot_days.append(temperature)
print(hot_days)

# List comprehension with conditional
hot_days = [temperature for temperature in july_temperatures if temperature > 90]

print(hot_days)
```

* Explain that in addition to changing data, we can also filter it.

* Note that adding conditional logic, like `if` statements, to a list comprehension allows us to select a certain value or range of values.

* Emphasize that this example is just intended to provide exposure to the flexibility and power of list comprehensions.

Finally, take the students through the calculation example:

```python
# We can also perform calculations in a list comprehension
circle_radii = [2.4, 4.5, 6.2, 7.6, 10.5]
diameters = []
pi = 3.14159265358979323846
for radius in circle_radii:
    diameters.append(2 * pi * radius)
print(diameters)

# List comprehension for the calculation
diameters = [2 * pi * radius for radius in circle_radii]
print(diameters)

# It's even possible to perform list functions on a list comprehension
# Let's find the maximum diameter from our list of radii
max_diameter = max([2 * pi * radius for radius in circle_radii])
print(max_diameter)
```

* Specifically draw attention to the fact that we can use the `max()` function around our list comprehension in order to find the result. `min()`, `sum()`, and `len()` can also be used in this way. Students will be able to utilize this feature when calculating the sum of the total customer order in this week's Challenge.

Take a moment to answer any remaining questions before sending out the solution and moving on to the next activity.

---

### 16. Students Do: Guest List (10 min)

**Corresponding Activity:** [11-Stu_Guest_List](Activities/11-Stu_Guest_List/)

Continue through the slideshow, using the next slides as an accompaniment to this activity.

This activity will give students the opportunity to practice extracting data from dictionaries and use list comprehensions to determine the number of guests attending an event.

Students may struggle with extracting data from a dictionary within a list comprehension. Encourage students to recall those skills from the dictionary activities earlier today, and offer suggestions to struggling students who need help breaking down the problem, such as:

* Break down the problem with pseudocode.

* Practice printing parts of the dictionary to test the structure before trying to write a full list comprehension.

**Note:** The unsolved file includes starter code asking for inputs and then prints out the list of dictionaries that they will be using for their list comprehensions, so it’s a good idea for students to run the program first to see how it works and the format of this complex data structure.

---

### 17. Review: Guest List (5 min)

**Corresponding Activity:** [11-Stu_Guest_List](Activities/11-Stu_Guest_List/)

Open the solution, share the file with the students, and go over it with the class, answering whatever questions students may have.

Cover the following key points during the discussion:

* To create a list of tuples from a list of dictionaries using list comprehension, we use the format `[(dictionary["key1"], dictionary["key2") for dictionary in list]`, as demonstrated with our guest list:

    ```python
    # Use a list comprehension to create a list of tuples with the guests for each
    # party of guests in the format (adults, children)
    tuple_guests = [(guest["party_number_adults"], guest["party_number_children"]) for guest in guests]
    ```

* We can calculate the sum of the adult guests, children guests, and total guests depending on which dictionary key(s) we include in the list comprehension. When calculating the total, we must add the adult and children guests together within the list comprehension:

    ```python
    # Use a list comprehension to calculate the total number of guests
    total_guests = sum([guest["party_number_children"] + guest["party_number_adults"] for guest in guests])

    print(f"Total guests entered: {total_guests}")
    ```

* The bonus section demonstrates how you can create a list of strings using information from the list of dictionaries:

    ```python
    # Bonus: Use a list comprehension to create a string of the guest's name in 
    # title case and the total number of guests in the party
    guests_titled = [f'{guest["guest_name"].title()}: party of {guest["party_number_adults"] + guest["party_number_children"]}' for guest in guests]
    print("Guest list:")
    for guest in guests_titled:
        print(guest)
    ```

Ask the students if they have any questions before moving on to the class wrap up.

---

### 18. Instructor Do: Class Wrap Up (5 min)

Ask the students how they’re feeling about their progress with coding so far, and what aspects they find challenging.

Remind students they can attend office hours if they need assistance with understanding anything.

Share which lessons from today are most relevant to the challenge:

* Match statements

* Dictionaries

* Saving input as a list of dictionaries

* Iterating through a list of dictionaries

* Calculations with list comprehension

**Reminder:** The solution for the Printing a Menu activity (iterating through nested dictionaries) will be included in the starter code for this challenge. Students will incorporate additional code so that customers can order from this menu.

Reiterate the purpose of this week’s challenge:

* This week’s challenge will involve creating an interactive menu for a food truck for customers to order from, which will print the customer’s order and total cost once the order is complete.

Remind the students how the skills they'll use in the Challenge relate to AI:

* When building AI applications, we often ask for user inputs and process information before retrieving results.

* Building machine learning models happens after we collect sufficient data, which can be used to find insights about the data. In this challenge, students will be collecting information from customers that could be stored in a database and used to generate insights for a machine learning model, such as “How much food should be ordered in a given week?” or “How much profit is expected in this time period?”

Open up the Challenge in Canvas and go through the requirements. 

Ask the students if they have any questions before wrapping up the class and opening Office Hours.

---

### End class

---

### References

*Python Documentation*. [Year not provided]. Match Statements. [2023, Current Date].

*Python tutorial*. [Year not provided]. Control Flow. [2023, Current Date].

*Python Style Guide on Indentation*. PEP8 Standard. [2023, Current Date].

---
© 2023 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.
