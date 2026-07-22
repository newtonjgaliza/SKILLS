---
name: devlog-manager
description: Gerencia logs de desenvolvimento (DEVLOG.md) e gera mensagens de commit detalhadas ao fim das sessões de trabalho.
---

# Devlog Manager Skill

Use esta skill sempre que o usuário solicitar a atualização do histórico de desenvolvimento (dev log) ou pedir uma mensagem de commit para as alterações atuais.

## Diretrizes

1. **Análise de Alterações:**
   - Use o comando `git status` e `git diff` para analisar quais arquivos foram criados, modificados ou deletados na sessão.
   - Identifique quais novas funcionalidades foram implementadas ou quais bugs foram corrigidos.

2. **Atualização do DEVLOG.md:**
   - Procure por um arquivo `DEVLOG.md` na raiz do projeto. Se não existir, crie-o.
   - Adicione uma entrada para a data atual (formato DD/MM/AAAA) organizada por turnos (Madrugada, Manhã, Tarde, Noite).
   - Escreva bullet points concisos e técnicos em português descrevendo cada alteração.

3. **Geração de Mensagem de Commit:**
   - Gere uma mensagem de commit semântica (seguindo o padrão Conventional Commits, ex: `feat:`, `fix:`, `refactor:`, `perf:`).
   - Liste em tópicos as principais mudanças de forma clara.
   - Forneça apenas a mensagem para o usuário copiar, sem executar o comando de commit diretamente, a menos que seja solicitado.
