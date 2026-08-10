🤖 Agente de Atendimento Inteligente com IA - Challenge Alura
Este repositório contém a implementação de um Agente de Atendimento ao Cliente automatizado, desenvolvido como parte do Challenge Alura Agente.
O projeto utiliza o n8n para orquestração de fluxos e integração com modelos de Inteligência Artificial da Google (Gemini).
🛠️ Arquitetura do Projeto
O fluxo de trabalho (workflow) foi estruturado no n8n utilizando os seguintes componentes principais:
 * Trigger de Entrada:
   * Nó do tipo Chat/Webhook (When chat message received) para capturar as interações do usuário em linguagem natural.
 * Modelo de Linguagem (LLM):
   * Google Gemini Chat Model integrado ao nó AI Agent para processamento de linguagem natural e geração de respostas contextualizadas.
 * Base de Conhecimento:
   * Instruções de sistema e regras de negócio da loja (Política de entregas, trocas, devoluções e pagamento) configuradas diretamente no agente de IA.
   * Integração com nó de busca vetorial (Simple Vector Store) e suporte a embeddings (Embeddings Google Gemini) para consulta documental.
📋 Funcionalidades
 * Resposta automatizada a dúvidas frequentes sobre:
   * Formas de pagamento e descontos (ex: PIX e parcelamento).
   * Prazos e políticas de frete grátis.
   * Regras para trocas e devoluções.
 * Manutenção do contexto da conversa durante o atendimento.
 * Respostas restritas estritamente à base de conhecimento da loja.
🚀 Como Importar e Executar no n8n
 * Faça o download do arquivo Meu fluxo de trabalho.json presente neste repositório.
 * Acesse a sua instância do n8n.
 * No painel principal, selecione a opção Import from File e envie o arquivo .json.
 * Configure as suas chaves de API para o Google Gemini nos nós de credenciais.
 * Ative o workflow e inicie o atendimento pelo Chat.
🛠️ Tecnologias Utilizadas
 * n8n (Automação e Orquestração de Fluxos)
 * Google Gemini AI (LLM e Embeddings)
 * JSON (Exportação e Importação de Arquiteturas)
