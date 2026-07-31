# Calling-LLM-in-Python
Gen AI Gemini

from google import genai

client = genai.Client(api_key="API_KEY")

interaction = client.interactions.create(
    model="gemini-3.6-flash",
    input=" please write me a def python function for visualise my LM plot"
)
print(interaction.output_text)
