# SCM_project
# difining function to give options
def give_options(x, y, z):
    print("a):", x)
    print("b):", y)
    print("c):", z)


# Here the user is asked to enter the name first
player_name = input("Please, Enter your name : ")
print("")

# welcoming and giving insstructions
print("Hello!", player_name)
print("A very warm welcome to BRAIN TEST")
print("It's basically a quiz game")
print("Here are some instructions you need to keep in your mind while playing this game:-")
print("""
1. The quiz consists of 10 questions that are carefully designed to help you self-assess your knowledge.
2. Each question in the quiz is of multiple-choice format and carring 10 marks each.
3. keep in mind, you have to write answer not option.
4. Answers are not case sensitive ie. you can write in capital letter as well in small letter.
5. After writing the answer, click the enter bottom for next question.
6. The total score of the quiz will be shown after completing the quiz.""")

# asking user to start the game
print("")
ans = input("Are you ready to play (yes/no): ")
print("")

# Initializing the score.
score = 0
negative_score = 0

# declaring the total number of question
total_questions = 10

# correct_ans list stores correct answers of each question.
correct_ans = [".py", "0", "paypal", "draco malfoy", "venus", "11", "87.58m", "ronan the accuser", "plasma", "junkook"]

# starting loop for each question
if ans.lower() == "yes":
    print("")

    # print question.
    print("Question no.1: Which of the following is the correct extension of the Python file?")
    give_options(".Python", ".pl", ".py")

    # taking answer as input.
    ans = input("Write your answer=  ")

    # condition checking.
    if ans.lower() == correct_ans[0]:
        score = score + 1
        print("Correct")
    else:
        negative_score = negative_score + 1
        print("Incorrect")
    print("")
    print("Question no.2: How many blue stripes are there on the U.S. flag? ")
    give_options('6', '7', '0')
    ans = input("Write your answer=  ")
    if ans.lower() == correct_ans[1]:
        score = score + 1
        print("Correct")
    else:
        negative_score = negative_score + 1
        print("Incorrect")
    print("")
    print(
        "Question no.3: In 1999,Elon Musk founded X.com, which merged with Confinity 2 years later to become which online business? ")
    give_options("twitter", "google", "paypal")
    ans = input("Write your answer=  ")
    if ans.lower() == correct_ans[2]:
        score = score + 1
        print("Correct")
    else:
        negative_score = negative_score + 1
        print("Incorrect")
    print("")
    print("Question no.4: Which one of these characters is not friends with Harry Potter?")
    give_options("Ron Weasley", "Neville Longbottom", "Draco Malfoy")
    ans = input("Write your answer=  ")
    if ans.lower() == correct_ans[3]:
        score = score + 1
        print("Correct")
    else:
        negative_score = negative_score + 1
        print("Incorrect")
    print("")
    print("Question no.5: Which planet is the hottest planet in our solar system?")
    give_options("venus", "saturn", "mercury")
    ans = input("Write your answer=  ")
    if ans.lower() == correct_ans[4]:
        score = score + 1
        print("Correct")
    else:
        negative_score = negative_score + 1
        print("Incorrect")
    print("")
    print("Question no.6: What is the t-shirt's number of football player Sunil chhetri?")
    give_options("11", "13", "12")
    ans = input("Write your answer=  ")
    if ans.lower() == correct_ans[5]:
        score = score + 1
        print("Correct")
    else:
        negative_score = negative_score + 1
        print("Incorrect")
    print("")
    print("Question no.7: What was the record for javelin throw in Neeraj Chopra’s Olympics gold?")
    give_options("89.9m", "85.6m", "87.58m")
    ans = input("Write your answer=  ")
    if ans.lower() == correct_ans[6]:
        score = score + 1
        print("Correct")
    else:
        negative_score = negative_score + 1
        print("Incorrect")
    print("")
    print('''Question no.8: Who is the villain in the movie "Guardians of the Galaxy: Vol 1"?''')
    give_options("Ronan The Accuser", "Obidiah Stane", "Yondu Udonta")
    ans = input("Write your answer=  ")
    if ans.lower() == correct_ans[7]:
        score = score + 1
        print("Correct")
    else:
        negative_score = negative_score + 1
        print("Incorrect")
    print("")
    print("Question no.9: Which one of the following is the 4th state of matter?")
    give_options("gas", "plasma", "Supercritical fluid")
    ans = input("Write your answer=  ")
    if ans.lower() == correct_ans[8]:
        score = score + 1
        print("Correct")
    else:
        negative_score = negative_score + 1
        print("Incorrect")
    print("")
    print('''Question no.10: Which member of BTS is called "the golden maknae"?''')
    give_options("junkook", "RM", "V")
    ans = input("Write your answer=  ")
    if ans.lower() == correct_ans[9]:
        score = score + 1
        print("Correct")
    else:
        negative_score = negative_score + 1
        print("Incorrect")
        print("")
else:
    print("dear", player_name, "you choosed not to play")
    print("")

# multiply the score with 10
i = score * 10
# multiply the negative score with 5
j = negative_score * 5
l = i - j

# pass the if else conditions to print the result
if l <= 30:
    print("Oh,", player_name, "your score is ", l, "/ 100 better luck next time and keep trying.")
elif 30 < l < 80:
    print("Nice!", player_name, " you scored ", l, "/ 100 you are quiet smart.")
elif l == 80:
    print("great", player_name, "you scored", l, "/100 ")
else:
    print("Congratulations!", player_name, " it's a perfect score ", l, "/ 100 you are very Intelligent.")
