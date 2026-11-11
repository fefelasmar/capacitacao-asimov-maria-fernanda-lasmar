# Git e GitHub — Semana 01

Este documento reúne os principais comandos e atividades realizados durante a primeira semana da capacitação da Asimov. O objetivo foi aprender a utilizar Git e GitHub para controlar versões de projetos, organizar alterações e trabalhar com diferentes branches.

## 1. Comandos básicos

| Comando | Função |
|---|---|
| `git init` | Inicializa um repositório Git. |
| `git clone` | Copia um repositório remoto para o computador. |
| `git status` | Mostra o estado atual dos arquivos. |
| `git add` | Prepara arquivos para o próximo commit. |
| `git commit` | Registra as alterações no histórico. |
| `git push` | Envia os commits para o GitHub. |
| `git pull` | Atualiza o repositório local com alterações remotas. |
| `git branch` | Lista as branches existentes. |
| `git switch` | Permite trocar de branch. |
| `git merge` | Integra alterações de outra branch. |
| `git log` | Exibe o histórico de commits. |
| `git remote -v` | Mostra os repositórios remotos conectados. |

## 2. Conventional Commits

Durante a capacitação, também foi trabalhado o padrão Conventional Commits, que organiza as mensagens de commit de acordo com o tipo de alteração realizada.

Os principais tipos utilizados são:

- `feat:` implementação de uma nova funcionalidade.
- `fix:` correção de erros.
- `docs:` alterações na documentação.
- `chore:` tarefas de configuração e manutenção.


## 3. Fluxo de trabalho com Git e GitHub

Uma das partes importantes da atividade foi aprender como organizar o desenvolvimento utilizando branches e Pull Requests.

O fluxo básico utilizado foi:

1. Criar ou clonar um repositório.
2. Criar uma branch para trabalhar em uma atividade específica.
3. Realizar as alterações nos arquivos.
4. Adicionar as alterações com `git add`.
5. Registrar as alterações com `git commit`.
6. Enviar a branch para o GitHub utilizando `git push`.
7. Abrir um Pull Request para integrar as alterações à branch principal (`main`).

Comandos utilizados nesse processo:

```bash
git switch -c nome-da-branch
git add .
git commit -m "docs: atualiza documentacao"
git push -u origin nome-da-branch
```

## 4. Resolução de conflito de merge

Durante a atividade, foi provocado intencionalmente um conflito de merge entre as branches `Teste1` e `Teste2`.

O conflito aconteceu porque as duas branches modificaram a mesma linha do arquivo `README.md` principal, mas com conteúdos diferentes. Na `Teste1`, foi adicionada uma referência ao Angular, enquanto na `Teste2` foi adicionada uma referência a HTML e CSS.

Ao tentar integrar as branches, o Git identificou o conflito e não conseguiu realizar a junção automaticamente.

### Identificação do conflito

O VS Code apresentou os marcadores de conflito no arquivo, indicando os trechos que precisavam ser analisados e resolvidos.

![Erro de conflito durante o merge](./imagens/erro1.png)

## Resolução de conflito de merge

Durante a atividade, foi provocado intencionalmente um conflito de merge entre as branches `Teste1` e `Teste2`.

O conflito aconteceu porque as duas branches modificaram a mesma linha do arquivo `README.md` principal, mas com conteúdos diferentes. Na `Teste1`, foi adicionada uma referência ao Angular, enquanto na `Teste2` foi adicionada uma referência a HTML e CSS.

Ao tentar integrar as branches, o Git identificou o conflito e não conseguiu realizar a junção automaticamente. Como indicado na foto, a seguir:

![Erro de conflito durante o merge](./imagens/erro1.png)


Para resolver, o arquivo foi aberto no VS Code, os marcadores de conflito foram identificados e removidos(sinais como "<,> e ="), e as duas informações foram mantidas no README (do Teste1, html e css, e do Teste 2, angular). Depois, a alteração foi adicionada e registrada com um commit. O que resultou em uma integração na main, das branchs teste1 e teste 2, ficando assim:

![Soluçãodo erro](.//imagens/erro2.png)

Depois desse erro, alterei os dados para as informações certas (mantendo apenas a semana 2 como html e css). E ficou assim: 

![Soluçãodo erro](.//imagens/erro3.png)


## Aprendizado

Durante a atividade, pratiquei os comandos básicos do Git, no ínicio digitava no automatico e esquecia de utilizar os commits convencionais, mas com a prática fui acostumando a modificalos de acordo com a norma.
Sobre o erro proposital, achei super interessante, a prática é diferente de assistir as aulas e como nunca tinha mexido com git ou github, gostei bastante.

## 6. Projeto complementar

Além das atividades da capacitação, também desenvolvi um currículo online para apresentar minhas informações acadêmicas, habilidades e experiências.

**[Acessar meu currículo online](https://fefelasmar.github.io/#home)**

## 7. Repositório da capacitação

[Voltar ao repositório principal da capacitação](https://github.com/fefelasmar/capacitacao-asimov-maria-fernanda-lasmar)