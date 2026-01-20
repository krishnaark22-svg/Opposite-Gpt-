# Opposite-Gpt-
def opposite_reply(message):
    opposites = {
        "yes": "no",
        "no": "yes",
        "true": "false",
        "false": "true",
        "up": "down",
        "down": "up",
        "happy": "sad",
        "sad": "happy",
        "on": "off",
        "off": "on"
    }

    msg = message.lower()
    return opposites.get(msg, "I will say the opposite of whatever you say 😄")

print("Opposite GPT App (type 'exit' to stop)")

while True:
    user = input("You: ")
    if user.lower() == "exit":
        print("Opposite GPT: Bye 👋")
        break
    print("Opposite GPT:", opposite_reply(user))
