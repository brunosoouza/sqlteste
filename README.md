GITHUB_TOKEN="ghp_xxxxx"
CONTENT_URL="https://api.github.com/repos/brnorg/meu-repo/contents/database/2026-04-13/ABC-123-cria-tabela.sql?ref=abc123"

curl -L \
  -H "Authorization: Bearer ${GITHUB_TOKEN}" \
  -H "Accept: application/vnd.github.raw" \
  -H "X-GitHub-Api-Version: 2026-03-10" \
  "$CONTENT_URL"
