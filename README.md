# EXP 5: COMPARATIVE ANALYSIS OF DIFFERENT TYPES OF PROMPTING PATTERNS AND EXPLAIN WITH VARIOUS TEST SCENARIOS

## Name : LATHIKESHWARAN J
## REG.NO : 212222230072

## Aim: 
To test and compare how different pattern models respond to various prompts (broad or unstructured) versus basic prompts (clearer and more refined) across multiple scenarios.  Analyze the quality, accuracy, and depth of the generated responses 

## **AI Tools Required**

* **ChatGPT (GPT-5 model)** or equivalent large language model.
* Text editor/word processor for documentation.

## Explanation: 
Define the Two Prompt Types:

Write a basic Prompt: Clear, detailed, and structured prompts that give specific instructions or context to guide the model.
Based on that pattern type refined the prompt and submit that with AI tool.
Get the ouput and write the report.

Prepare Multiple Test Scenarios:
Select various scenarios such as:
Generating a creative story.
Answering a factual question.
Summarizing an article or concept.
Providing advice or recommendations.
Or Any other test scenario
For each scenario, create both a naïve and a basic prompt. Ensure each pair of prompts targets the same task but with different levels of structure.
Run Experiments with ChatGPT:
Input the naïve prompt for each scenario and record the generated response.
Then input the corresponding basic prompt and capture that response.
Repeat this process for all selected scenarios to gather a full set of results.
Evaluate Responses : 
	Compare how ChatGPT performs when given naïve versus basic prompts and analyze the output based on Quality,Accuracy and Depth. Also analyse does ChatGPT consistently provide better results with basic prompts? Are there scenarios where naïve prompts work equally well?
Deliverables:
A table comparing ChatGPT's responses to naïve and basic prompts across all scenarios.
Analysis of how prompt clarity impacts the quality, accuracy, and depth of ChatGPT’s outputs.
Summary of findings with insights on how to structure prompts for optimal results when using ChatGPT.

## Types of Prompting

| **Type of Prompting**                   | **Definition**                                                         | **Advantages**                                      | **Disadvantages**                            | **Example Prompt**                                                                                                         |
| --------------------------------------- | ---------------------------------------------------------------------- | --------------------------------------------------- | -------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| **1. Zero-Shot Prompting**              | Asking the model to perform a task **without any example or context.** | Quick, simple, no training data required.           | May give inaccurate or vague answers.        | “Classify this review as positive or negative: ‘I love this phone!’”                                                       |
| **2. One-Shot Prompting**               | Giving **one example** before the actual task.                         | Helps model understand the pattern slightly better. | Limited learning; might not generalize.      | “Example: ‘This food is bad’ → Negative. Now classify: ‘This restaurant is great!’”                                        |
| **3. Few-Shot Prompting**               | Giving **multiple examples** before the task.                          | Improves accuracy; model learns style and pattern.  | Prompt becomes long; may still misinterpret. | “Example 1: ‘Awesome product’ → Positive. Example 2: ‘Terrible quality’ → Negative. Now classify: ‘Very nice experience!’” |
| **4. Chain-of-Thought (CoT) Prompting** | Asking the model to **show reasoning steps** before giving the answer. | Increases accuracy for logic or math-based tasks.   | Slower; may generate unnecessary text.       | “Let’s think step-by-step. If 5 pens cost ₹50, how much for 8 pens?”                                                       |
| **5. Few-Shot + CoT Prompting**         | Combining examples and reasoning steps.                                | Very powerful for reasoning and generalization.     | Lengthy prompts; higher computation.         | Provide few examples of reasoning before task.                                                                             |
| **6. Role-based Prompting**             | Assigning a **role** to the model before the question.                 | Improves contextual relevance and tone.             | Depends on clarity of role.                  | “You are a physics professor. Explain quantum entanglement in simple words.”                                               |
| **7. Instruction-based Prompting**      | Giving explicit **instructions or format expectations.**               | More control over structure of output.              | May restrict creativity.                     | “Summarize this paragraph in 3 bullet points with a conclusion.”                                                           |
| **8. ReAct Prompting (Reason + Act)**   | Model reasons first, then performs the action step-by-step.            | Improves factual accuracy and decision-making.      | More complex setup.                          | “Reason about the question before answering: What are the advantages of solar energy?”                                     |
| **9. Multimodal Prompting**             | Using **text + image + audio or video** as input.                      | Suitable for complex real-world problems.           | Needs multimodal AI (like GPT-4V).           | “Analyze this image and describe the mood of the person.”                                                                  |
| **10. Retrieval-Augmented Prompting**   | Combining AI prompt with **external knowledge sources** or documents.  | Gives factually grounded answers.                   | Needs external data access or APIs.          | “Using this document, summarize the company’s financial report.”                                                           |



## Comparative Analysis Table

| **Criterion**       | **Zero-Shot**      | **One-Shot**         | **Few-Shot**    | **CoT**          | **Role-Based**     | **Instruction-Based** |
| ------------------- | ------------------ | -------------------- | --------------- | ---------------- | ------------------ | --------------------- |
| **Accuracy**        | Low                | Medium               | High            | Very High        | High               | High                  |
| **Complexity**      | Very Low           | Low                  | Medium          | High             | Medium             | Medium                |
| **Response Length** | Short              | Short                | Medium          | Long             | Medium             | Controlled            |
| **Best Use Case**   | Simple tasks       | Basic classification | NLP tasks       | Math, logic      | Explanations       | Structured outputs    |
| **Training Need**   | None               | Minimal              | Some            | Logical thinking | Context setting    | Instruction clarity   |
| **Example Domain**  | Sentiment analysis | Categorization       | Text generation | Problem solving  | Teaching, tutoring | Summarization         |

## Test Scenarios

Let’s take a sample problem and apply different prompting patterns to see the variation in outputs.

### Scenario: Text Classification

Task: Classify the sentiment of the review:

“The movie was fantastic and full of emotion!”

🔸 Zero-Shot Prompt

Classify the sentiment: “The movie was fantastic and full of emotion!”
Output: Positive ✅

🔸 One-Shot Prompt

Example: “The movie was boring” → Negative
Classify: “The movie was fantastic and full of emotion!”
Output: Positive ✅ (Slightly more accurate tone)

🔸 Few-Shot Prompt

Example 1: “I loved this film” → Positive
Example 2: “It was terrible and dull” → Negative
Classify: “The movie was fantastic and full of emotion!”
Output: Strongly Positive ✅ (Better contextual understanding)

🔸 Chain-of-Thought Prompt

Let’s think step-by-step. The review uses the words “fantastic” and “full of emotion,” which are positive expressions.
Therefore, sentiment: Positive.
Output: Positive ✅ (With reasoning)

🔸 Role-based Prompt

You are a film critic. Analyze the sentiment: “The movie was fantastic and full of emotion!”
Output: “As a film critic, I’d say it conveys strong positive emotions.” ✅

🔸 Instruction-based Prompt

Give the sentiment and a one-line explanation.
Output: Sentiment: Positive. Reason: The words indicate excitement and praise. ✅

### Scenario 2: Reasoning Task

Question: “If 3 apples cost ₹15, how much do 7 apples cost?”

## Prompt Type	Output

| **Prompt Type**       | **Output**                                                 |
| --------------------- | ---------------------------------------------------------- |
| **Zero-Shot**         | ₹35 ❌ (May guess wrong)                                    |
| **Chain-of-Thought**  | “Each apple = ₹5. 7 × ₹5 = ₹35.” ✅                         |
| **Few-Shot + CoT**    | “Given pattern: 2 apples = ₹10 → 1 = ₹5 → 7 = ₹35.” ✅      |
| **Instruction-based** | “Answer in step-by-step format.” ✅ Accurate and formatted. |


## Conclusion

| **Prompting Pattern** | **When to Use**                     | **Performance**            |
| --------------------- | ----------------------------------- | -------------------------- |
| **Zero-Shot**         | For quick, simple tasks             | ⚡ Fast but less accurate   |
| **Few-Shot**          | When you can provide examples       | 🎯 Balanced and reliable   |
| **CoT**               | For reasoning or step-based tasks   | 🧩 Very accurate           |
| **Role-Based**        | For tone and perspective control    | 👩‍🏫 Context-rich answers |
| **Instruction-Based** | For formatted or structured outputs | 🗂️ Clear and organized    |
| **ReAct / Retrieval** | For factual and complex tasks       | 🧠 Expert-level responses  |

## Result

The experiment on prompt comparison was executed successfully.

