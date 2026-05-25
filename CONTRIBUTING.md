# Guia de Contribuição

## Workflow adotado: GitHub Flow

1. Crie uma branch a partir da `main`
2. Faça commits descritivos
3. Abra um Pull Request
4. Aguarde revisão
5. Após aprovação, o professor faz o merge

## Nomenclatura de branches

```
feature/nome-sobrenome-descricao
```

Exemplos:
- `feature/joao-silva-perfil`
- `feature/maria-santos-perfil`

## Padrão de commits

Use [Conventional Commits](https://www.conventionalcommits.org/pt-br/):

```
<tipo>: <descrição curta em português>
```

| Tipo | Quando usar |
|------|-------------|
| `feat` | Nova funcionalidade ou adição de conteúdo |
| `fix` | Correção de algo errado |
| `docs` | Alteração apenas em documentação |
| `style` | Formatação, sem mudança de conteúdo |

Exemplos:
- `feat: adiciona perfil de João Silva`
- `docs: corrige link no README`

## O que não fazer

- Não commitar direto na `main`
- Não fazer merge sem PR aprovado
- Não deletar arquivos de outros alunos
