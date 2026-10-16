# Checklist do LinkedIn + preparação para a entrevista técnica

## Parte 1 — Arrumar o LinkedIn ANTES de mandar a mensagem

A recrutadora vai abrir seu perfil em segundos depois de receber a mensagem. O perfil é a
sua primeira entrevista.

- [ ] **Foto** de rosto, nítida, fundo neutro. Nada de foto cortada de festa.
- [ ] **Título (headline)** com as palavras que ela busca. Ex.:
      `Desenvolvedor Fullstack | .NET · C# · Angular · SQL Server`
      (não coloque só "Desenvolvedor" — o título é o campo que mais pesa na busca dela)
- [ ] **Localização** correta — a vaga é de Curitiba/PR; se você está em outra cidade,
      deixe claro na mensagem que topa remoto/mudança, senão o filtro te corta.
- [ ] **Seção "Sobre"** com 3 a 5 linhas: o que você faz, em que stack, qual domínio,
      e o que procura. Escreva em primeira pessoa, sem clichê de "apaixonado por tecnologia".
- [ ] **Experiências** com as mesmas entregas do currículo (pelo menos 2 bullets cada).
- [ ] **Competências** — adicione e deixe no topo: `C#`, `.NET`, `ASP.NET Core`, `Angular`,
      `TypeScript`, `SQL Server`, `Entity Framework`.
- [ ] **"Open to work"** ativado (pode deixar visível só para recrutadores, se preferir
      que a empresa atual não veja).
- [ ] **URL personalizada**: `linkedin.com/in/lucas-correia-dev` em vez do código aleatório.

## Parte 2 — O que cai numa entrevista de Fullstack Sênior .NET/Angular

Estude por aqui, na ordem de probabilidade:

### C# / .NET
- `async`/`await`: o que acontece por baixo, deadlock, `ConfigureAwait`, quando NÃO usar async
- Injeção de dependência e os tempos de vida: Singleton, Scoped, Transient (pergunta clássica)
- Entity Framework: lazy vs eager loading, problema do N+1, `AsNoTracking`, quando cair pro SQL puro
- Middleware, filtros e o pipeline de request do ASP.NET Core
- Garbage collector, `IDisposable`, `using`, structs vs classes
- Tratamento de erro, logging estruturado e validação (FluentValidation)

### Angular
- Change detection, `OnPush` e por que a tela "não atualiza"
- RxJS: `map`, `switchMap` vs `mergeMap` vs `concatMap`, `takeUntil` e vazamento de subscription
- Lazy loading de módulos, rotas e guards
- Formulários reativos vs template-driven
- Signals e standalone components (se o projeto for Angular 16+)
- Interceptors para token/JWT

### Banco de dados
- Índices: quando ajudam, quando atrapalham, índice composto
- Diferença entre os `JOIN`, e como ler um plano de execução
- Transação e nível de isolamento; deadlock
- Fazer uma query de média dificuldade no papel/tela compartilhada

### Arquitetura (é aqui que se decide o "sênior")
- Como você estruturaria uma aplicação nova hoje e **por quê** (Clean Architecture, camadas)
- Monolito vs microsserviço — e por que microsserviço nem sempre é a resposta
- Cache, fila (RabbitMQ/Service Bus), idempotência
- Autenticação/autorização: JWT, refresh token, OAuth
- Como você garante qualidade: testes, code review, CI

### Comportamental (prepare 3 histórias no formato situação → ação → resultado)
1. Um problema técnico difícil que você resolveu
2. Um conflito ou discordância técnica com o time, e como terminou
3. Um erro seu em produção e o que você mudou depois

## Parte 3 — Perguntas de dinheiro e contrato

Consultoria de alocação pergunta pretensão salarial cedo. Chegue com número pronto:

- Pesquise a faixa para Fullstack Sênior .NET em Curitiba (Glassdoor, Love Mondays,
  pesquisa salarial da Catho/Revelo, grupos de dev).
- Tenha **uma faixa**, não um número solto: "entre R$ [X] e R$ [Y], dependendo do modelo".
- **CLT e PJ não se comparam direto.** Em PJ você paga imposto, não tem 13º, férias nem FGTS.
  Regra prática de mercado: PJ costuma pedir de 20% a 40% a mais que o CLT equivalente.
- Se te empurrarem pra falar primeiro e você não souber a faixa, devolva:
  *"Qual a faixa prevista para a posição? Me adapto se estiver dentro do mercado."*

## Parte 4 — Não dependa de uma vaga só

Uma candidatura é uma loteria, dez é um processo. Na mesma semana:

- [ ] Candidate-se a 10 a 15 vagas de .NET/Angular (LinkedIn, Gupy, Programathor, Coodesh)
- [ ] Mande mensagem para 5 outros tech recruiters que postaram vagas da sua stack
- [ ] Peça indicação para 3 ex-colegas — indicação interna é o caminho com maior taxa de retorno
- [ ] Suba 1 ou 2 projetos bons no GitHub, com README explicando o que é e como rodar
      (hoje seu repositório está vazio — perfil de dev sênior com GitHub vazio levanta dúvida)
