FROM node:20-bookworm-slim

# Claude Code CLI global installieren
RUN npm install -g @anthropic-ai/claude-code

# Fuer die MCP-Server (npx-basiert) reicht das mitgelieferte npm/npx aus dem
# Node-Image bereits aus - kein zusaetzliches Python/uv noetig, solange wir
# bei den npx-Varianten von influxdb3-mcp-server und mcp-grafana bleiben.

WORKDIR /workspace

# Haelt den Container am Laufen, damit man sich per
# "docker exec -it claude-code claude" hineinverbinden kann
# (analog zum bestehenden ttyd-Workflow).
CMD ["sleep", "infinity"]
