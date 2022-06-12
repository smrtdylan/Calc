#calc
option = input('Hello User! Would you like to use this Calculator? (YES or NO?) ')
str(option.lower())
if option == 'yes':
    firstnum = input("What's your first number? ")

    secondnum = input("What's your second number/exponent number? ")

    equation = input('Which one-step equation would you like to do? Type MULTI, DIV, ADD, SUB, or EXP ')
    equation.upper()

    if str(equation.upper()) == 'MULTI':
        response = float(firstnum) * float(secondnum)
        print(str(response))
    elif str(equation.upper()) == 'DIV':
        response = float(firstnum) / float(secondnum)
        print(str(response))
    elif str(equation.upper()) == 'ADD':
        response = float(firstnum) + float(secondnum)
        print(str(response))
    elif str(equation.upper()) == 'SUB':
        response = float(firstnum) - float(secondnum)
        print(str(response))
    else:
        response = float(firstnum) ** float(secondnum)
        print(str(response))


elif option == 'no':
    print('Goodbye!')
