# Korala for Gemini CLI

Publish this directory as the root of a public GitHub repository (for example
`korala-ai/gemini-extension`) with the `gemini-cli-extension` topic. The
Gemini CLI extension gallery crawls tagged repositories daily.

```
gemini extensions install https://github.com/korala-ai/gemini-extension
```

Gemini CLI discovers Korala's OAuth server by itself and opens a browser to
sign in on first use. Without the extension:

```
gemini mcp add --transport http korala https://api.korala.ai/mcp
```
