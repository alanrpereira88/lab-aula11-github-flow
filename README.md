# Lab — GitHub Flow

**DevOps I · Aula 11.1 · Unidade 2**

---

## O que é GitHub Flow?

GitHub Flow é um workflow leve baseado em branches. Possui uma única regra central:

> **`main` é sempre estável e deployável.**

Qualquer trabalho novo acontece em uma branch de vida curta. Quando pronto, a branch é integrada via Pull Request.

```
main  ──●────────────────────────●──  (sempre estável)
         \                      /
feature   ●── commit ── commit ──     (branch curta → PR → merge)
```

### Regras deste repositório

| Regra | Detalhe |
|-------|---------|
| Nunca commitar direto na `main` | A `main` só recebe código via PR aprovado |
| Uma branch por tarefa | Cada contribuição = uma branch |
| Nomenclatura | `feature/nome-sobrenome-descricao` |
| Todo merge via Pull Request | Sem merge direto no GitHub |

---

## Exercício — Adicione seu perfil ao time

### Passo 1 — Clone o repositório

```bash
git clone git@github-univertix:alanrpereira88/lab-aula11-github-flow.git
cd lab-aula11-github-flow
```

### Passo 2 — Crie sua branch a partir da `main`

```bash
git switch main
git pull
git switch -c feature/seu-nome-perfil
```

Exemplo: `feature/joao-silva-perfil`

### Passo 3 — Copie o template e preencha seu perfil

```bash
cp time/_template.md time/seu-nome.md
```

Edite `time/seu-nome.md` com suas informações reais.

### Passo 4 — Commit e push

```bash
git add time/seu-nome.md
git commit -m "feat: adiciona perfil de [Seu Nome]"
git push origin feature/seu-nome-perfil
```

### Passo 5 — Abra um Pull Request

1. Acesse o repositório no GitHub
2. Clique em **"Compare & pull request"**
3. Título: `feat: adiciona perfil de [Seu Nome]`
4. Descrição: descreva brevemente quem você é
5. Clique em **"Create pull request"**

### Passo 6 — Revise o PR de um colega

Leia o PR de outro aluno e aprove ou solicite ajuste.

---

## Entrega

- URL do Pull Request aberto no GitHub

---

## Estrutura do repositório

```
lab-aula11-github-flow/
├── README.md          ← você está aqui
├── CONTRIBUTING.md    ← regras de contribuição
├── docs/
│   └── sobre-o-projeto.md
└── time/
    ├── _template.md   ← copie este arquivo
    └── alan-pereira.md  ← exemplo do professor
```
