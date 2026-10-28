# colab-demo

A small demo project for working with GitHub and Google Colab.


## Creative ideas notebook

[`creative_ideas.ipynb`](creative_ideas.ipynb) is a beginner-friendly Google Colab notebook that asks for an everyday object and uses the OpenAI Responses API with `gpt-6-luna` to suggest **three numbered, unusual, practical ideas**.

1. Open [Google Colab](https://colab.research.google.com/), choose **File → Upload notebook**, and upload `creative_ideas.ipynb`.
2. Connect to a Python 3 runtime (CPU is enough) and run the cells from top to bottom. The first code cell installs or updates the OpenAI SDK.
3. Enter your OpenAI API key once at the hidden `getpass` prompt, then enter an everyday object. You need model access and available API credit; requests may incur charges.
4. Read the three ideas numbered 1, 2, and 3. Enter another object when prompted; the program keeps running without restarting the notebook or rerunning the cell.
5. Type `quit` to stop. This also accepts capitalization such as `QUIT` and surrounding spaces. Blank input asks you to try again without making an API request.

If a request fails, check your key, model access, API credit, and connection, then try another object or type `quit`. To use a different API key, stop the program and rerun the idea cell. Each object sent to the API is a separate request.

Enter your key only at the runtime prompt. Never paste it into code, notebook text, outputs, or Git. The notebook does not print or save the key. Disconnect and delete the Colab runtime when finished, and clear cell outputs before sharing or saving to Git.

API reference: [official OpenAI text generation guide](https://developers.openai.com/api/docs/guides/text?lang=python).
