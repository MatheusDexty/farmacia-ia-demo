# FarmacIA - Demo

Mockup navegável da plataforma de triagem farmacêutica com IA.

🔗 **Ver demo:** https://matheusdexty.github.io/farmacia-ia-demo/

## Sobre

Repositório público apenas com o mockup demonstrativo. O produto, a documentação
completa e o código de produção ficam em repositório privado.

A demo cobre 5 telas:
1. Boas-vindas e consentimento LGPD
2. Anamnese conversacional (guiada por um motor de protocolos, com explicação do porquê de cada pergunta)
3. Ficha gerada com sugestão preliminar de princípio ativo
4. Cenário de red flag (encaminhamento médico)
5. Painel do farmacêutico com fila de casos e tomada de decisão

## O que a plataforma faz (motor de protocolos)

Deixou de ser um chatbot de poucas categorias e virou um **motor de protocolos
clínicos**: cada sintoma é um protocolo com perguntas próprias, red flags e uma
escada terapêutica.

- **Muitos protocolos** - dor de cabeça, febre, gripe, dor de garganta, tosse,
  azia, náusea, diarreia, constipação, gases, cólica, dor muscular, rinite, alergia
- **Anamnese dinâmica** - as próximas perguntas se adaptam às respostas
- **Explicação das perguntas** - a IA diz por que está perguntando (mais confiança)
- **Escalonamento terapêutico** - 1ª linha, 2ª linha, 3ª linha; se não melhorar,
  sobe o degrau, depois farmacêutico, depois médico
- **Red flags determinísticas** - regras (não o LLM), com citação de fonte oficial

## Princípios do produto

- Farmacêutico no loop sempre - a IA não decide sozinha
- Red flags determinísticas (não dependem do LLM)
- A IA pode dizer "não sei"
- Auditabilidade total
- Privacidade primeiro (LGPD Art. 11)

## Stack do mockup

HTML + Tailwind CSS via CDN. Single-page, sem build, sem dependências. Abre em
qualquer navegador moderno.

---

*Mockup demonstrativo - não é o produto final.*
