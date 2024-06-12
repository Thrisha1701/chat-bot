responses={"hi":"hello","name":"Sai Thrisha","section":"tesla","roll no":"4B1","branch":"ece","default":"sorry i didn't catch you"}
def respond(message):
    if message in responses:
        return responses[message]
    else:
        return responses["default"]
print("Bot:Hello iam chatbot")
print("Bot:You can start chat with me if u want to end chat type bye")
while True:
    user_input=input("you: ")
    if user_input.lower()=="bye":
        print("Bot:Bye have a great day")
        break
    else:
        response=respond(user_input)
        print("Bot: ",response)