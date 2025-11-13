# Exercício 03 – Catálogo Colaborativo de Tecnologias

## Objetivo

Praticar:

- edição de **um único arquivo Markdown compartilhado**;
- adicionar itens em listas já existentes;
- tentar evitar conflitos usando boas práticas de colaboração (atualizar a branch antes de commitar, atenção ao que já foi modificado).

---

## Visão geral

Neste exercício, **todos os estudantes** vão editar o **mesmo arquivo**:

`exercicios/03-lista-tecnologias/catalogo-tecnologia.md`

Esse arquivo contém várias listas:

- IDEs
- Tecnologias / Ferramentas
- Plataformas
- Linguagens de Programação
- Empresas do ecossistema
- Outros

Seu objetivo é **adicionar uma nova linha** em uma dessas listas, **sem repetir itens que já estejam no arquivo**.

---

## Passo a passo

1. Atualize seu repositório local a partir do seu fork e da branch `main` (se necessário).

2. Crie uma branch específica para o exercício 03:

   ```bash
   git checkout -b ex03-seu-nome
   ```

3. Abra o arquivo:

   ```text
   exercicios/03-lista-tecnologias/catalogo-tecnologia.md
   ```

4. Escolha **apenas uma** das listas e adicione **um novo item**, seguindo o formato:

   ```markdown
   - Nome do item (opcional: comentário curto) - @seu-usuario-github
   ```

   Exemplos:
   - `- VS Code - @joaosilva`
   - `- Godot (engine para jogos 2D/3D) - @maria-oliveira`

   > **Importante:** verifique se o item **já não existe** na lista antes de adicionar.

5. Salve o arquivo e faça:

   ```bash
   git add exercicios/03-lista-tecnologias/catalogo-tecnologia.md
   git commit -m "adiciona item na lista de <categoria>"
   git push origin ex03-seu-nome
   ```

6. Abra um Pull Request para o repositório do professor:
   - Título sugerido: `Exercício 03 - <seu nome>`
   - Na descrição, indique qual categoria você alterou e qual item adicionou.

---

## Dicas para evitar (ou reduzir) conflitos

- Faça `git pull` (a partir do seu fork atualizado) na branch `main` antes de criar a branch do exercício.
- Tente escolher uma categoria/lista que ainda esteja com poucos itens.
- Faça sua edição, commit e push logo após puxar as atualizações (não fique muitas horas com a branch parada).
- Se houver conflito, tudo bem: peça ajuda ao professor/monitoria para resolver – isso também faz parte do aprendizado.

---

## Critérios de avaliação

- Branch criada corretamente.
- Edição feita **somente** no arquivo `catalogo-tecnologia.md`.
- Item novo adicionado sem duplicar o que já existia na lista.
- Formato do item consistente com os exemplos.
- Commit claro e Pull Request aberto corretamente.
