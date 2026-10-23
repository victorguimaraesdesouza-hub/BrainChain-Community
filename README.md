# BrainChain Community

**Vários agentes de IA, um único lugar para trabalhar.**

O **BrainChain Orchestrator** é um aplicativo de desktop para quem programa com agentes de IA. Em vez de alternar entre um terminal do Claude Code, outro do Codex, uma aba do navegador e um editor, você abre tudo isso lado a lado, organizado por workspace e por projeto, e deixa os agentes trabalharem juntos.

Este repositório é o ponto de encontro público do projeto: aqui você acompanha o que está sendo construído, tira dúvidas e fica sabendo quando abrirem novas vagas de teste.

> **Status:** em construção, em **alpha teste fechado**. Ainda não há versão pública para baixar. Em breve serão liberadas mais vagas para testadores. Veja [Como acompanhar](#como-acompanhar).

---

## O que é o BrainChain

O BrainChain é uma IDE multiagente. Cada agente roda no seu próprio painel de terminal, dentro do projeto certo, e você controla todos da mesma tela: abre, pausa, renomeia, manda instruções, aprova o que eles pedem e vê o que cada um está fazendo.

A ideia central é simples: **usar sempre o agente certo, com o modelo certo, para cada tarefa**, e permitir que eles conversem entre si, dividam o trabalho e entreguem uns para os outros, com você no controle das decisões importantes.

O BrainChain não substitui os agentes que você já usa. Ele roda as próprias CLIs oficiais (Claude Code, Codex, OpenCode e outras), com o login e o plano que você já tem em cada uma, e acrescenta a organização, a comunicação e o controle em volta delas.

## Para quem é

- Quem programa com agentes de IA no dia a dia e já se pegou com cinco terminais abertos.
- Quem usa mais de um provedor (Anthropic, OpenAI, Google, modelos locais...) e quer escolher o melhor para cada tarefa.
- Quem quer pôr vários agentes trabalhando em paralelo sem perder o controle do que eles fazem.
- Quem prefere rodar modelos no próprio computador.

Hoje o aplicativo roda no **Windows**.

## O que já dá para fazer

### Workspaces, projetos e painéis
- Organize o trabalho em **workspaces** e **projetos**, cada um apontando para a sua pasta.
- Abra vários agentes ao mesmo tempo em **painéis** que você redimensiona, minimiza, maximiza ou destaca em janelas próprias.
- Busque workspaces, projetos e agentes pela barra lateral, fixe os favoritos e veja de relance quem está trabalhando.
- Abra também **terminais comuns** (Prompt de Comando, PowerShell, Git Bash) como painéis do projeto.

### Agentes suportados
O BrainChain trabalha com as CLIs oficiais de cada fornecedor. A instalação é opcional e você escolhe quais quer usar:

Claude Code · Codex · OpenCode · Antigravity · Copilot · Cursor Agent · Qwen Code · Amp · Factory Droid · Mistral Vibe · Kimi Code · MiMo Code · Grok Build · Ollama e outros servidores de IA local

Cada agente aparece no menu só quando a CLI correspondente está instalada e disponível no seu computador.

### Agentes que conversam entre si
- O BrainChain tem um servidor **MCP** próprio que conecta os agentes: eles trocam mensagens, delegam tarefas uns aos outros, registram e acompanham tarefas e consultam o que os outros agentes do workspace estão fazendo.
- **Memória por projeto:** cada projeto guarda um resumo vivo (decisões, próximos passos, tarefas abertas) que os agentes leem ao começar, para não recomeçar do zero a cada sessão.
- **Squad Mode:** monte um time com papéis definidos, um coordenador e regras de quem pode decidir o quê. Um **Tomador de Decisão** opcional ajuda quando há mais de um caminho plausível.

### Você no controle
- **Modos de aprovação** por workspace e por agente: *Padrão*, *Pedir aprovação* ou *Livre*.
- Quando um agente pede permissão, o pedido aparece em cima da conversa dele, com ação, motivo, risco e escopo. Aprovar ou recusar exige confirmação, e a decisão volta sozinha para o agente.
- Uma caixa de aprovações reúne todos os pedidos e o histórico do workspace.

### Escrever para os agentes
- Uma barra de digitação compartilhada, com histórico, desfazer/refazer e referências: `@` para citar um agente e `#` para citar um projeto.
- Menu **`/`** com os comandos da CLI de cada agente.
- **FlyKey:** uma janela flutuante para mandar instruções rapidamente, sem sair do que você está fazendo.

### Tudo ao lado dos agentes
- **Word Code:** editor de arquivos integrado, com visualização das diferenças.
- **Arquivos e Git:** árvore de arquivos, status, diff, histórico, stage, commit e sincronização.
- **Navegador** embutido, com abas, favoritos, histórico e ferramentas de inspeção.
- **Anotações:** notas em Markdown suas e dos agentes, com rascunhos, compartilhamento e exportação.

### Modo chat e voz
- Um **modo chat** para conversar direto com o assistente do BrainChain, com conversas salvas no seu computador.
- **Modo voz:** você fala, o BrainChain transcreve e responde falando. A transcrição é feita no próprio computador; o áudio não sai da máquina.

### IA local
- Conecte servidores de IA que rodam no seu computador, como **Ollama**, **LM Studio** e **llama.cpp**, e use esses modelos como agentes.
- Com o Ollama, o BrainChain aproveita a GPU quando ela é compatível.

### Consumo do plano
- A barra superior mostra quanto do plano de assinatura do Claude e do Codex já foi usado, e cada painel do Claude mostra a velocidade em tokens por segundo.

### Acesso remoto
- Trabalhe nos workspaces de outro computador seu pela própria IDE, como se fossem locais: arquivos, Git, terminais e agentes rodam no computador de origem.
- Toda conexão precisa ser aprovada na hora no computador acessado, e você escolhe quais workspaces ficam visíveis.
- Este recurso ainda está sendo testado entre computadores reais e, por enquanto, é para usar só entre máquinas e pessoas de confiança.

### Idiomas
A interface está disponível em português, inglês, espanhol, francês, alemão, italiano, japonês e chinês.

## Em breve

- **Mais vagas no alpha teste.** As próximas turmas de testadores serão anunciadas aqui.
- **Um visual novo.** Um redesenho completo da interface está em andamento, mantendo todas as funções que já existem.
- **Acesso remoto validado** entre computadores reais, em rede local e pela internet.

O BrainChain está em desenvolvimento ativo: recursos podem mudar, e outros podem aparecer antes da versão pública.

## Como acompanhar

- Clique em **Watch** (no topo desta página) para receber os avisos, inclusive a abertura de novas vagas de teste.
- Clique em **Star** para mostrar seu interesse e ajudar o projeto a ganhar visibilidade.
- Use a aba **[Discussions](../../discussions)** para fazer perguntas, sugerir ideias e conversar com outras pessoas interessadas.

## Perguntas frequentes

**Posso baixar o BrainChain agora?**
Ainda não. O aplicativo está em alpha teste fechado, com um grupo pequeno de testadores. Quando houver novas vagas, o aviso sai aqui.

**Como faço para participar dos testes?**
Acompanhe este repositório (botão **Watch**). As próximas vagas serão anunciadas aqui e nas Discussions.

**Preciso pagar para usar os agentes?**
O BrainChain usa as CLIs oficiais de cada fornecedor com a sua própria conta. O que cada fornecedor cobra continua sendo entre você e ele. Os modelos locais (Ollama, LM Studio, llama.cpp) rodam no seu computador.

**O BrainChain é um modelo de IA?**
Não. Ele é o ambiente onde os agentes trabalham: organiza, conecta e dá controle sobre eles. Os modelos são dos fornecedores que você escolher, ou os que você roda localmente.

**Funciona no Mac ou no Linux?**
Por enquanto o aplicativo é feito e testado para Windows.

**O código do BrainChain é aberto?**
Não. Este repositório é a página pública do projeto e da comunidade; ele não contém o código do aplicativo.

**Como relato um problema ou sugiro uma ideia?**
Abra uma conversa na aba **Discussions**.

---

Os nomes Claude, Codex, Copilot, Cursor, Ollama e os demais citados pertencem aos seus respectivos donos. O BrainChain se integra às ferramentas oficiais de cada um e não tem vínculo com esses fornecedores.

© 2026 BrainChain
