# Quiz
# quiz_app.py

# List of questions and answers
print("WELCOME TO THE MINI QUIZ🤔 ")
quiz = [
    {
        "question": "What is the capital of India?🤔",
        "options": ["A. Berlin", "B. New Delhi", "C. Paris", "D. Rome"],
        "answer": "B"
    },
    {
        "question": "Which planet is known as the Red planet ?🤔",
        "options": ["A. Venus", "B. Saturn", "C. Mars", "D. Jupiter"],
        "answer": "C"
    },
    {
        "question": "What is 5 + 7?🤔",
        "options": ["A. 10", "B. 12", "C. 14", "D. 15"],
        "answer": "B"
    },
    {
        "question": "What is the largest mammal in the world?🤔",
        "options": ["A. Elephant", "B. Whale Shark", "C. Giraffe", "D. Blue Whale"],
        "answer": "D"
    },
    {
        "question": "What is 9 x 5?🤔",
        "options": ["A. 54", "B. 45", "C. 64", "D. 56"],
        "answer": "B"
    },
    {
        "question": "Which device is used to connect to the internet?🤔",
        "options": ["A. Mouse", "B. Printer", "C. Modem", "D. Scanner"],
        "answer": "C"
    },
    {
        "question": "Who invented the light bulb?🤔",
        "options": ["A. Newton", "B. Edison", "C. Einstein", "D. Tesla"],
        "answer": "B"
    },
    {
        "question": "Which gas do plants absorb from the atmosphere?🤔",
        "options": ["A. Oxygen", "B. Hydrogen", "C. Carbon Dioxide", "D. Nitrogen"],
        "answer": "C"
    },
    {
        "question": "Which number is a prime number?🤔",
        "options": ["A. 4", "B. 9", "C. 11", "D. 15"],
        "answer": "C"
    },
    {
        "question": "What does CPU stand for?🤔",
        "options": ["A. Central Power Unit", "B. Central Processing Unit", "C. Computer Primary Unit", "D. Core Programming Unit"],
        "answer": "B"
    }
]


# Score tracking
score = 0

# Quiz loop
for i, q in enumerate(quiz, 1):
    print(f"\nQuestion {i}: {q['question']}")
    for option in q['options']:
        print(option)

    user_answer = input("Enter your answer (A/B/C/D): ").strip().upper()

    if user_answer == q['answer']:
        print("✅ Hurry...Correct!🤩")
        score += 1
    else:
        print(f"❌ Oops..Wrong!😔 The correct answer is {q['answer']}.")

# Final score
print(f"\nYour Final Score: {score}/{len(quiz)}")
