# AI Tools

Remix has its own AI tool named **RemixAI** and a sub-project called **RemixAI Copilot** for code completion. 

When you load Remix, the **RemixAI Assistant** appears in the Right Side Panel.

![RemixAI Assistant Right Side Panel.](images/ai/remixai-right-panel.png)

// David put the info about the minimize button here from Release 0.71

RemixAI is also integrated into other parts of the tool.

- **Explaining a contract** icon at the button of the Main Panel when a .sol file is active.
- **Explaining compiler errors** button when an error is thrown in the Solidity Compiler
- **Right-click menu options** of the Editor
- **Code requests in the Editor** by prepending an AI code request in a file with a double slash (//).

## Choosing an LLM for code explanations

In the RemixAI Assistant, there is a choice of LLMs for use in **code explanations** and in the AI Assistant. The default LLM is MistralAI. But click the MistralAI button and a modal will popup where you can select Anthropic, OpenAI, or MistralAI.

![RemixAI LLM dropdown menu.](images/ai/llm-dropdown.png)

## Natural languages and RemixAI
The RemixAI Assitant will respond to a question in the language that it is asked.

## Computer languages and RemixAI
RemixAI will be able to answer questions about Solidity, JS/TS, Vyper and other computer languages.

## Adding context to the LLM

Clicking the `@Add context` button will bring up a modal where you can set the context of your request.

![RemixAI add context flow.](images/ai/remixai-add-context.png)

You can also set the context to the current Workspace while you type, by starting a request with `/w`.

## Code Completion

When you type a space or a new line, the RemixAI Assistant will propose some code. The proposed code is a technique called, **code completion**. The RemixAI Assistant's suggested code will take into account what has already been written in the file.

The switch to activate it is at the bottom left of the Main Panel when a file is active. Once activated, suggests code using MistralAI LLM.  For **code completion** there is no choice of LLM.

![Remix AI Copilot button.](images/ai/a-ai-switch.png)

All other RemixAI tools are always on.

When you load Remix, the RemixAI Assistant appears in the Right Side Panel.

## Editor: Right-click Menu

When you right-click a function, a popup menu appears with some options executed by the RemixAI. They include, **Explain this function**, **Explain this code**, and **Generate documentation**.

![Remix AI right click menu.](images/ai/a-ai-editor-popup-menu.png)

```{note}
For both **Explain this function** or **Explain this code**, the answer will be printed out in Remix's Terminal.
```

The "Explain this code" option in the Editor's Right-click menu can be triggered with, or without, highlighting a block of code. If some code has not been highlighted, RemixAI will take into account the code surrounding the cursor.

## Editor: Code Completion

As explained above, with the RemixAI Copilot switched on, when you put a space after a word or make a new line, the Copilot will make a suggestion.

![RemixAI completion proposal.](images/ai/a-ai-completion-proposal.png)

Hit tab to accept the suggestion.

![RemixAI accepted completion.](images/ai/a-ai-completion-accepted.png)

## Editor: Ask RemixAI with //

In the Editor, when the AI Copilot is on, you can ask it a coding question with the `//` prompt.
For example:

```text
// write a function that returns an array with 3 elements from the function's parameters
```

## Compilers: Explain Error

In the compiler error "cards" of both the Solidity Compiler and the Vyper compiler there is a button to "Ask RemixAI".

![Compiler Explain Error](images/ai/a-ai-solcomp1.png)
