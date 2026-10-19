# claude-bridge plugin

Gives an org Claude instance two things:

1. A skill, `claude-bridge-log`, that defines the shared handoff log between `claude-ai` and `org-claude`.
2. A ThinkSL8 MCP server entry (`https://thinksl8.com/mcp`) in `.mcp.json`.

## Install

1. Zip the contents of this folder so `.claude-plugin/plugin.json` sits at the zip root (the prepared `claude-bridge.zip` already does).
2. In the org instance, open the plugin or skill settings and upload the zip. The exact menu name depends on how the org deployment is set up.
3. Enable the plugin, then confirm the ThinkSL8 tools appear in a new session.

## Check before relying on it

- If your admin blocks custom connectors, the plugin's `.mcp.json` may be ignored or rejected. Ask the admin before trying to get around it.
- The ThinkSL8 connector exposes canvas reading and search. Its write tools only handle voice notes (audio plus transcript), so the log itself is best kept as `BRIDGE-LOG.md` in a shared folder, with ThinkSL8 used for reading.
- This package has not been test-installed in your org.
