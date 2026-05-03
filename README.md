# Termos de Serviço e Política de Privacidade da Nyra

Última atualização: 3 de Maio de 2026

Bem-vindo(a) à Nyra. Ao interagir com este bot no Discord, concordas com os termos estabelecidos abaixo. Lê-os com atenção. Este não é o típico "bot simpático de IA". A Nyra foi criada por Nakamura para ser irreverente, pragmática, sem filtros e direta.

---

## 1. Natureza do Serviço e Conteúdo

1. **Sem Filtros ou Censura:**
   A Nyra foi desenvolvida intencionalmente sem restrições comportamentais artificiais que ditam a habitual "polidez" ou "moderação" comercial de IA. A Nyra pode (e vai) usar sarcasmo, humor ácido, calão (palavrões), e expressar "opiniões" de forma agressiva. Ao usá-la, assumes total responsabilidade por lidares com este tipo de linguagem. Não toleras sarcasmo? Não a invoques.

2. **Isenção de Responsabilidade sobre Output (Geração de Textos e Imagens):**
   Tudo o que a Nyra diz ou cria (texto, áudio, código, imagens através das APIs acopladas) é gerado por algoritmos generativos avançados baseados no LLM Gemini, OpenRouter, entre outros. O criador (Nakamura) não partilha as "opiniões" da IA nem se responsabiliza por conselhos técnicos, morais, legais ou médicos fornecidos pelo bot.

## 2. Coleta e Privacidade de Dados (Sistema de Memória RAG)

A Nyra possui uma arquitetura de "Memória de Longo Prazo" (RAG). Entende o que isso implica para os teus dados:

1. **O que é guardado:**
   A Nyra tem a capacidade de reter informações passadas na sua base de dados (SQLite), se for relevante, ou se lhe pedires especificamente usando o seu sistema de memórias.
2. **Escopo de Memórias (Isolamento):**
   Toda a memória obedece a um contexto restrito:
   - **Privadas (Scope: user):** Memórias que o bot guarda sobre ti ficam atreladas ao teu `user_id` e ao `guild_id` em que foram invocadas. Nenhum outro utilizador num servidor pode acessar às tuas informações pessoais, e as tuas memórias nunca "vazam" para outros servidores ou DMs.
   - **Gerais (Scope: guild):** Se a memória for classificada como regras do servidor ou informação de comunidade, todos os presentes nesse servidor podem beneficiar dessa memória.
3. **Logs e Segurança:**
   Os logs técnicos efetuados pelo bot estão purificados e ofuscados. O sistema regista apenas IDs (como número de quem guardou/eliminou algo) e contagens operacionais, não havendo extração do texto íntimo/privado da tua memória para os ficheiros de texto visíveis ao administrador do sistema.
4. **O Direito ao Esquecimento:**
   Os teus dados pertencem-te. Foram-te providenciados comandos operacionais abertos onde podes visualizar e solicitar a eliminação dos teus dados:
   - `/rag_memory_list`: Para veres as tuas memórias.
   - `/rag_memory_delete <id>`: Para removeres uma memória em específico.
   - `/rag_forget_me confirm:true`: Para destruíres permanentemente todas as tuas memórias associadas àquele servidor ou canal de DM.

## 3. Limitações de Uso Diário e Custos

1. **Créditos e Limites Pessoais:**
   Como as chamadas de Inteligência Artificial dependem de fundos privados em APIs comerciais alocados pelo seu criador, **os utilizadores estão sujeitos a um limite diário de operações** (ex: quantidade de mensagens com raciocínio AI, limite de geração de imagens).
2. **Fallback para Infraestrutura Grátis:**
   Quando atinges o teu limite pessoal diário financiado, a Nyra transitará o teu uso para um ecossistema gratuito (através da OpenRouter). Nestes casos, a qualidade das respostas ou raciocínio pode variar. Não nos responsabilizamos por perdas de precisão nestes períodos ou timeouts de APIs de terceiros.
3. **Renovação:**
   Estes limites renovam-se automaticamente de acordo com o intervalo horário programado internamente (tipicamente em rotação de aproximadamente cada 24 horas).

## 4. Moderação Automática (Automod) e Gestão no Servidor

1. A Nyra incorpora ferramentas clássicas de administração e automod (contagem de convites, palavras-chave de spam `discord.gg`, menções abusivas). 
2. Caso o automod detete abuso, a Nyra possui autoridade técnica para atribuir timeout, silenciar ou expelir (ban/kick) os responsáveis do canal do servidor (desde que ativado pelo Administrador local do servidor onde ela está presente através do `/config`). O uso do bot num servidor infere a aceitação desta delegação de moderação.

## 5. Aceitação

O uso de qualquer Slash Command (ex: `/mensagem`, `/criar_imagem`, `/dm`), o "taggar" ou mencionar a Nyra, ou dar resposta ativa e consciente nos minijogos propostos, consubstancia a aceitação plena e irrevogável destes termos. 

Se não concordares, podes simplesmente remover a Nyra do teu servidor ou não a mencionar/invocar nos canais disponíveis.

---
*© 2026 Desenvolvido por Nakamura.*
