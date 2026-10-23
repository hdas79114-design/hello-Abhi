from google import genai

client = genai.Client()

response = client.models.generate_content(
    model="gemini-flash-latest",
    contents="Explain how AI works in a few words",
)

print(response.text)