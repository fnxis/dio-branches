# Tutorial: Colaborando em um Repositório GitHub

## 1. **Usando o GitHub pelo Navegador (Web)**

### A. Para quem vai fazer Pull Request (Contribuidor)

#### **Repositório Público**
1. **Faça um fork** do repositório clicando em "Fork" no canto superior direito.
2. **Clone o fork** para sua máquina:
   ```bash
   git clone https://github.com/SEU_USUARIO/NOME_DO_REPO.git
   ```
3. **Crie um novo branch** para sua alteração:
   ```bash
   git checkout -b minha-feature
   ```
4. Faça as alterações desejadas nos arquivos do projeto.
5. **Adicione e faça commit das alterações:**
   ```bash
   git add .
   git commit -m "Adiciona minha nova feature"
   ```
6. **Envie o branch para seu fork no GitHub:**
   ```bash
   git push origin minha-feature
   ```
7. **No GitHub**, acesse seu repositório forkado. Aparecerá um botão “Compare & pull request” – clique nele.
8. Preencha o título e a descrição do Pull Request e clique em “Create pull request”.

#### **Repositório Privado**
- O mantenedor precisa adicionar você como colaborador.
- Depois, siga o mesmo passo a passo acima (não precisa fazer fork, pode clonar direto o repositório principal).

---

### B. Para quem é o Dono do Repositório

#### **Adicionar um colaborador (apenas para repositórios privados):**
1. Acesse o repositório no GitHub.
2. Vá em **Settings > Collaborators**.
3. Clique em **Add people** e digite o nome de usuário da pessoa.
4. Espere a pessoa aceitar o convite.

---

## 2. **Usando o Git Bash (Terminal)**

### A. Clonando o repositório

- **Público** (fork):
  ```bash
  git clone https://github.com/SEU_USUARIO/NOME_DO_REPO.git
  ```
- **Privado** (colaborador):
  ```bash
  git clone https://github.com/DONO/NOME_DO_REPO.git
  ```

### B. Criando e usando branches

```bash
git checkout -b meu-branch
# Faça suas alterações
git add .
git commit -m "Descrição da alteração"
git push origin meu-branch
```

### C. Criando Pull Request pelo navegador

1. Após dar push do branch, vá até o repositório no GitHub.
2. Clique em “Compare & pull request” ou vá na aba **Pull requests** e clique em **New pull request**.
3. Compare seu branch com o branch principal (normalmente `main` ou `develop`).
4. Preencha o título e descrição, clique em **Create pull request**.

---

## 3. **Resumo Visual**

```
1. Fork (se público)
2. Clone
3. Novo branch
4. Alterações
5. Commit
6. Push
7. Pull Request
```

---

## 4. **Dicas**

- Sempre crie um branch novo para cada alteração.
- Escreva mensagens de commit claras.
- Use o campo de descrição do Pull Request para explicar o que sua alteração faz.

---

Se precisar de um passo a passo para um caso específico (ex: usando GitHub Desktop ou CLI), é só pedir!
