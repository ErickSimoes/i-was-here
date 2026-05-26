# 🚀 Atividades Práticas de Git e GitHub - Semestre 2026.1

---

## 🎯 Fase 1: Meu Primeiro Repositório (Individual)

Nesta primeira fase, o objetivo é criar o seu próprio repositório, entender os conceitos iniciais de versionamento e subir seu primeiro código.

### Passo a passo

1. **Crie ou acesse sua conta no GitHub:** Acesse [github.com](https://github.com) e faça login.
2. **Crie um novo repositório:** - Clique no botão **`New`** ou no ícone de `+` no canto superior direito.
   - Nomeie o repositório como `atividades-ic-git-2026-1`.
   - Deixe o repositório como **Public** (Público).
   - Marque a opção **"Add a README file"**.
   - Clique em **Create repository**.
3. **Clone o repositório para a sua máquina:**
   - No seu terminal, rode o comando:

     ```bash
     git clone https://github.com/SEU_USUARIO/atividades-ic-git-2026-1.git
     ```

4. **Adicione um arquivo de anotações:**
   - Entre na pasta do projeto:

     ```bash
     cd atividades-ic-git-2026-1
     ```

   - Crie um arquivo chamado `meus-aprendizados.txt` e adicione um pequeno texto sobre o que você já aprendeu neste semestre.
5. **Faça o Commit e o Push:**
   - Adicione o arquivo ao *staging area*:

     ```bash
     git add meus-aprendizados.txt
     ```

   - Faça o *commit* com uma mensagem descritiva:

     ```bash
     git commit -m "docs: adiciona arquivo de aprendizados da fase 1"
     ```

   - Envie as alterações para o GitHub (*Push*):

     ```bash
     git push origin main
     ```

**Guarde o link desse repositório, você vai precisar dele na Fase 3!**

---

## 🤝 Fase 2: Colaboração (Trabalho em Dupla)

No mundo real, nunca trabalhamos sozinhos. Nesta fase, você fará uma contribuição no repositório de um colega da turma.

### Passo a passo

1. **Encontre sua dupla:** Troque o link do repositório da Fase 1 com um colega.
2. **Faça o Fork do repositório do colega:**
   - Acesse o link do repositório do seu colega.
   - Clique no botão **`Fork`** no canto superior direito da página e confirme para copiar o repositório para a sua conta.
3. **Clone o SEU Fork:**
   - Cuidado: clone o link que está na *sua* conta agora, não o do seu colega!

     ```bash
     git clone https://github.com/SEU_USUARIO/atividades-ic-git-2026-1.git
     ```

4. **Crie uma nova *Branch*:**
   - É uma boa prática nunca trabalhar direto na branch `main` ao colaborar.

     ```bash
     git checkout -b add-colaborador-seu-nome
     ```

5. **Faça sua contribuição:**
   - Edite o arquivo `README.md` do seu colega e adicione uma seção chamada "Colaboradores".
   - Adicione o seu nome e uma pequena mensagem de incentivo para o semestre. (seja decente)
6. **Commit e Push:**
   - Salve as alterações:

     ```bash
     git add README.md
     git commit -m "feat: adiciona assinatura de colaborador no README"
     git push origin add-colaborador-seu-nome
     ```

7. **Abra um *Pull Request* (PR):**
   - Acesse o GitHub, vá até a página do seu fork e você verá um botão verde dizendo **`Compare & pull request`**. Clique nele.
   - Deixe uma mensagem amigável e confirme a criação do PR para o repositório original do seu colega.
8. **Aceite o PR do seu colega:**
   - Volte ao seu próprio repositório original. Você deve ter recebido um *Pull Request* do seu colega. Revise a alteração e clique em **`Merge pull request`**.

---

## 🌍 Fase 3: I Was Here (Open Source)

Agora que você já sabe como colaborar, você fará sua primeira contribuição em um repositório Open Source externo! Vamos usar este projeto para isso!

O seu objetivo é fazer um PR neste repositório adicionando os seus dados, **identificando-se com o e-mail da School** e colocando o **link do repositório que você criou na Fase 1**.

### Passo a passo

1. **Acesse o repositório alvo:**
   - Acesse: [https://github.com/ErickSimoes/i-was-here](https://github.com/ErickSimoes/i-was-here)
2. **Faça o Fork do repositório:**
   - Clique em **`Fork`** no canto superior direito para trazer uma cópia desse repositório para a sua conta.
3. **Clone o fork e crie uma branch:**
   - No terminal:

     ```bash
     git clone https://github.com/SEU_USUARIO/i-was-here.git
     cd i-was-here
     git checkout -b contribuicao-2026-1-SEUNOME
     ```

4. **Adicione as suas informações:**
   - Acesse ao arquivo `i-was-here.md`;
   - Siga o template proposto nas primeiras linhas do arquivo;
5. **Commit e Push:**
   - Faça o commit das suas alterações:

     ```bash
     git add .
     git commit -m "feat: adiciona assinatura de SEU_NOME, email da School e link das atividades"
     git push origin contribuicao-2026-1-SEUNOME
     ```

6. **Crie o *Pull Request* Final:**
   - Volte para o GitHub no seu fork de `i-was-here`.
   - Clique em **`Compare & pull request`**.
   - No título do PR, coloque algo como: `feat: Adiciona contribuição de [Seu Nome] - Turma [A/B] 2026.1`.
   - Na descrição do PR, explique rapidamente que esta é a atividade da turma [A/B] do semestre 2026.1 e que o link das práticas anteriores está incluso.
   - Clique em **Create pull request**.

🎉 **Parabéns!** Você completou todo o ciclo do Git e GitHub, desde a criação local até a contribuição remota e open source!
