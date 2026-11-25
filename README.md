# Shapers MCP

Find engineers and scientists through public work. Ask for a shortlist with sources, look up a builder, or find related projects. [Check tool costs](https://shapers.si/pricing).

The remote endpoint is `https://mcp.shapers.si/mcp` and uses Streamable HTTP. Sign in when your client prompts you.

| Client | Connect |
| --- | --- |
| Claude Code | Run `claude mcp add --transport http shapers https://mcp.shapers.si/mcp`, then open `/mcp` to authenticate. |
| Codex | Run `codex mcp add shapers --url https://mcp.shapers.si/mcp`, then `codex mcp login shapers`. |
| VS Code | Run **MCP: Add Server**, select HTTP, enter the endpoint, and name it `shapers`. |
| Cursor | Copy the Shapers entry from [.mcp.json](.mcp.json) into your MCP settings. |
| Grok Build | The [.grok-plugin manifest](.grok-plugin/plugin.json) uses the same remote MCP configuration. |
| Gemini CLI | Run `gemini extensions install https://github.com/Luca-Blight/shapers-mcp`, enter your Shapers API key at the prompt, restart Gemini CLI, and run `gemini mcp list`. |

The Gemini CLI extension sends the key to the Shapers endpoint in the `X-API-Key` header. Keep it in your client’s private settings. OAuth clients discover the sign-in service from the MCP endpoint.

Try “Look up the builder torvalds and show me the public work that supports the profile.” Open a returned source to check what work it establishes.

[MCP documentation](https://shapers.si/docs/mcp) · [Source coverage](https://shapers.si/coverage) · [Shapers account](https://shapers.si/account)
