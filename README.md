# apl-pf

APL (2.0) is a "prompt framework" or just a format. **It's not related to the programming language under the same name.**

It's used to create and decode commands that can be inputted into Large Language Models, such as GPT-3.5 / ChatGPT.

## Encoder Prompt

The encoder prompt is the prompt that allows users to give the LLM an input they want to encode into the APL format.

It creates a "command" that has three parameters (complexity, dataset and instruction) that give the decoder prompt an understanding of what it's meant to be.

## Decoder Prompt

The decoder prompt is what gives the LLM the understanding of what APL is, it bases it's understand of the dataset and instruction parameter.

It reads the command and replys to it as if it was given a regular and normal sentence allowing seamless use.


## Pros and Cons

There are numerous pros and cons to this idea, however it's not made to replace writing your prompts in natural languages.

Pros:
- More consistent replies, due to the way commands are formatted you are more likely to get similar replies to someone using the same command.
- Less characters, the actual prompt itself has less characters. **However read the first con.**
- Easier to customise, alongside the encoder prompts ability to create parameters that it deems useful to the command. You can add and remove things easier.
- Easier to share, projects can be "complied" into a program like format.

Cons:
- Technically, it does use MORE characters due to the need of a decoder prompt. Every update I want to condense the decoder prompt to use less and less characters.
- Lack of ease of use, you need to first give either the encoder or decoder prompt and then use the command you want to make or use. Can be a waste of time.
- It might just not be what you want, APL might just look pretty useless (too complicated to set up and use) to you which is a fair take to have but give it a try first.

I made this project to be a foundation for future projects I want to make and I can see it being useful in certain LLM applications, potentially even used as a backbone to cool and even more advanced projects!

## Use-cases

I wanted to share some of the use-cases I can see this being used for, here they are:

- Life-like video games, create a template character using the format for an LLM to create an actor for the game. Creating custom parameters like "name" or "occupation" for an easier way of creating a character in the game.
- Character.Ai esque applications, could be used to create an actor easier (pretty similar to the first example).
- Programming Language for an IDE that is used to create AI applications, due to it's nature to have an "SDK" idea behind it (custom parameters).
