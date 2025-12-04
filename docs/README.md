# 📘 **Guia Completo de Comandos Git — Explicado**

Um guia prático, objetivo e explicativo dos principais comandos Git para configuração, uso diário, branches, inspeção e resolução de conflitos.

---

# 🚀 **1. Configuração Inicial do Git**

```bash
git config --global user.name "erick.eleuterio"      # Define seu nome nos commits
git config --global user.email "e-mail"              # Define seu e-mail nos commits
git config --system editor vim                       # Define o editor padrão (vim)
git config --global --edit                           # Abre o arquivo global de configurações para edição
git config --global alias.c "commit -ma"             # Cria um atalho: 'git c "msg"' já commita e adiciona
git config --list                                    # Lista todas as configurações atuais
```

---

# 📂 **2. Comandos Básicos — Inicialização e Fluxo Diário**

```bash
git init                         # Cria um novo repositório Git local
git clone [url]                  # Clona um repositório remoto para sua máquina
git add [arquivo]                # Adiciona arquivos ao staging (pronto para commit)
git commit -m "mensagem"         # Salva mudanças com uma mensagem descritiva
git push                         # Envia commits para o repositório remoto
git pull                         # Baixa e mescla as mudanças do remoto
```

---

# 🌿 **3. Gerenciamento de Branches**

```bash
git branch                       # Lista branches locais
git branch novo-branch           # Cria um novo branch
git checkout [branch]            # Troca para o branch especificado
git merge [branch]               # Junta o branch indicado ao branch atual
git branch -D [branch]           # Deleta um branch local
```

### Exemplos:

```bash
git branch dev                   # Cria branch 'dev'
git checkout dev                 # Troca para o branch dev
git merge dev                    # Mescla 'dev' no branch atual
git branch -D dev                # Remove branch dev
```

---

# 🛠️ **4. Utilitários do Dia a Dia**

```bash
git stash                        # Guarda alterações temporariamente sem commitar
git stash pop                    # Restaura a última stash e remove ela da lista
git status                       # Mostra arquivos modificados e prontos para commit
git log                          # Mostra histórico de commits
git log --graph --oneline --all  # Histórico resumido em formato gráfico
git remote -v                    # Lista os repositórios remotos configurados
git remote add origin [url]      # Adiciona repositório remoto chamado 'origin'
```

---

# 🔧 **5. Resolução de Conflitos e Limpeza**

```bash
git stash list                   # Lista todas as stashes criadas
git stash apply                  # Aplica a stash sem removê-la
git stash drop                   # Remove uma stash específica
git reset --soft HEAD~1          # Remove o último commit, mantendo mudanças staged
git reset HEAD [arquivo]         # Remove arquivo do staging (desfaz 'git add')
git checkout -- [arquivo]        # Descarta alterações no arquivo e volta ao último commit
```

---

# 🧭 **6. Branches Avançados (moderno)**

```bash
git switch [branch]              # Troca para um branch (substitui checkout)
git switch -c novo-branch        # Cria e troca para um novo branch
git branch -m antigo novo        # Renomeia um branch
```

---

# 🔍 **7. Inspeção e Comparação**

```bash
git diff                         # Mostra diferenças não commitadas
git diff --staged                # Mostra diferenças do staged (após 'git add')
git show [commit]                # Mostra detalhes de um commit específico
```
