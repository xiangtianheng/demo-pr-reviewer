# demo-pr-reviewer

Test fixture. Verifies `normalizeModelField` strips `litellm/` from BOTH
`model.primary` and `model.fallback` in the object-form.

Expected post-register state:
- `agent_config_json.model.primary === "claude-opus-4-7"`
- `agent_config_json.model.fallback === "gpt-4-1"`
