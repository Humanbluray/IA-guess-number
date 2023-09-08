# IA-guess-number
this is a short program in python wher IA try to guess a number chosen between 1 ans 99

left_born = 0
right_born = 100
question = "your number is it up?, down? or equal to "
down = "d"
up = "u"
equal = "e"
count = 0

#the game begins

answer = ""

while answer != equal:
    answer = input(question + str(int(left_born + (right_born - left_born) / 2)) + " ")

    if answer == down:
        right_born = left_born + (right_born - left_born) / 2  
    else:
        left_born = (left_born + right_born) / 2

    count += 1 
       
print("i found your nubmer in " + str(count) + " tries")
