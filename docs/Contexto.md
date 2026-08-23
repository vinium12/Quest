# Contexto do Projeto: Quest
**Documentação Base para Inteligência Artificial e Agentes de Código**

Este documento centraliza as regras de negócio, requisitos, decisões de design e arquitetura pedagógica do projeto **Quest**. Ele deve ser utilizado como contexto absoluto para qualquer IA que for auxiliar no desenvolvimento do código, design ou documentação do sistema.

## 1. Visão Geral do Projeto
O **Quest** é uma plataforma EdTech focada em avaliação formativa contínua e diagnóstico pedagógico em tempo real dentro da sala de aula. O sistema resolve duas grandes dores educacionais: a falta de visibilidade do professor sobre a real compreensão da turma (que leva ao ensino "para a média") e a inibição dos alunos em tirar dúvidas pelo medo da exposição pública.

## 2. Equipe e Responsabilidades
* **Vinicius Fernandes de Lima:** UI/UX Design, Prototipagem, Identidade Visual e Frontend.
* **Jônatas Frinhani de Souza Palmeira:** Backend, Modelagem de Dados e Infraestrutura.
* **Gustavo de Souza Morais:** Backend, Integrações e Infraestrutura.

## 3. Stack Tecnológica
* **Frontend:** React, JavaScript/TypeScript. Interface web leve e responsiva.
* **Backend:** Node.js com framework Express.
* **Banco de Dados:** PostgreSQL (banco relacional).
* **Arquitetura/Acesso:** Aplicação Web acessada via navegador. O acesso dos estudantes às salas virtuais é feito através de um código PIN.

## 4. Funcionalidades Core (MVP)
* **RF01:** O professor cria uma sala de aula virtual.
* **RF02:** O aluno acessa a aula através de um código PIN.
* **RF03:** O professor sincroniza e compartilha seus slides/materiais em tempo real com os alunos.
* **RF04:** O aluno envia dúvidas de forma totalmente anônima durante a explicação.
* **RF05:** O professor recebe e visualiza as dúvidas anônimas em tempo real em seu painel.
* **RF06:** Aplicação de verificações formativas interativas para geração de diagnóstico.
* **RF07:** O painel exibe instantaneamente o "Panorama de Aprendizagem" / "Foto Diagnóstica" para o professor.
* **RF08:** Geração de relatórios analíticos individuais de desempenho pós-aula.

## 5. Engenharia Pedagógica (Mecânica de Avaliação)
* A mecânica exata de diagnóstico está em definição, mas **questões comuns de múltipla escolha (4 alternativas) devem ser expressamente evitadas** para não gerar diagnósticos superficiais.
* O sistema deve explorar alternativas pedagógicas focadas em metodologias ativas e construção de conhecimento, que permitam ao professor visualizar lacunas reais, como: Nuvem de Palavras (Word Cloud), Termômetro de Autoeficácia (escala Likert), "Ponto de Lama" (Muddiest Point) ou respostas curtas (Short Text Stream).

## 6. Identidade Visual e UI/UX (Design System: Cognitive Clarity)
A interface é construída sobre a filosofia "Cognitive Clarity", que utiliza harmonia monocromática para reduzir o ruído visual e promover foco[cite: 1]. A estética une **Minimalismo e Glassmorphism**[cite: 1].
* **Paleta de Cores (Full Purple):** O projeto adota um espectro monocromático baseado em roxo[cite: 1].
  * **Primary:** Violeta vibrante (`#8B5CF6`) - Utilizado para ações de alto destaque, estados ativos e identificação da marca[cite: 1].
  * **Secondary:** Lavanda pastel suave (`#DDD6FE`) - Para fundos de componentes, estados selecionados e botões secundários[cite: 1].
  * **Tertiary:** Tint ultra-claro (`#F5F3FF`) - Para grandes superfícies, fundos de página e containers sutis[cite: 1].
  * **Neutral/Texto:** Carvão escuro com tom índigo (`#1E1B4B`) - Para máximo contraste na tipografia e iconografia sobre fundos claros[cite: 1].
  * *Nota de Design:* Cores funcionais padrão (verde, vermelho, amarelo) devem ser evitadas; feedbacks de erro ou sucesso devem usar variações tonais da paleta roxa ou depender estritamente de iconografia[cite: 1].
* **Tipografia:** A família **Work Sans** é o padrão para todos os níveis, garantindo uma personalidade profissional e versátil[cite: 1]. Headlines usam pesos fortes (600-700) com leve espaçamento negativo, e o corpo de texto (Body) é fixado em 16px para leitura otimizada[cite: 1].
* **Layout e Espaçamento:** O grid fluido baseia-se em múltiplos de 4px, com distanciamentos verticais estritos em múltiplos de 8px[cite: 1]. Componentes tipo Card devem ter padding interno generoso (24px+) para evitar interfaces congestionadas[cite: 1].
* **Formas e Elevação:**
  * Componentes usam cantos arredondados: 8px para inputs/botões pequenos, 16px para cards e 24px para modais grandes[cite: 1]. Botões interativos nunca devem ter cantos retos[cite: 1].
  * Sombras pretas agressivas são proibidas. A profundidade é dada por *Tonal Layering* (sobreposição de contrastes) e sombras extremamente difusas tingidas de roxo (ex: `rgba(139, 92, 246, 0.08)` com blur de 20-40px)[cite: 1].
  * Modais usam *Glassmorphism* com background blur de 12px e bordas brancas semitransparentes de 1px[cite: 1].
* **Logo:** O texto "Quest" utiliza a tipografia sem serifa base, com a letra "Q" estilizada geometricamente no formato de uma lupa, simbolizando a busca contínua por diagnóstico.