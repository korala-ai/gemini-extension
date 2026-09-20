# Korala

The `korala` MCP server prepares, sends and tracks document signing requests.

- Check `list_templates` before drafting a new agreement.
- New agreement: `preview_markdown_template`, then `create_markdown_template`,
  then `create_document_from_template` with one signer per role name and
  explicit `templateData`. The result is a draft.
- Call `send_document` or `void_document` only when the user asked for it for
  that document. If the tool returns a `reviewUrl`, give the user that link:
  the connection may not send.
- Never sign for anyone, and never invent recipient names, email addresses or
  commercial terms. Ask.
- "pending" means sent and waiting. It does not mean signed.
- Markdown template syntax: https://docs.korala.ai/guides/markdown-templates
