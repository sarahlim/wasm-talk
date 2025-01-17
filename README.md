# All the memory safety of C combined with all the blazing speed of JavaScript

Slides and demo code for my [React Rally](https://www.reactrally.com) 2019 talk, "All The Memory Safety Of C Combined With All The Blazing Speed Of JavaScript
".

> According to [the website](https://webassembly.org/), WebAssembly is "a binary instruction format for a stack-based virtual machine, designed as a compilation target for higher-level languages like C++ and Rust." One year ago, I knew what some of those words meant. Now I understand all of them, and my goal is to share this understanding with you, fellow JavaScript programmer. We'll deep-dive into the WASM linear memory model and execution semantics, and explore how to interact with WASM modules using the JavaScript API. If calling C++ a "high-level language" makes you feel slightly ill, you are the target audience member for this talk. The title, by the way, is a reference to [A Brief, Incomplete, and Mostly Wrong History of Programming Languages](https://james-iry.blogspot.com/2009/05/brief-incomplete-and-mostly-wrong.html) by James Iry, which you should read immediately.

See also [wasm-trace](https://github.com/sarahlim/wasm-trace).

## Development

You need [pandoc](https://pandoc.org/) and [pandoc-citeproc](https://github.com/jgm/pandoc-citeproc). You can install both via Homebrew, Cabal, or Stack.

Edit slides in `index.md`. All [Pandoc markdown](https://pandoc.org/MANUAL.html#producing-slide-shows-with-pandoc), HTML, and LaTeX is valid.

This Vim command will rebuild slides on write:

```vim
autocmd BufWritePost * :silent exec "!make"
```

Then just serve the `slides` directory on localhost and navigate there in your browser.
