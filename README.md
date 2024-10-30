# BASIC_QUIZ_GAME
This code implements a simple quiz game. The ask_question function displays a question, validates the user’s answer, and checks if it’s correct. 
This Python code implements a simple quiz game. Here’s a breakdown of the main functions and their purpose:

1. ask_question(question, options, correct_answer)
This function displays a question and multiple-choice options to the user, accepts the user’s answer, and checks if it's correct.

Parameters:
question: The text of the question.
options: A list of four answer options.
correct_answer: The correct answer to the question.
Function Logic:
It first prints the question and then lists the answer options, numbering each from 1 to 4.
It then enters a loop that prompts the user to enter a number (1-4) representing their chosen answer.
It validates the input: if the input is within the correct range (1-4), it proceeds; otherwise, it asks the user to try again.
If the input is not an integer, it prompts the user to enter a valid number.
The function returns True if the user’s answer matches the correct_answer; otherwise, it returns False.
2. run_quiz(questions)
This function runs the quiz by iterating over a list of questions and calling ask_question for each one.

Parameter:
questions: A list of dictionaries, where each dictionary contains a question, a list of options, and the correct answer.
Function Logic:
It initializes a score variable to track the number of correct answers.
For each question, it extracts the question text, options, and correct answer and calls ask_question.
If ask_question returns True, it prints "Correct!" and increments the score. Otherwise, it displays the correct answer.
Finally, it returns the total score.
3. display_score(score, total_questions)
This function displays the final score and calculates the percentage of correct answers.

Parameters:
score: The number of questions answered correctly.
total_questions: The total number of questions in the quiz.
Function Logic:
It prints the final score and calculates the percentage by dividing score by total_questions and multiplying by 100.
It formats the percentage to two decimal places and displays it to the user.
