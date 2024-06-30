# Codsoft
import random

def generate_response(user_input):
    user_input = user_input.lower().strip()

    
    if 'hello' in user_input:
        return "Hello there! How can I help you?"
    elif 'how are you' in user_input:
        return "I'm just a bot, but thanks for asking!"
    elif 'thank you' in user_input:
        return "You're welcome!"
    elif 'bye' in user_input:
        return "Goodbye! Have a nice day."
    else:
        return "Sorry, I'm not sure how to respond to that."
        
def main():
    print("Bot: Hello! How can I assist you today?")
    
    while True:
        user_input = input("You: ")
        
        if user_input.lower() == 'exit':
            print("Bot: Goodbye!")
            break
        
        bot_response = generate_response(user_input)
        print(f"Bot: {bot_response}")

if __name__ == "__main__":
    main()
