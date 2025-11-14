# Exercício 01 – Perfil em Markdown

## Objetivo

Praticar o fluxo básico do Git: fork → clone → branch → commit → push → pull request.

## Tarefa

Crie um arquivo Markdown com um pequeno perfil seu.

### Passo a passo

1. Crie uma branch:

   ```bash
   git checkout -b ex01-seu-nome
   ```

2. Crie um arquivo dentro desta pasta:

   ```bash
   perfil-<seu-usuario-github>.md
   ```

3. Use o template:

   ```markdown
   # Seu nome completo

   ## Curso e período

   Ciência da Computação - 1º período

   ## Áreas de interesse em tecnologia
   
   - Exemplo 1
   - Exemplo 2
   - Exemplo 3

   ## Uma curiosidade sobre você
   
   Escreva 2–3 frases com algo que você gostaria de compartilhar.
   
   ```

4. Faça commit e push:

   ```bash
   git add exercicios/01-perfil-markdown/perfil-<seu-usuario>.md
   git commit -m "adiciona perfil de <seu-usuario>"
   git push origin ex01-seu-nome
   ```

5. Abra um Pull Request no GitHub.

## Critérios de avaliação

- Branch criada corretamente
- Nome correto do arquivo
- Template preenchido
- Commit claro
- PR enviado corretamente
