🚀 Welcome to the Prompt Engineering Experimenter! 🚀

Enter the text you want to process (e.g., a movie review):
> Movie review

🔬 Running Experiments...

--- Zero-Shot Prompting ---

✨ Sending prompt to Gemini...
------------------------------------
📜 Prompt: "Classify the sentiment of this movie review: 'Movie review'"
------------------------------------
💬 Gemini's Zero-Shot Response:
Without any actual content in the movie review, it's impossible to classify the sentiment. "Movie review" is just a label. I need the actual text of the review to determine if it's positive, negative, or neutral.


--- Zero-Shot Prompting ---

✨ Sending prompt to Gemini...
------------------------------------
📜 Prompt: "Classify the sentiment of this movie review: 'Prompt Enginear'"
------------------------------------
💬 Gemini's Zero-Shot Response:
Without any actual content in the Prompt Enginear, it's impossible to classify the sentiment. "Prompt Enginear" is just a label. I need the actual text of the review to determine if it's positive, negative, or neutral.

--- Few-Shot Prompting ---

✨ Sending prompt to Gemini...
------------------------------------
📜 Prompt: "Classify the sentiment of this movie review: 'The movie was an absolute masterpiece, thrilling from start to finish!'

Review: 'The movie was an absolute masterpiece, thrilling from start to finish!'
Sentiment: Positive

Review: 'I really wanted to like this film, but it was slow and predictable.'
Sentiment: Negative

Review: 'It was an okay movie, not great but not terrible either.'
Sentiment: Neutral

Review: 'Movie review'
Sentiment:"
------------------------------------

💬 Gemini's Few-Shot Response:
Sentiment: **Neutral**

--- Few-Shot Prompting with a twist ---

✨ Sending prompt to Gemini...
------------------------------------
📜 Prompt: "Classify the sentiment of this movie review: 'The movie was an absolute masterpiece, thrilling from start to finish!'

Review: 'The movie was an absolute masterpiece, thrilling from start to finish!'
Sentiment: Positive

Review: 'I really wanted to like this film, but it was slow and predictable.'
Sentiment: Negative

Review: 'It was an okay movie, not great but not terrible either.'
Sentiment: Neutral

Review: 'Oh the movie was great, if you are looking for a lullaby'
Sentiment:"
------------------------------------

💬 Gemini's Few-Shot Response:
Sentiment: **Negative**

--- Chain-of-Thought Prompting ---

✨ Sending prompt to Gemini...
------------------------------------
📜 Prompt: "Classify the sentiment of this movie review and explain your reasoning: 'Movie review'. Let's think step-by-step."
------------------------------------

💬 Gemini's Chain-of-Thought Response:
Okay, let's analyze the sentiment of the text: "Movie review".

**Step 1: Identify the key phrase.**

The key phrase is "Movie review".

**Step 2: Determine the inherent sentiment of the phrase.**

The phrase "Movie review" itself is **neutral**. It simply indicates that a review of a movie is present or being discussed. It doesn't express any positive or negative emotion about the movie itself.

**Step 3: Consider potential context.**

Without any additional context, we can only assume that the phrase is a label or a heading. Labels and headings are typically neutral.

**Conclusion:**

The sentiment of the phrase "Movie review" is **neutral**. It doesn't convey any positive or negative opinion.

🎉 Experiments Complete! 🎉

🤔 Compare and Contrast:
-------------------------
Consider the following when comparing the outputs:
1.  **Accuracy/Relevance:** How well did each technique perform the task (e.g., sentiment classification)?
2.  **Completeness of Response:** Did CoT provide a more reasoned or detailed output?
3.  **Conciseness:** Were some responses more to-the-point than others?
4.  **Ease of Implementation:** How complex was it to set up each prompt type?
5.  **Generalizability:** How might these techniques perform on different tasks or with different inputs?

For example:
-   **Zero-shot** is the simplest but might be less accurate for complex tasks if the model hasn't been explicitly trained for them.
-   **Few-shot** provides context and examples, often improving accuracy, especially for specific formats or nuanced tasks. However, selecting good examples is key.
-   **Chain-of-Thought** encourages the model to break down the problem, which can lead to better reasoning and more accurate results for complex problems, though the output might be more verbose.
