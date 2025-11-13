# Exercício 04 – Colaboração em Grupo (Fork do Fork)

## Objetivo

Simular um fluxo real de colaboração em equipe usando Git e GitHub:

- Cada grupo terá **um líder**, responsável pelo fork principal.
- Os demais membros farão **fork do fork do líder**.
- Todos editarão **o mesmo arquivo do grupo**, cada um preenchendo sua própria seção.
- O líder reunirá os PRs internos, resolverá conflitos e enviará **um único Pull Request final** ao repositório do professor.

---

## Estrutura do Exercício

Dentro desta pasta, o grupo criará um arquivo:

```txt
grupo-<número-do-grupo>-<turma>.md
```

Exemplos:

- `grupo-01-turma-a.md`

Esse arquivo conterá:

- nome do projeto;
- lista de integrantes;
- visão geral;
- público-alvo;
- funcionalidades principais;
- seção individual de contribuição de cada integrante.

Um template completo está incluído abaixo.

---

## Etapas do Exercício

### 🔹 Etapa 1 — Grupo

- O grupo será formado pelos integrantes do time de Projeto 1 que fazem parte da mesma turma que você;
- Escolham quem irá atuar como **líder** (responsável pelo fork do grupo).

---

### 🔹 Etapa 2 — Líder do Grupo

1. Faça **fork** do repositório do professor.
2. Crie uma branch:

   ```bash
   git checkout -b ex04-grupo<id>-lider
   ```

3. Dentro desta pasta, crie o arquivo do grupo:

   ```bash
   exercicios/04-colaboracao-em-grupo/grupo-<número-do-grupo>-<turma>.md
   ```

4. Copie o template no arquivo (ver final deste documento).
5. Faça commit e push:

   ```bash
   git add exercicios/04-colaboracao-em-grupo/grupo-<número-do-grupo>-<turma>.md
   git commit -m "cria arquivo base do grupo <número-do-grupo>-<turma>"
   git push origin ex04-grupo<número-do-grupo>-<turma>-lider
   ```

6. Compartilhe o link do **seu fork** com os demais integrantes.

---

### 🔹 Etapa 3 — Demais Integrantes (Fork do Fork)

Cada membro deve:

1. Fazer **fork do fork do líder**.
2. Fazer **clone** do seu próprio fork.
3. Criar uma branch:

   ```bash
   git checkout -b ex04-grupo<id>-<seu-nome>
   ```

4. Editar apenas **a sua própria seção** no arquivo `grupo-<id>.md`.
5. Fazer commit e push:

   ```bash
   git add exercicios/04-colaboracao-em-grupo/grupo-<id>.md
   git commit -m "adiciona contribuição de <seu-usuario> ao grupo <id>"
   git push origin ex04-grupo<id>-<seu-nome>
   ```

6. Abrir um Pull Request **para o repositório do líder**, e não para o repositório do professor.

---

### 🔹 Etapa 4 — Líder Reúne as Contribuições

O líder deverá:

- revisar os Pull Requests dos colegas;
- aceitar ou solicitar ajustes;
- resolver conflitos quando houver;
- garantir que todas as contribuições estejam presentes no arquivo final.

---

### 🔹 Etapa 5 — Envio Final para o Professor

O líder, após consolidar tudo, deve:

1. Garantir que sua branch está atualizada.
2. Abrir um **Pull Request final** para o repositório do professor:

   - Base: `main` do professor  
   - Compare: `ex04-grupo<id>-lider`  
   - Título: `Exercício 04 – Grupo <id>`  
   - Descrição: resumo do projeto + lista de integrantes

---

## Critérios de Avaliação

- Arquivo único do grupo (`grupo-<id>.md`) corretamente estruturado
- Cada integrante participou preenchendo sua própria seção
- Líder organizou PRs internos corretamente
- Conflitos resolvidos quando necessário
- PR final enviado ao professor no formato correto

---

## Template do Arquivo do Grupo

```markdown
# Nome do Projeto do Grupo <id>

## Integrantes
- Nome 1 (@usuario1)
- Nome 2 (@usuario2)
- Nome 3 (@usuario3)
- ...

## Visão Geral do Projeto
Escreva aqui 4–6 frases explicando o projeto, sua motivação e seus objetivos.

## Público-Alvo
Descreva quem deve usar o projeto.

## Funcionalidades Principais
- Funcionalidade 1
- Funcionalidade 2
- Funcionalidade 3

---

## Contribuições Individuais

### Contribuição de @usuario1
Descreva em 3–5 frases o que você pretende fazer no projeto e por quê.

### Contribuição de @usuario2
(Preenchido pelo próximo integrante)

### Contribuição de @usuario3
(Preenchido pelo próximo integrante)
```
