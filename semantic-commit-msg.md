## Semantic Commit Message

I liked the [Angular] and this one commit guidelines and [this one] I found in GitHub Gist 🚀

### TL;DR;

Format: `<type>: <subject>`

|           Type | Description                                                          |
| -------------: | -------------------------------------------------------------------- |
|     **`feat`** | new feature for the user, not a new feature for build script         |
|    **`chore`** | updating grunt tasks etc; no production code change                  |
|     **`docs`** | changes to the documentation                                         |
|      **`fix`** | bug fix for the user, not a fix to a build script                    |
| **`refactor`** | refactoring production code, eg. renaming a variable                 |
|    **`style`** | formatting, missing semi colons, etc; no production code change      |
|     **`test`** | adding missing tests, refactoring tests; no production code change   |
|   **`revert`** | "This reverts COMMIT_HASH" or "This reverts the pull request PR_NUM" |

#### Hints 💡

- **Commit message < 100 characters!**
  *Why? This allows the message to be easier to read on GitHub as well as in various git tools.*

[Angular]: https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines
[this one]: https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716#file-semantic-commit-messages-md
