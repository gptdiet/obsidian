![](https://www.askmarvin.ai/img/heroes/ai_fn_fruits_hero.png)

Meet [Marvin](https://github.com/prefecthq/marvin): a batteries-included library for building AI-powered software. Marvin's job is to integrate AI directly into your codebase by making it look and feel like any other function.




Sure, I can help you with that. Here's a zsh function that you can add to your `.zshrc` file:

```
function process-ports() {
    lsof -iTCP -sTCP:LISTEN | awk -v pattern="$1" '$0 ~ pattern {print $1, $2, $3, $8, $9}'
}
```

This function takes one argument, which is the pattern to search for in the output of `lsof`. You can call the function like this:

```
process-ports temporal
```

Let me know if you have any questions!