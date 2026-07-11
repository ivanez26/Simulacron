# Simulacron

This project utilises a chosen LLM to simulate a living fictional character. The character is described in depth by a user and an LLM starts to write a diary of each day of that character. Based on the diary entries the character changes and evolves over time. An LLM also will have choices on how to develop the character, what events to trigger. Overall, the project will have an LLM with memory and some form of agency. The name is inspired by the 13th Floor movie and the novel it's based on.

## Architecture

The easiest way to make a flipping book is to use the React library. React is an open-source JavaScript library for building user interfaces and has built-in flipping book function. Hence the frontend language is JavaScript or similar. For making it a standalone app use Electron.

The backend handles the LLM functionality. Although the first language which comes to my mind for this is Python I would pause and think more. The LLM requests are simple prompts in the end whihc are sent over Internet. The alternatives to Python could be JavaScript (to keep full app within one language) or Go (to have a lightweight and quick app). If using JavaScript take all required steps to protect the API key from exposure (put LLM API calls inside a backend environment). 