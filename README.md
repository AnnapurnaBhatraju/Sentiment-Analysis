# Sentiment Analysis and Prompting Techniques

## Sentiment Analysis

Sentiment analysis is the process of determining the emotional tone behind a body of text. It helps in understanding customer opinions, reviews, and feedback, such as the sentiment of a customer staying at a hotel. The text is classified into categories such as positive, negative, or neutral.

### Example:
Input: "I had an amazing stay at the hotel, everything was perfect!"  
Output: Positive Sentiment

Input: "The room was dirty and the service was horrible."  
Output: Negative Sentiment

## Prompting Techniques

Prompting techniques involve providing specific input to a language model to guide it in generating the desired output. Below are the main types of prompting techniques, with examples based on a customer's feedback during a hotel stay:

### 1. Zero-Shot Prompting
Zero-shot prompting is when the model is given a task without any prior examples. The model is expected to generate a response based on its understanding of the task.

**Example (Positive):**  
Prompt: "Classify the sentiment of the following hotel review: 'The staff was friendly and the room was spotless. I had a great time!'"
Output: Positive Sentiment

**Example (Negative):**  
Prompt: "Classify the sentiment of the following hotel review: 'The room was noisy and the food was cold. It was a disappointing experience.'"
Output: Negative Sentiment

### 2. One-Shot Prompting
One-shot prompting provides the model with one example to guide its response. It helps the model understand the task more clearly by showing a relevant example.

**Example (Positive):**  
Prompt: "Here's an example: 'The hotel exceeded my expectations, the staff was kind.' (Positive). Now, classify the sentiment of: 'The hotel was wonderful, I will definitely return!'"
Output: Positive Sentiment

**Example (Negative):**  
Prompt: "Here's an example: 'The hotel exceeded my expectations, the staff was kind.' (Positive). Now, classify the sentiment of: 'The air conditioning didn’t work and the bed was uncomfortable.'"
Output: Negative Sentiment

### 3. Few-Shot Prompting
Few-shot prompting provides the model with a small number of examples to help it understand the task more effectively. This allows the model to learn from the patterns in the examples and apply them to new inputs.

**Example (Positive):**  
Prompt:
Example 1: 'The hotel was perfect, the room was spacious and comfortable.' (Positive)
Example 2: 'I had a wonderful experience, the location was great.' (Positive)
Now, classify the sentiment of: 'I had a great stay, the service was top-notch.'


Output: Positive Sentiment

**Example (Negative):**  
Prompt:
Example 1: 'The hotel was perfect, the room was spacious and comfortable.' (Positive)
Example 2: 'I had a wonderful experience, the location was great.' (Positive)
Now, classify the sentiment of: 'The room was too small, and the staff was rude.'
Output: Negative Sentiment

### 4. Chain of Thought (CoT) Prompting
Chain of Thought (CoT) prompting involves asking the model to think step-by-step before providing an answer. This technique can lead to better logical reasoning and more detailed responses.

**Example (Positive):**  
Prompt: "Explain why this hotel review is positive: 'The breakfast was delicious, the staff was attentive, and the location was perfect.'"  
Response: "The phrase 'delicious breakfast' indicates a pleasant experience, 'attentive staff' shows good service, and 'perfect location' suggests satisfaction with the hotel's location."  
Output: Positive Sentiment
























