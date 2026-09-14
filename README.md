🧭 Guia GitHub — Caderno Temático (NotebookLM)

🎯 Contexto e Objetivos

Escolhi o GitHub como tema deste caderno temático porque, apesar de já ter alguma experiência com desenvolvimento, ainda não dominava a ferramenta na prática. Vi no desafio uma boa oportunidade de aprender GitHub de forma estruturada, usando IA como apoio ativo de estudo — e já documentar esse aprendizado em um repositório real, reforçando o próprio portfólio.

Objetivos de estudo:
- Entender a diferença entre Git e GitHub e como eles se complementam
- Compreender o fluxo básico de trabalho (working directory → staging → commit → push)
- Aprender conceitos de colaboração (fork, clone, pull request, merge)
- Conhecer os principais recursos do GitHub como plataforma (Pages, Actions, Copilot, perfil/portfólio)

---

📚 Curadoria de Fontes

Fontes selecionadas e enviadas ao NotebookLM:

1. GitHub Learn (Skills) — trilhas interativas oficiais, cobrindo desde "Introduction to GitHub" até GitHub Actions e segurança — https://skills.github.com
2. GitHub Docs — Get Started — documentação oficial com primeiros passos — https://docs.github.com/pt/get-started
3. GitHub Docs — Repositórios — criação e gerenciamento de repositórios — https://docs.github.com/pt/repositories
4. GitHub Education — Git Cheat Sheet (PDF) — resumo oficial dos comandos e conceitos principais — https://education.github.com/git-cheat-sheet-education.pdf
5. Curso Git e GitHub — Professor José de Assis (YouTube, playlist) — curso prático em vídeo cobrindo o fluxo completo — https://www.youtube.com/playlist?list=PLbEOwbQR9lqzK14I7OOeREEIE4k6rjgIj

---

 🧠 Engenharia de Prompts e "Cicatrizes"

Documentação dos prompts testados no NotebookLM, respostas obtidas e observações do processo.

 Prompt 1 — Mapeamento inicial
> "Quais são os cursos essenciais para iniciantes no GitHub?"

Resposta obtida (resumo): o NotebookLM organizou os cursos em duas categorias — trilhas oficiais do GitHub Learn/Skills (divididas em "primeiro dia" e "primeira semana" no GitHub) e cursos práticos em vídeo no YouTube (José de Assis, Tiago Matos). Trouxe também menção ao papel do GitHub Copilot e do GitHub Actions no ecossistema atual.

Observação:resposta bem completa e organizada por categorias — não precisou de reformulação. Boa fonte pra montar a curadoria de fontes acima.

Prompt 2 — Conceito básico
> "Explique o que é um repositório como se eu fosse iniciante"

Resposta obtida (resumo): usou a analogia de uma "pasta de projeto com máquina do tempo", comparando com a bagunça de pastas tipo `projeto_final_v2` sem controle de versão. Explicou snapshots, histórico e a diferença entre repositório local e remoto.

Observação: a analogia funcionou muito bem para fixar o conceito — prompts pedindo "como se eu fosse iniciante" geram respostas mais didáticas e menos técnicas.

Prompt 3 — Comparação de conceitos
> "Qual a diferença entre fork e clone?"

Resposta obtida (resumo):trouxe uma tabela comparativa clara (localização, origem→destino, como executar, objetivo) e explicou como os dois comandos trabalham juntos no fluxo de contribuição em projetos open source (fork → clone → alteração/push → pull request).

Observação:pedir explicitamente uma comparação gerou uma resposta em formato de tabela, o que facilitou bastante o entendimento — vale repetir esse tipo de prompt para outros pares de conceitos (ex: push vs. pull, merge vs. rebase).

Dificuldades encontradas
- Perguntas muito abertas (ex: "me fale sobre GitHub") tendem a gerar respostas genéricas demais — funcionou melhor pedir explicações direcionadas ("como se eu fosse iniciante", "com uma tabela comparativa").
- Vale sempre revisar se a fonte usada pelo NotebookLM é atual, já que o GitHub lança recursos novos com frequência (ex: Copilot, Actions).

---

📖 Miniguia de Estudo (Entrega Final)

Resumos estruturados

Git vs. GitHub

| | Git | GitHub |
|---|---|---|
| O que é? | Software de linha de comando para controle de versão | Serviço de hospedagem e rede social para repositórios Git |
| Onde opera? | Localmente, no computador | Na nuvem |
| Função principal | Rastrear histórico de alterações de arquivos | Facilitar colaboração, backup remoto e automação de times |
| Custo | 100% gratuito e open source | Gratuito para uso pessoal, planos pagos para empresas |

As quatro zonas do Git

`Working Directory` (arquivos atuais) → `git add` → `Staging Area` (preparação) → `git commit` → `Local Repository` (histórico salvo) → `git push` → `Remote Repository` (backup na nuvem/GitHub)

Ciclo de trabalho diário
1. `git status` — inspecionar o que mudou
2. `git add [arquivo]` — preparar as mudanças
3. `git commit -m "mensagem"` — registrar a alteração
4. `git push` — enviar para o GitHub

Branches e colaboração
- `git branch [nome]` cria uma ramificação para trabalhar em algo novo sem afetar o código principal (`main`)
- `git merge [branch]` une o trabalho de volta — se duas pessoas alterarem a mesma linha, o Git aponta um conflito que precisa ser resolvido manualmente
- Fork cria uma cópia do projeto de outra pessoa na sua conta do GitHub; **clone** baixa um repositório para o computador. O fluxo de colaboração em projetos abertos costuma ser: fork → clone → alteração → push → pull request

GitHub como plataforma
- Perfil/Portfólio:README.md personalizado com Markdown, selos (shields.io)
- GitHub Pages: hospedagem gratuita de sites estáticos direto do repositório
- Issues & Projects:uadros Kanban para gerenciar tarefas
- GitHub Actions:automação de testes e deploy (CI/CD)
- GitHub Copilot:IA que ajuda a gerar código, revisar pull requests e modernizar sistemas

Glossário

| Termo | Definição |
|---|---|
| Repositório | Pasta do projeto com todo o histórico de alterações |
| Commit | Registro (snapshot) de uma alteração salva |
| Branch | Linha paralela de desenvolvimento |
| Merge | União do histórico de uma branch com outra |
| Fork | Cópia de um repositório de outra pessoa para a sua conta |
| Clone | Download de um repositório remoto para o computador |
| Push | Envio de commits locais para o repositório remoto |
| Pull | Busca e mescla de commits do remoto para o local |
| Staging Area | Área de preparação antes do commit |
| Pull Request | Pedido para que suas alterações sejam incorporadas ao projeto original |

Prompts reutilizáveis (para revisão futura)

- "Explique [conceito] como se eu fosse iniciante"
- "Qual a diferença entre [conceito A] e [conceito B]? Traga uma tabela comparativa"
- "Quais são os comandos essenciais para [tarefa específica, ex: resolver conflitos de merge]?"
- "Me dê um passo a passo prático para [ação, ex: criar minha primeira Pull Request]"

---

*Material produzido com apoio do NotebookLM como parte do desafio de projeto da DIO.*
