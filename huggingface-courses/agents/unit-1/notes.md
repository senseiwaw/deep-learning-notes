# Unit 1 

## What is an agent ?
definition : An AI agent is a system that leverages an AI model to interact with its environment in order to achieve a user-defined objective. It *combines* resonning, planning and the execution of actions (usually using external tools) to fullfil tasks.

### What is an agent composed of ?
* Brain (AI Model, reasoning, choosing best options)
* Body (capabilities and tools)


### What AI Model are used for agents ?
* **Large Language Models** (LLM) which inputs&outputs **Text** such as : 
* * *ChatGPT* from *OpenAI*
  * *Gemini* from *Google*
  * *Llama* from *Meta*
* but other types of models are available such as **Vision Language Models** (VLM) that take **Images/Videos** as inputs.

### How agents execute actions ?
* the answer is : they use (external) **Tools** to execute **Actions**


## What are LLMs ?
definition : An AI model that is very good at both **understanding and generating human language**. This model was trained on a vast amount of text, allowing it to learn patterns, *structure* and meaning *in language*. It generally contains many milions of parameters. They are built on a **Transformer** architecture (a neural network architecture from deep learning based on the **Attention** algorithm)

### How they can get good at **understanding and generating human language** ?
answer : transformers
### What is a Transformer ?
there are 3 types of Transformers : 
* An Encoder : takes text as input and outputs a dense representation (**embedding**) of this text
* A Decoder : takes a sequence of tokens and outputs the next most probable token, **one at a time**
* Seq2Seq (sequence to sequence / Encoder-Decoder) : combines a encoder to transform the text into a *context-representation* then uses a decoder to output the next token.

the underlying principle of an LLM is to predict the next token given a sequence of previous tokens.


