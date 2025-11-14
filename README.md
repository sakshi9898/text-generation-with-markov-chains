# Markov Chain Text Generator

## Overview
This program generates random text using a Markov Chain model. It analyzes a given text, builds a dictionary of word transitions, and generates new text that mimics the style of the input.

## Features
- Splits input text into individual words.
- Builds a Markov Chain dictionary automatically.
- Generates text of fixed or custom length.
- Modular code structure with separate functions for each task.

## How It Works
1. The text is loaded from the load_text() function.
2. preprocess() converts the text into a list of words.
3. build_chain() creates a mapping of each word to possible next words.
4. generate() randomly produces new text using the chain.

## How to Run
Run the script using:

python markov_generator.py

## Customization
You can modify the base text inside the load_text() function.

Example:
def load_text():
    return "Your custom text goes here."

You can change the output length by modifying:

generate(chain, 50)

## Output
The program prints generated text based on the Markov Chain model.
