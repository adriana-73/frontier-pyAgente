#  🐍 Python Mentor: Assistente de Aprendizado e Otimização


Assistente de IA desenvolvido no Azure Foundry Link https://adrianacelestrina-4807-resource.services.ai.azure.com/api/projects/adrianacelestrina-4807com o modelo gpt-4o-mini, especializado em ensinar, otimizar e debugar código Python. Nosso objetivo é transformar iniciantes em experts, fornecendo suporte estruturado e focado nas melhores práticas da linguagem, com conceitos (ELI5)



## 🎯 Objetivo e Capacidades e ação funcional tool call

O Mentor Python atua como um recurso de aprendizado e referência rápida, com foco nas seguintes áreas:

| Categoria | Descrição |
| Aprendizado | Explica conceitos complexos de Python, utilizando a técnica "Explain Like I'm 5 (ELI5)" para clareza máxima. |  
| Otimização | Sugere melhorias de performance e refatoração de código. |  
| Frameworks | Possui conhecimento detalhado em bibliotecas essenciais como Django, Pandas, NumPy, FastAPI e TensorFlow. |
| Ação Funcional (Tool).ferramenta de Pesquisa do Bing (Tool Call) para realizar buscas de informações em tempo real.|
| Debugging | Ajuda a depurar trechos de código e sugere correções funcionais. |
|Restrição Principal: O assistente somente responderá a dúvidas relacionadas à linguagem Python|



## Fluxo de Execução e Prova da Ação Funcional
O processo de execução do Agente Python Mentor é iniciado quando uma informação atualizada ou externa é solicitada, comprovando o uso da nossa Ação Funcional (Tool Call):

1. Entrada do Usuário (Prompt): O usuário insere uma pergunta que exige dados recentes ou documentação externa (ex.: "Quais são as novidades de sintaxe na última versão do Python?"). ![pergunta e resposta do agente](assets/TOOL.png)  Análise e Decisão (Tool Call): O modelo de linguagem (GPT-4o-mini) analisa a pergunta e, seguindo as instruções do sistema, determina que a informação deve ser buscada na web para garantir a precisão.
  
2. Execução da Ação Funcional: O agente invoca a ferramenta Pesquisa do Bing, passando a consulta (query) relevante para a busca. Este é o ponto que comprova a Ação Funcional. (Este momento é visível no log de thread no print ![pergunta e resposta do agente](assets/capt-voz.png).
   
3. Processamento e Geração: A ferramenta do Bing retorna o resultado da busca, e o agente utiliza essa informação para construir uma resposta completa e estruturada, seguindo o padrão de ensino (ELI5).![pergunta e resposta do agente](assets/PR-05.png)
   
4. Saída Final: A resposta (contendo a informação atualizada) é entregue ao usuário. ![pergunta e resposta do agente](assets/inicio01.png)


---

## 📝 Estrutura de Resposta (Compromisso com a Qualidade)

Toda interação segue um formato rigoroso (definido no Prompt do Sistema) para garantir o aprendizado: Explicação detalhada e Exemplo de Código funcional, além de referências à documentação oficial.

Exemplo de Interação:

Pergunta do Usuário:
> "O que são listas em Python e como posso usá-las?"
![pergunta e resposta do agente](assets/perg-03.png)

Resposta do Assistente (Simulação do  input e Output):
![pergunta e resposta do agente](assets/fluxo.png)




| Componente | Conteúdo Gerado |

| Explicação | Em Python, uma lista é uma estrutura de dados que pode armazenar valores em uma sequência ordenada. Elas são mutáveis, ou seja, podem ser modificadas após serem criadas. Você pode criar uma lista usando colchetes [], adicionar elementos com .append() e acessar valores usando índices. |
| Exemplo de Código | python # Criação de uma lista: nomes = ["Alice", "Bob", "Charlie"] # Adicionando um elemento: nomes.append("David") # Acessando um elemento: print(nomes[0]) # Saída: Alice  |

-Esta ação comprova a funcionalidade do agente a ![Pergunta e resposta](assets/04-resp.png)

| Referências | A documentação oficial do Python é recomendada: 
[https://docs.python.org/3/tutorial/datastructures.html](https://docs.python.org/3/tutorial/datastructures.html) |
