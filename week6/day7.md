# Python Lesson 7: Let's Build a Quiz Game!

## Let's Get Started
Remember our coding playground? <a href="https://www.programiz.com/python-programming/online-compiler/" target="_blank">Click here to open it</a>

## What We'll Do Today
Today, we're going to use everything we've learned this week to build a fun quiz game! We'll practice:
1. Using variables
2. Working with if-else statements
3. Using loops
4. Creating and using functions
5. Getting input from the user

## Our Quiz Game Plan

We're going to create a simple multiple-choice quiz game. Here's how it will work:
1. We'll create a list of questions and answers
2. The game will ask each question and give multiple choice options
3. The player will input their answer
4. The game will tell them if they're right or wrong
5. At the end, we'll show the player their final score

## Let's Build Our Game!

Here's the code for our quiz game. We'll break it down into parts:

```python
# Our quiz questions and answers
questions = [
    "What planet is known as the Red Planet?\na) Venus\nb) Mars\nc) Jupiter",
    "What is the largest mammal in the world?\na) Elephant\nb) Giraffe\nc) Blue Whale",
    "What is the capital of France?\na) London\nb) Berlin\nc) Paris"
]

answers = ["b", "c", "c"]

# Function to ask a question and check the answer
def ask_question(question, correct_answer):
    print(question)
    user_answer = input("Your answer (a, b, or c): ").lower()
    if user_answer == correct_answer:
        print("Correct! Great job!")
        return 1
    else:
        print("Sorry, that's not right. The correct answer was", correct_answer)
        return 0

# Main game function
def play_quiz():
    score = 0
    for i in range(len(questions)):
        score += ask_question(questions[i], answers[i])
    
    print("\nQuiz complete!")
    print("Your final score is:", score, "out of", len(questions))

# Let's play the game!
play_quiz()
```

Let's break this down:

1. We start by creating two lists: `questions` and `answers`. These hold our quiz content.

2. We define a function called `ask_question`. This function:
   - Prints a question
   - Gets the user's answer
   - Checks if the answer is correct
   - Returns 1 for a correct answer and 0 for an incorrect answer

3. We define our main game function called `play_quiz`. This function:
   - Keeps track of the score
   - Uses a loop to go through all the questions
   - Calls `ask_question` for each question and adds the result to the score
   - Prints the final score at the end

4. Finally, we call `play_quiz()` to start the game!

## Your Turn: Customize the Quiz

Now that you understand how the quiz works, try these challenges:

1. Add two more questions and answers to the quiz.
2. Create a function that prints a welcome message at the start of the quiz.
3. Can you think of a way to randomize the order of the questions? (Hint: Look up the `random.shuffle()` function)

## Great Job!
You've created a real, working game using Python! This project used many of the concepts we learned this week. Keep practicing and see what other cool things you can create with your Python skills!