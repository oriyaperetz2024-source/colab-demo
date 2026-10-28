# colab-demo

A small demo project for working with GitHub and Google Colab.


## Creative ideas notebook

[`creative_ideas.ipynb`](creative_ideas.ipynb) is a beginner-friendly Google Colab notebook that asks for an everyday object and uses the OpenAI Responses API with `gpt-6-luna` to suggest **one unusual, practical use**.

1. Open [Google Colab](https://colab.research.google.com/), choose **File → Upload notebook**, and upload `creative_ideas.ipynb`.
2. Connect to a Python 3 runtime (CPU is enough) and run the cells from top to bottom. The first code cell installs or updates the OpenAI SDK.
3. Enter an object, then enter your OpenAI API key at the hidden `getpass` prompt. You need model access and available API credit; requests may incur charges.
4. Read the idea. Rerun the idea cell to try another object. If a request fails, check your key, model access, API credit, and connection.

Enter your key only at the runtime prompt. Never paste it into code, notebook text, outputs, or Git. The notebook does not print or save the key. Disconnect and delete the Colab runtime when finished, and clear cell outputs before sharing or saving to Git.

API reference: [official OpenAI text generation guide](https://developers.openai.com/api/docs/guides/text?lang=python).
