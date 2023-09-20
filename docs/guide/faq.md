# FAQ

## Why use ESLint for formatting?

Refer to [Why](/guide/why).

## How to auto-format on save?

##### VS Code

Install [VS Code ESLint extension](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)

Add the following settings to your `.vscode/settings.json`:

```jsonc
{
  "editor.formatOnSave": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
}
```

## The error messages (squiggly line) for code style is annoying

If you are using VS Code, you can override those warning with the following config in your `.vscode/settings.json`:

```jsonc
{
  "eslint.rules.customizations": [
    {
      "rule": "@stylistic/*",
      "severity": "off"
    }
  ]
}
```

It tells VS Code to not show errors in your editor but still have the ability to auto-fix them.

## How can I migrate?

Refer to [Migration Guide](/guide/migration).

## When should I migrate?

Also refer to [Migration Guide](/guide/migration#when-should-i-migrate).