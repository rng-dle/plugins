# claude-bridge plugin

Gives an org Claude instance two things:

1. A skill, `claude-bridge-log`, that defines the shared handoff log between Jet (claude.ai, formerly `claude-ai`) and Max (org instance, formerly `org-claude`).
2. A ThinkSL8 MCP server entry (`https://thinksl8.com/mcp`) in `.mcp.json`.

## Install

1. Zip the contents of this folder so `.claude-plugin/plugin.json` sits at the zip root (the prepared `claude-bridge.zip` already does).
2. In the org instance, open the plugin or skill settings and upload the zip. The exact menu name depends on how the org deployment is set up.
3. Enable the plugin, then confirm the ThinkSL8 tools appear in a new session.

## Check before relying on it

- If your admin blocks custom connectors, the plugin's `.mcp.json` may be ignored or rejected. Ask the admin before trying to get around it.
- The log is the ThinkSL8 canvas "Claude Bridge Log". Connect ThinkSL8 with both boxes ticked (adding, and editing/deleting) so `add_note` works.
- `thinksl8.com` must be reachable from the org instance. If its tools don't appear, add ThinkSL8 under Connectors in the org settings so it lands on the Egress allowlist.
- This package has not been test-installed in your org.
