# vi-llm

``vi-llm`` is basically a wrapper for [llm](https://github.com/simonw/llm) that
gets all of its prompts from Vim, enabling an interactive communication with
ChatGPT using llm, by letting you input a message through the vim editor, then
sending that message to the LLM interface. subsequently displaying any logs
received from the interface right back in your text editor, repeatedly, until
the user quitting the vim editor without doing any changes. In essence, it
operates similarly to a chat interface. You type in messages (or commands)
which get sent to the LLM system, and any response from the LLM system gets
displayed back to you. This cycle continues, enabling continuous, interactive
communication with the LLM from your command line.

# Showcase

![asciicast](showcase.gif)

# Usage

The arguments that you provide to ``vi-llm`` is passed into ``llm``. This means
you can still use templates, provide a conservation id, or set system messages,
like you use in ``llm``. The usage of ``chat`` command becomes unnecessary in
``vi-llm``, since ``vi-llm`` is essentially a wrapper for ``llm`` that
implements the ``chat`` command in a more interactive way.

To read about how I use llm and vi-llm, you can check out my
[essay](https://rugu.dev/en/blog/vi-llm/).

# Installation

First, you need to install [simonw/llm](https://github.com/simonw/llm).

Then, put the `vi-llm` file in an area that's defined in your PATH environment variable.

Once this is done, you are ready to get started.
