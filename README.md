# Gotham-Criminal-input
# This code helps for Detective Gordon to get help from Batman depending on the number of criminals observed. This idea for this code wasn't initially mine but I created the code entirely by myself!
print('Hi Mr Gordon! Please enter the number of criminals that you have identified!')

criminals = int(input())
if criminals < 1:
    raise ValueError("Please enter a value greater than or equal to 1!")
if 1 <= criminals < 5:
    print('I got this! Batman, I will give you a status report once the criminals are apprehended. State whether (arrested/escaped).')
    status_report = input()
    if status_report == 'arrested':
        print('Successfully arrested')
    elif status_report == 'escaped':
        print('Batman, the criminals have gotten away!')
    else:
        print("Please type in 'arrested' or 'escaped'")
        status_report = input()
        if status_report != 'arrested' or 'escaped':
            print('Error has occurred, Please re-run program with defined input options!')
elif 5<=criminals<=10:
    print('Help me Batman! Would you like to ask Batman if Robin is available(Y/N)')
    Help = input()
    if Help == 'Y':
        print('Your request has been noted. Batman & Robin are soon arriving!')
    elif Help == 'N':
        print('No problem Mr Gordon, Batman is coming to assist you!')
    else:
        print('Please choose either (Y/N) Mr Gordon!')
else:
    print('Good luck out there')
