# DIO.IA
Repositorio para atividade (Gerado no Claude)

# 🛡️ Miniguia de Estudos: DevSecOps com NotebookLM

## 📝 Contexto e Objetivos
Este repositório foi desenvolvido como parte de um desafio de projeto na **DIO (Digital Innovation One)**. O objetivo principal é aplicar o conceito de **aprendizagem ativa** utilizando o **NotebookLM** (ferramenta de IA do Google) para sintetizar, organizar e dominar conceitos complexos de segurança da informação.

*   **Assunto Escolhido:** DevSecOps (A integração de práticas de segurança no ciclo de vida de desenvolvimento e operações).
*   **Objetivos de Estudo:** 
    *   Compreender como a cultura DevOps evolui para mitigar riscos de segurança sem desacelerar as entregas.
    *   Identificar ferramentas e pontos de automação para análise de vulnerabilidades (SAST, DAST e SCA).
    *   Aprender a criar políticas de segurança como código.

---

## 📚 Curadoria de Fontes
Para alimentar o NotebookLM e garantir respostas tecnicamente precisas e sem alucinações, foram selecionadas as seguintes fontes abertas de alta autoridade:

1.  **OWASP Top 10 CI/CD Security Risks:** Guia oficial sobre as maiores vulnerabilidades em esteiras de implantação automatizadas. [Link para o Projeto OWASP](https://owasp.org/www-project-top-10-cicd-security-risks/)
2.  **CISA (Cybersecurity and Infrastructure Security Agency):** Documentação sobre práticas recomendadas para a segurança da cadeia de suprimentos de software (*Software Supply Chain*). [Link CISA](https://www.cisa.gov/)
3.  **Red Hat Guide - What is DevSecOps?:** Artigo conceitual detalhando a transição cultural de equipes isoladas para a responsabilidade compartilhada. [Link Red Hat](https://www.redhat.com/)

---

## 🧠 Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

Nesta seção, documento os testes de prompts realizados no NotebookLM, os resultados obtidos e como refinei as instruções para superar limitações da IA.

### Teste 1: Prompt Amplo (Abordagem Inicial)
*   **Prompt:** *"Me explica o que é DevSecOps com base nos textos."*
*   **Resultado:** A IA trouxe uma resposta excessivamente genérica, focando apenas no conceito de "cultura" e ignorando a parte técnica de CI/CD que constava nos documentos da OWASP.
*   **Lição aprendida:** Prompts abertos geram respostas superficiais, mesmo com boas fontes.

### Teste 2: Prompt Estruturado (Refinamento)
*   **Prompt:** *"Com base estritamente no documento da OWASP fornecido, liste os 3 principais riscos em esteiras de CI/CD e indique uma ação de mitigação prática para cada um. Formate em uma tabela."*
*   **Resultado:** Excelente. A IA gerou a tabela exata com as citações diretas das fontes, correlacionando o risco com a mitigação recomendada pelas agências de segurança.

> 💡 **Dica de Troubleshooting:** O NotebookLM é excelente para não alucinar, mas ele se limita rigorosamente ao que você envia. Se a resposta parecer incompleta, certifique-se de que o trecho específico do PDF não está em formato de imagem não indexada (sem OCR).

---

## 📖 Miniguia de Estudo (Entrega Final)

### 1. Resumo Estruturado: O Coração do DevSecOps
Diferente do modelo tradicional onde a segurança é uma fase final e isolada (gerando gargalos), o DevSecOps introduz o conceito de **Shift Left** (Mover para a esquerda). Isso significa que a segurança é pensada desde a concepção do código.

*   **Fase de Build:** Análise Estática de Código (SAST) procura falhas no código-fonte antes da compilação.
*   **Fase de Teste:** Análise Dinâmica (DAST) simula ataques no ambiente de testes.
*   **Fase de Deploy:** Verificação de dependências de terceiros (SCA) garante que bibliotecas open-source não possuam vulnerabilidades conhecidas (CVEs).

### 2. Glossário de Conceitos Chave
*   **Shift Left:** Prática de introduzir testes de segurança e validações nas etapas iniciais do desenvolvimento de software.
*   **CI/CD (Continuous Integration / Continuous Deployment):** Automação do processo de integrar código, rodar testes e implantar o software em produção.
*   **SAST (Static Application Security Testing):** Varredura de segurança "caixa-branca", que analisa o código sem executá-lo.
*   **Pipeline:** A esteira automatizada por onde o código passa desde o commit do desenvolvedor até o servidor final.
