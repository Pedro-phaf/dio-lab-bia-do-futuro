

***

# 🎓 Luli: Sua Educadora Financeira Inteligente

Bem-vindo ao repositório da **Luli**, uma assistente virtual proativa focada em educação financeira. Este projeto utiliza Inteligência Artificial Generativa para transformar a interação com dados financeiros, ensinando conceitos complexos de forma didática, personalizada e amigável.

## 🎯 Sobre o Projeto

A Luli atua como uma educadora de bolso. Ela consome os dados mockados do cliente (perfil, transações recentes, histórico de atendimento e portfólio) para criar explicações e exemplos práticos baseados na realidade do usuário. 

**Principais Diretrizes da Luli:**
* **Foco em Educação:** Ensina conceitos e tira dúvidas, mas não recomenda investimentos específicos.
* **Personalização:** Usa o saldo, o perfil e os objetivos do cliente para ilustrar os ensinamentos.
* **Segurança:** Responde exclusivamente sobre finanças pessoais, evitando alucinações.
* **Linguagem Acessível:** Comunica-se de forma simples, direta e interativa.

## 🛠️ Tecnologias Utilizadas

* **Python:** Linguagem base do projeto.
* **Streamlit:** Construção da interface gráfica interativa (Chat).
* **Ollama:** Execução local do modelo de linguagem (LLM `gpt-oss`) garantindo privacidade e rapidez.

## 📂 Estrutura do Repositório

* `src/app.py`: Código-fonte principal com a interface de chat e a integração com a IA via API.
* `data/`: Base de conhecimento (arquivos `.csv` e `.json` com transações, perfil e produtos financeiros).
* `docs/`: Documentação técnica detalhada, englobando arquitetura, testes de prompts, métricas e o roteiro do pitch.

## 🚀 Como Executar Localmente

1. Certifique-se de ter o **Ollama** rodando localmente em sua máquina na porta padrão (`11434`) com o modelo definido:
   ```bash
   ollama run gpt-oss
   ```

2. Instale as dependências do projeto:
   ```bash
   pip install streamlit pandas requests
   ```

3. Inicie a aplicação:
   ```bash
   streamlit run src/app.py
   ```
