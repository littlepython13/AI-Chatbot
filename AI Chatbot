import google.generativeai as genai

API_KEY = "YOUR API KEY"

genai.configure(api_key=API_KEY)

model = genai.GenerativeModel('gemini-pro')
chat_session = model.start_chat(history=[])

while True:
    user_input = input("You: ")

    if not user_input.strip():
        break

    response = chat_session.send_message(user_input)
    print(f"\nBot: {response.text}\n")
