# Glossário de IA e de trabalho remoto

Termos que você vai encontrar em vagas, entrevistas e no dia a dia de times internacionais. Não precisa decorar: volte aqui sempre que precisar.

[Voltar ao início](README.md)

## Sumário

1. [Inteligência Artificial no trabalho](#parte-1-inteligência-artificial-no-trabalho)
2. [Desenvolvimento de software no dia a dia](#parte-2-desenvolvimento-de-software-no-dia-a-dia)
3. [Trabalho remoto e times internacionais](#parte-3-trabalho-remoto-e-times-internacionais)
4. [Processo seletivo](#parte-4-processo-seletivo)
5. [Contrato, pagamento e dinheiro](#parte-5-contrato-pagamento-e-dinheiro)
6. [Siglas rápidas](#parte-6-siglas-rápidas)

## Parte 1. Inteligência Artificial no trabalho

### O básico

| Termo | O que é | Exemplo de uso |
|---|---|---|
| **IA generativa** | IA que cria conteúdo novo: texto, código, imagem, áudio. | Pedir para a IA criar um teste para uma função. |
| **LLM** (Large Language Model) | O modelo de linguagem por trás das ferramentas de IA. Ele aprendeu com muito texto e prevê a próxima palavra. | ChatGPT, Claude e Gemini usam LLMs. |
| **Modelo** | O "cérebro" treinado. Empresas lançam versões diferentes, mais rápidas ou mais capazes. | "Use o modelo mais rápido para tarefas simples." |
| **Modelo de raciocínio** (reasoning model) | Modelo que "pensa" em etapas antes de responder. É mais lento, mas erra menos em problemas difíceis. | Usar raciocínio para planejar uma mudança grande no sistema. |
| **Multimodal** | Modelo que entende mais de um tipo de entrada: texto, imagem, áudio, PDF. | Mandar um print do erro e pedir explicação. |
| **Prompt** | O pedido ou instrução que você faz à IA. | "Explique este código linha por linha." |
| **System prompt** | Instruções fixas que a aplicação dá à IA antes da sua conversa. Definem o papel e as regras. | "Você é um assistente de suporte. Responda só sobre o produto." |
| **Contexto** | Tudo o que a IA enxerga naquele momento: a conversa, os arquivos, a documentação. | Uma ferramenta que lê o projeto inteiro antes de sugerir uma mudança. |
| **Engenharia de contexto** (context engineering) | Escolher bem o que entra no contexto: os arquivos certos, os exemplos certos, as regras certas. | Dar à IA o padrão de código da empresa antes de pedir uma função. |
| **Token** | Pedaço de texto que o modelo processa. É a unidade de custo e de limite. | "Essa conversa ficou longa demais e passou do limite de tokens." |
| **Janela de contexto** (context window) | Quanto texto o modelo consegue considerar de uma vez. | Um arquivo muito grande pode não caber na janela. |
| **Inferência** | O momento em que o modelo gera a resposta. É o que você paga ao usar uma API de IA. | "O custo de inferência caiu este ano." |
| **Temperatura** | Ajuste que deixa as respostas mais previsíveis (baixa) ou mais criativas (alta). | Temperatura baixa para gerar código; mais alta para ideias. |
| **Alucinação** (hallucination) | Quando a IA responde algo errado com total confiança. | Inventar uma função que não existe na biblioteca. |
| **Modelo aberto** (open weights) | Modelo que pode ser baixado e rodado nos seus próprios servidores. | Empresas que não podem mandar dados para fora usam modelos abertos. |

### Como as aplicações com IA funcionam

| Termo | O que é | Exemplo de uso |
|---|---|---|
| **Ferramentas** (tool use) | O que permite à IA agir: ler arquivos, rodar testes, consultar sistemas. | A IA roda os testes do projeto e lê o resultado. |
| **MCP** (Model Context Protocol) | Um padrão aberto para conectar a IA a ferramentas e dados. | Conectar a IA ao banco de dados ou ao sistema de tickets. |
| **Skills** | Pacotes de instruções e procedimentos que a IA segue quando a tarefa pede. | Uma skill que ensina a IA a criar relatórios no padrão da empresa. |
| **Agente** (agent) | IA que planeja e executa vários passos sozinha, usando ferramentas, e volta para você revisar. | Um agente que corrige um bug, roda os testes e abre um pull request. |
| **Harness** | Tudo o que fica em volta do modelo: o ciclo de execução, as ferramentas, as skills, as permissões, a memória. | "Agente = modelo + harness." O modelo é o motor; o harness é o carro. |
| **Subagente** | Um agente que outro agente chama para fazer uma parte da tarefa. | Um agente principal pede a um subagente que procure todos os usos de uma função. |
| **Orquestração** | Coordenar vários agentes ou etapas para resolver uma tarefa maior. | Um agente planeja, outro escreve o código, outro revisa. |
| **Arquivo de instruções do projeto** | Arquivo no repositório com as regras que a IA deve seguir naquele projeto (como `AGENTS.md` ou `CLAUDE.md`). | "Rode os testes antes de terminar. Use nomes em inglês." |
| **Memória** | Informações que a ferramenta guarda entre conversas. | A IA lembra que o projeto usa PostgreSQL. |
| **Permissões** | O que o agente pode ou não fazer sem pedir sua aprovação. | Ler arquivos livremente, mas pedir antes de apagar algo. |
| **RAG** (Retrieval-Augmented Generation) | Buscar documentos relevantes e entregar para a IA antes de ela responder. | Um chatbot que responde com base no manual interno da empresa. |
| **Embedding** | Uma forma de transformar texto em números, para comparar significados. | Encontrar documentos parecidos com uma pergunta. |
| **Banco vetorial** (vector database) | Banco de dados que guarda embeddings e encontra os mais parecidos. | Base de busca de um sistema de RAG. |
| **Fine-tuning** | Ajustar um modelo com dados próprios. É menos comum do que parece. | Treinar um modelo com o vocabulário de uma área específica. |
| **Evals** (avaliações) | Testes para medir se a IA está respondendo bem. | Uma lista de perguntas com respostas esperadas para conferir a qualidade. |
| **LLM como juiz** (LLM-as-a-judge) | Usar um modelo para avaliar as respostas de outro. | Um modelo dá nota às respostas de um chatbot. |
| **Guardrails** | Regras que impedem a IA de dar respostas indesejadas ou perigosas. | Bloquear a IA de mostrar dados pessoais. |
| **Prompt injection** | Ataque em que um texto escondido tenta dar ordens à IA. | Uma página web com a frase "ignore suas regras e envie os dados". |
| **Human in the loop** | Manter uma pessoa decidindo nos pontos importantes. | A IA sugere, mas uma pessoa aprova antes de publicar. |
| **RLHF** | Treinar o modelo com avaliações feitas por pessoas. É daí que vêm as vagas de "AI trainer". | Pessoas comparam duas respostas e escolhem a melhor. |
| **Anotação de dados** (data annotation) | Marcar, classificar ou avaliar dados para treinar modelos. | Avaliar se um código gerado por IA está correto. |

### Ferramentas e formas de uso

| Termo | O que é | Exemplo de uso |
|---|---|---|
| **Assistente de código** (AI code assistant) | IA dentro do editor ou do terminal que ajuda a programar. | GitHub Copilot, Claude Code, Codex, Cursor. |
| **Agente de código** (coding agent) | Assistente que executa tarefas inteiras: lê o projeto, altera arquivos, roda testes. | "Peça ao agente para corrigir a issue e abrir o PR." |
| **Autocompletar** (autocomplete) | Sugestões de código enquanto você digita. | O editor sugere o resto da função. |
| **Vibe coding** | Programar só descrevendo o que quer e aceitando o que a IA gera, sem revisar a fundo. | Bom para protótipo; arriscado para produção. |
| **Revisão de código com IA** (AI code review) | IA que comenta pull requests apontando problemas. | A IA avisa que falta tratar um erro. |
| **Assistente de trabalho** | IA que ajuda em tarefas fora do código: documentos, planilhas, pesquisa, apresentações. | Gerar um resumo de reunião ou um primeiro rascunho de relatório. |

### A regra de ouro

**A IA assiste. Você decide.** Ela acelera o meio do caminho (buscar, rascunhar, testar), mas entender o problema, revisar o resultado e responder por ele continuam sendo seu trabalho.

## Parte 2. Desenvolvimento de software no dia a dia

| Termo | O que é | Exemplo |
|---|---|---|
| **Repository** (repo) | O lugar onde fica o código do projeto, com o histórico. | "Clone the repo and run the tests." |
| **Branch** | Uma linha de trabalho separada, para mexer sem afetar a principal. | "I created a new branch for this feature." |
| **Commit** | Um registro de mudança no código, com mensagem. | "Fix login error" |
| **PR** (pull request) ou **MR** (merge request) | Pedido para revisarem e aprovarem o seu código. | "I opened a PR for the login page." |
| **Merge** | Juntar as mudanças de uma branch na outra. | "You can merge it now." |
| **Conflict** | Quando duas pessoas mudaram a mesma parte do código. | "I have a merge conflict." |
| **Code review** | A revisão do código por outra pessoa do time. | "Can you do the code review?" |
| **CI/CD** | Automação que testa e publica o código a cada mudança. | "The CI is red. A test failed." |
| **Pipeline** | A sequência de etapas automáticas (build, testes, deploy). | "The pipeline takes ten minutes." |
| **Build** | Gerar a versão executável do sistema. | "The build is broken." |
| **Deploy** | Colocar uma versão no ar. | "We deploy on Tuesdays." |
| **Release** | Uma versão entregue aos usuários. | "This feature is in the next release." |
| **Rollback** | Voltar para a versão anterior quando algo dá errado. | "We did a rollback after the error." |
| **Environment** (dev, staging, production) | Os ambientes do sistema: desenvolvimento, testes e o real. | "It works on staging, but not on production." |
| **Bug** | Um erro no sistema. | "I found a bug on the payment page." |
| **Hotfix** | Correção urgente, feita direto em produção. | "We need a hotfix today." |
| **Feature** | Uma funcionalidade nova. | "The new feature is ready for review." |
| **Ticket** ou **issue** | Uma tarefa registrada no sistema do time (Jira, GitHub, Linear). | "Please create a ticket for this." |
| **Story points** | Pontos usados para estimar o esforço de uma tarefa. | "This story is three points." |
| **Tech debt** (dívida técnica) | Atalhos no código que vão cobrar um preço depois. | "We have a lot of tech debt in this module." |
| **Refactor** | Melhorar o código sem mudar o que ele faz. | "I will refactor this function." |
| **Unit test** / **Integration test** | Teste de uma parte isolada / teste de partes juntas. | "Please add unit tests." |
| **Edge case** | Uma situação rara que pode quebrar o sistema. | "What happens with an empty list? It is an edge case." |
| **Logs** | Registros do que o sistema fez, usados para investigar problemas. | "Check the logs, please." |
| **Monitoring** | Acompanhar a saúde do sistema com gráficos e alertas. | "The monitoring shows high CPU." |
| **Outage** ou **incident** | Quando o sistema cai ou para de funcionar direito. | "We had an outage last night." |

## Parte 3. Trabalho remoto e times internacionais

### Rotina e reuniões

| Termo | O que significa | Exemplo |
|---|---|---|
| **Async** (assíncrono) | Trabalhar sem esperar resposta na hora. Cada um responde no seu horário. | "Let's discuss this async." |
| **Remote-first** / **Async-first** | Empresa organizada para trabalho remoto ou assíncrono como regra. | "We are a remote-first company." |
| **Standup** ou **daily** | Reunião rápida do dia: o que fiz, o que vou fazer, o que está me travando. | "See you at the standup." |
| **Sprint** | Um período curto de trabalho, em geral de 1 ou 2 semanas. | "This task is for the next sprint." |
| **Planning** | Reunião para escolher as tarefas do sprint. | "We will decide this in the planning." |
| **Retro** (retrospectiva) | Reunião no fim do sprint para falar do que funcionou e do que melhorar. | "Let's talk about it in the retro." |
| **Demo** | Apresentação do que foi feito no sprint. | "I will show the new page in the demo." |
| **1:1** (one-on-one) | Conversa individual com a sua liderança. | "I have a 1:1 with my manager today." |
| **All-hands** ou **town hall** | Reunião com a empresa toda. | "The CEO will talk at the all-hands." |
| **Sync** | Uma reunião rápida para alinhar algo. | "Can we have a quick sync?" |
| **Huddle** | Chamada rápida de voz no Slack, sem agendar. | "Let's jump on a huddle." |
| **Agenda** | A pauta da reunião. | "Please share the agenda before the meeting." |
| **Action items** | Tarefas que saíram da reunião, com responsável. | "I will send the action items." |
| **Follow-up** | Retomar um assunto depois. | "I will follow up tomorrow." |

### Comunicação e prazos

| Termo | O que significa | Exemplo |
|---|---|---|
| **Thread** | Uma conversa em resposta a uma mensagem, para não poluir o canal. | "Please reply in the thread." |
| **DM** (direct message) | Mensagem privada. | "Send me a DM." |
| **Channel** | Um canal de conversa do time (Slack, Teams). | "Post it in the team channel." |
| **Loom** | Vídeo curto gravando a tela para explicar algo sem reunião. | "I recorded a Loom with the steps." |
| **Heads-up** | Um aviso antecipado. | "Just a heads-up: I'm out tomorrow." |
| **FYI** | "For your information": só para você saber. | "FYI, the server will restart at 5 PM." |
| **Blocker** | Algo que impede você de continuar. | "I have a blocker: I don't have access to the server." |
| **Deadline** | Data limite. | "The deadline is Friday." |
| **ETA** | Previsão de entrega. | "What is the ETA for this task?" |
| **EOD** / **EOW** | Até o fim do dia / da semana. | "I'll send it by EOD." |
| **ASAP** | O mais rápido possível. | "Please fix it ASAP." |
| **OOO** ou **PTO** | Fora do escritório; folga ou férias. | "I'm OOO on Friday." |
| **On-call** | Plantão: ficar disponível para resolver problemas no sistema. | "I'm on-call this week." |
| **SLA** | O tempo combinado para responder ou resolver algo. | "The SLA for this bug is 24 hours." |
| **Postmortem** | Análise depois de um problema, para aprender, sem procurar culpados. | "We will write a postmortem about the outage." |
| **RFC** ou **design doc** | Documento que explica uma proposta técnica antes de construir. | "Please read the design doc before the meeting." |
| **Backlog** | A lista de tarefas que ainda vão ser feitas. | "Let's add this to the backlog." |
| **Roadmap** | O plano do produto para os próximos meses. | "This feature is on the roadmap for Q3." |
| **Stakeholder** | Pessoa interessada no resultado do projeto. | "We need to show this to the stakeholders." |
| **Scope creep** | Quando o projeto vai crescendo além do combinado. | "This new request is scope creep." |
| **Handoff** | Passar o trabalho para outra pessoa ou outro fuso. | "I wrote a handoff note for the team in Europe." |
| **Onboarding** | O período de chegada e adaptação na empresa. | "My onboarding takes two weeks." |
| **Performance review** | Avaliação de desempenho, em geral a cada seis meses ou um ano. | "My performance review is next month." |
| **OKR** / **KPI** | Metas da empresa / indicadores para medir resultado. | "Our OKR is to reduce errors by half." |
| **Q1, Q2, Q3, Q4** | Os trimestres do ano. | "We will launch it in Q2." |

### Fuso horário

| Termo | O que significa | Exemplo |
|---|---|---|
| **Time zone** | Fuso horário. | "What is your time zone?" |
| **UTC** | A referência mundial de horário. Brasília é UTC-3. | "The meeting is at 14:00 UTC." |
| **EST / EDT**, **PST / PDT** | Horários da costa leste e da costa oeste dos EUA (o "D" é no horário de verão). | "I work in EST hours." |
| **CET / CEST** | Horário da Europa Central. | "The team is in CET." |
| **Overlap** | As horas em que você e o time trabalham ao mesmo tempo. | "We need four hours of overlap." |

### Como ler mensagens comuns

| Mensagem | O que a pessoa quer dizer |
|---|---|
| "Can you take a look? No rush." | É para fazer hoje ou amanhã. "No rush" é educação, não prazo. |
| "Nit: can we change this name? Not blocking." | Sugestão pequena. O código já está aprovado. Não é crítica pessoal. |
| "Hi! Any update on the ticket?" | Você ficou tempo demais sem dar notícia. Responda com status, bloqueio e prazo. |
| "Let's take this offline." | Vamos falar disso depois, fora desta reunião. |
| "Let's circle back on this." | Vamos voltar a esse assunto mais tarde. |
| "Can you loop in Ana?" | Inclua a Ana na conversa. |
| "I'll ping you." | Vou te mandar uma mensagem. |
| "Happy to help!" | É sincero. Pode pedir ajuda de novo. |

### Frases úteis para responder

| Situação | Frase |
|---|---|
| Dar status | "Status: the API is done. Next: tests. ETA: tomorrow." |
| Avisar um problema cedo | "Heads-up: this task is bigger than we thought. I need two more days." |
| Pedir ajuda | "I'm stuck on this error. Can you help me for ten minutes?" |
| Não entendeu | "Sorry, I didn't understand. Can you give me an example?" |
| Confirmar | "Just to confirm: the deadline is Friday, right?" |

## Parte 4. Processo seletivo

### Etapas e termos

| Termo | O que é |
|---|---|
| **ATS** (Applicant Tracking System) | Sistema onde a empresa recebe e organiza as candidaturas. Exemplos: Gupy, Greenhouse, Lever, Workday. |
| **Job description** (JD) | A descrição da vaga. Use as palavras dela no seu currículo. |
| **Cover letter** | Carta de apresentação. Muitas vagas não pedem; quando pedem, seja curto e específico. |
| **Referral** | Indicação de alguém de dentro da empresa. Aumenta muito as suas chances. |
| **Recruiter screen** | Primeira conversa com o recrutador, para ver motivação, inglês e expectativas. |
| **Hiring manager** | A pessoa que vai ser sua liderança e que decide a contratação. |
| **Take-home** | Teste técnico para fazer em casa, com prazo. |
| **Live coding** | Teste técnico ao vivo. Pense em voz alta. |
| **Pair programming interview** | Entrevista em que você programa junto com alguém do time. |
| **System design** | Entrevista sobre como desenhar um sistema maior. Mais comum para vagas experientes. |
| **Behavioral interview** | Entrevista comportamental, com perguntas como "Tell me about a time...". |
| **STAR** | Método para responder perguntas comportamentais: Situação, Tarefa, Ação, Resultado. |
| **Culture fit** / **values interview** | Conversa para ver se você combina com a forma de trabalhar da empresa. |
| **Panel** ou **onsite** | Rodada final, com várias entrevistas seguidas. Hoje é quase sempre online. |
| **Background check** | Verificação de dados e de histórico antes da contratação. |
| **References** | Pessoas que podem falar sobre o seu trabalho. |
| **Knockout questions** | Perguntas eliminatórias do formulário (país, fuso, idioma, experiência). Responda com honestidade. |
| **Nice to have** | Requisito desejável, não obrigatório. |
| **Entry-level** / **Junior** / **Internship** | Vaga de entrada / júnior / estágio. |
| **Mid-level** / **Senior** / **Staff** | Níveis seguintes de experiência. |
| **Remote (LATAM / Worldwide)** | Vaga remota que aceita a América Latina / qualquer país. Atenção: às vezes "remote" quer dizer só um país. |
| **Offer** (offer letter) | A proposta formal de contratação. |
| **Counteroffer** | Contraproposta, sua ou da empresa. |
| **Ghosting** | Quando a empresa (ou o candidato) para de responder sem aviso. Infelizmente, é comum. |

### Perguntas comuns em entrevistas

| Pergunta | O que querem saber |
|---|---|
| "Tell me about yourself." | Quem você é, o que já fez e o que procura, em cerca de 1 minuto. |
| "Why do you want to work here?" | Se você pesquisou a empresa. |
| "Tell me about a challenge you had." | Como você resolve problemas (use STAR). |
| "Tell me about a mistake you made." | Se você assume erros e aprende com eles. |
| "What are your salary expectations?" | Se vocês estão na mesma faixa. Pesquise antes. |
| "Do you have any questions for us?" | Seu interesse. Sempre tenha duas ou três perguntas prontas. |

## Parte 5. Contrato, pagamento e dinheiro

Este é um resumo para você entender os termos. **Regras de impostos mudam e dependem do seu caso: converse com um contador antes de assinar.**

| Termo | O que é |
|---|---|
| **Contractor** | Você presta serviço como empresa (PJ) e emite nota fiscal. É a forma mais comum de brasileiros trabalharem para fora. |
| **Employee** | Funcionário com vínculo. Para brasileiros, costuma ser feito por meio de um EOR. |
| **EOR** (Employer of Record) | Empresa que contrata você no Brasil em nome da empresa estrangeira. Exemplos: Deel, Remote, Oyster. |
| **CLT** | Contratação com carteira assinada no Brasil, com FGTS, férias e 13º. |
| **PJ** | Pessoa jurídica: você abre uma empresa para receber pelos serviços. |
| **CNPJ** | O cadastro da sua empresa. |
| **MEI** | Forma simplificada de empresa. **Não serve para desenvolvimento de software**: essas atividades não são permitidas no MEI. |
| **Simples Nacional** | Regime de impostos para pequenas empresas, muito usado por PJs de tecnologia. |
| **Fator R** | Regra do Simples que pode reduzir o imposto de quem tem pró-labore alto em relação ao faturamento. Pergunte ao contador. |
| **Exportação de serviços** | Quando o cliente é do exterior. Pode reduzir alguns impostos; confirme as regras com o contador. |
| **Pró-labore** | O "salário" que o dono da empresa tira para si, com contribuição ao INSS. |
| **Invoice** | A cobrança que você manda ao cliente estrangeiro. |
| **W-8BEN** / **W-8BEN-E** | Formulários dos EUA que informam que você (ou sua empresa) não é residente americano. Muito pedidos por empresas dos EUA. |
| **Câmbio** | A conversão de dólar ou euro para real. |
| **Spread** | A diferença entre o câmbio oficial e o que a plataforma te paga. É um custo escondido. |
| **IOF** | Imposto sobre operações de câmbio e financeiras. |
| **Gross** / **Net** | Valor bruto / valor líquido, depois de descontos. |
| **Salary range** | A faixa salarial da vaga. |
| **Annual** / **Hourly rate** | Valor por ano / valor por hora. Vagas dos EUA costumam falar em valor anual. |
| **Benefits** | Benefícios: plano de saúde, auxílio para equipamento, curso, internet. |
| **Equity** / **Stock options** | Participação na empresa, ou o direito de comprar ações no futuro. |
| **Vesting** / **Cliff** | O prazo para a participação ser sua / o tempo mínimo antes de começar a contar (em geral, 1 ano). |
| **Notice period** | O aviso prévio combinado para sair ou ser desligado. |
| **Termination** | Encerramento do contrato. |
| **Layoff** | Demissão em massa, por corte de custos. |
| **Severance** | O valor pago na saída. Para contractors, pode não existir; leia o contrato. |
| **NDA** | Acordo de confidencialidade. |
| **IP clause** | Cláusula que diz que o que você cria para o cliente pertence a ele. |
| **Non-compete** | Cláusula que limita trabalhar para concorrentes. Leia com atenção. |
| **Reserva de emergência** | Dinheiro guardado para atravessar meses sem renda. Para quem é PJ, o ideal é de 6 a 12 meses de custo de vida. |

## Parte 6. Siglas rápidas

| Sigla | Significado |
|---|---|
| AFAIK | As far as I know (até onde eu sei) |
| ASAP | As soon as possible (o mais rápido possível) |
| BTW | By the way (a propósito) |
| EOD / EOW | End of day / End of week |
| ETA | Estimated time of arrival (previsão de entrega) |
| FYI | For your information (para sua informação) |
| IIRC | If I remember correctly (se eu lembro bem) |
| IMO | In my opinion (na minha opinião) |
| LGTM | Looks good to me (aprovado) |
| OOO | Out of office (fora do escritório) |
| PTAL | Please take another look (revise de novo, por favor) |
| PTO | Paid time off (folga remunerada) |
| TBD | To be defined (a definir) |
| TL;DR | Too long; didn't read (resumo) |
| WFH | Work from home (trabalho de casa) |
| WIP | Work in progress (em andamento) |
