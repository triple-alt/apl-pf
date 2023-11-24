# APL 2.0

APL (2.0) is what I like to call a "prompt framework", but you could also just call it a format. **It's not related to the programming language under the same name.**

APL is used to create commands that are used inside of the APL framework, they are made with the [Encoder](https://github.com/triple-alt/apl-pf/blob/main/encoder-prompt) prompt and then used with the [Decoder]((https://github.com/triple-alt/apl-pf/blob/main/decoder-prompt)) prompt.

Both the Encoder and Decoder prompts have different versions **(however I make sure to try and match the version numbers but sometimes they aren't)**, the most recent versions are [here for the decoder prompt](https://github.com/triple-alt/apl-pf/blob/main/decoder-prompt) and [here for the encoder prompt](https://github.com/triple-alt/apl-pf/blob/main/encoder-prompt). Legacy (old) versions can be found [here](https://github.com/triple-alt/apl-pf/tree/main/legacy) and they are not suggested for use, but purely for learning and experimentation. Versions are major changes in either prompt, small changes are not documenated and following the project [commits](https://github.com/triple-alt/apl-pf/commits/main) is suggested as I name the change there. APL 1.0 can be found [here](https://github.com/apl-pf/APL-1.0), using this is not suggested at all.

## What is a Prompt Framework?

A prompt framework is a term I use to generalise a prompt that has multiple pieces to it or multiple use-cases, almost like a programming language. APL can be used for hundreds of different things and has two seperate prompts that make it work, however they are not necessary. APL can also be edited and fit into someone elses liking as it's available to be used by everybody and documentated, which in my opinion is an important part to a project being considered a prompt framework. 

## What is the Encoder Prompt?

The Encoder Prompt is what is used to **create** an APL command, it puts all the text into all the parameters such as important key-words into "dataset" and if there are instructional phrases in the prompt, that is put into the "instruction" parameter. It's like rearranging the prompt into a less human readable sentence but more readable by the LLM as it doesn't have to necessarily figure out what is what. **In theory, you could write your prompt into the APL format by yourself but this prompt is here to make it easier!**

## What is the Decoder Prompt?

The Decoder Prompt is what is necessary to be able to use the APL command, it's like an instruction set for the LLM to be able to percieve what the text in the command is, without it the LLM wouldn't be able to figure out what to do with it. It works by explaning in short what each parameter of a command does and what it means, but it's then for the LLM to decide what to do with each parameter. **However it's written to maintain a certain path of understanding so that it can be used almost flawlessly as if it was natural language.**

## How the Encoder and Decoder Prompts work:

<img width="888" alt="HowtoImage" src="https://github.com/triple-alt/apl-pf/assets/149606011/c2a4e544-f2bb-428a-957c-d25d843e4823">

**Updated everytime a major change is added or removed. Prompts used here may not be upto date!!**

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
