# Mega Prompt — ConexãoCurrículos

Este documento apresenta o prompt original utilizado para orientar a criação do MVP ConexãoCurrículos na plataforma Lovable.

O texto foi preservado conforme a especificação utilizada no desenvolvimento. As alterações solicitadas posteriormente estão documentadas separadamente no README.md.

---

# CONEXÃOCURRÍCULOS — MVP

Crie uma aplicação web funcional chamada **ConexãoCurrículos**, que compara um currículo com uma descrição de vaga e gera uma versão otimizada para sistemas ATS (Applicant Tracking Systems).

## OBJETIVO

O usuário deverá conseguir:

1. Colar a descrição de uma vaga.
2. Colar seu currículo.
3. Clicar em analisar.
4. Visualizar o percentual de compatibilidade.
5. Consultar palavras-chave encontradas e ausentes.
6. Visualizar pontos fortes e recomendações.
7. Gerar uma versão ATS friendly do currículo.
8. Editar o resultado e baixar em PDF.

## REGRA FUNDAMENTAL

A aplicação melhora a apresentação das experiências e qualificações do candidato, mas nunca inventa experiências, competências, formações, certificações, empresas ou resultados profissionais.

Exibir essa regra claramente na interface.

## DESIGN SYSTEM

Utilize React, TypeScript, Tailwind CSS e shadcn/ui.

Identidade visual:
- Azul principal: #2563EB.
- Azul-marinho: #14213D.
- Fundo: #F8FAFC.
- Branco: #FFFFFF.
- Verde: #16A34A.
- Amarelo: #F59E0B.
- Vermelho: #DC2626.
- Tipografia Inter.
- Ícones Lucide.

Criar uma interface minimalista, moderna, profissional e responsiva.

Utilizar cards, botões, badges, textareas, barras de progresso e componentes shadcn/ui.

## TELA PRINCIPAL

Cabeçalho com o logotipo e nome ConexãoCurrículos.

Título:

**Seu currículo combina com a vaga? Descubra antes de enviar.**

Subtítulo:

Compare suas qualificações com os requisitos da oportunidade e descubra como melhorar seu currículo para sistemas ATS.

Criar dois campos de texto amplos:

### DESCRIÇÃO DA VAGA

Placeholder: Cole aqui a descrição completa da oportunidade.

### MEU CURRÍCULO

Placeholder: Cole aqui seu currículo completo.

Botão principal: **Analisar compatibilidade**

Validar os campos antes de iniciar a análise.

Não criar login, cadastro, dashboard, histórico, upload de arquivos ou banco de dados.

## ANÁLISE INTELIGENTE

Utilizar uma integração real com inteligência artificial, por meio de backend seguro.

A análise deverá:

1. Identificar os requisitos da vaga.
2. Identificar as qualificações e experiências do currículo.
3. Comparar as competências.
4. Identificar palavras-chave encontradas.
5. Identificar palavras-chave relacionadas.
6. Identificar palavras-chave ausentes.
7. Identificar pontos fortes.
8. Gerar recomendações de melhoria.

Calcular um índice de compatibilidade de 0 a 100, baseado na correspondência entre os requisitos da vaga e as evidências presentes no currículo.

A pontuação é uma estimativa da plataforma, não uma pontuação oficial de sistemas ATS ou uma garantia de contratação.

Não utilizar pontuações aleatórias ou resultados fictícios.

## TELA DE RESULTADOS

Apresentar:

- Percentual de compatibilidade em destaque.
- Quantidade de requisitos encontrados.
- Quantidade de requisitos relacionados.
- Quantidade de requisitos ausentes.
- Lista de palavras-chave encontradas.
- Lista de palavras-chave ausentes.
- Pontos fortes.
- Recomendações personalizadas.

Utilizar cores para facilitar a interpretação:

- Verde para correspondências.
- Amarelo para correspondências parciais.
- Vermelho para requisitos sem evidência.

Adicionar o botão **Gerar currículo otimizado**.

## CURRÍCULO OTIMIZADO

Utilizar IA para reescrever e reorganizar o currículo com base na vaga.

Preservar rigorosamente as informações originais.

Não inventar dados.

Priorizar:
- Resumo profissional.
- Competências.
- Experiências profissionais.
- Formação acadêmica.
- Cursos e certificações.
- Idiomas, quando informados.

Utilizar títulos convencionais, estrutura de uma coluna, linguagem profissional e formatação simples compatível com sistemas ATS.

Apresentar o resultado em um editor de texto funcional para revisão.

Adicionar:
- Botão Copiar currículo.
- Botão Baixar PDF.
- Botão Nova análise.

O PDF deve utilizar papel A4, fonte legível e margens adequadas, preservando o conteúdo editado.

## REQUISITOS TÉCNICOS

- Implementar a análise real com IA.
- Utilizar backend seguro para a chave da API.
- Não expor credenciais no frontend.
- Tratar erros e campos vazios.
- Apresentar carregamento durante a análise.
- Não simular resultados.
- Não criar funcionalidades que não foram solicitadas.

Se a integração com IA depender de uma chave externa, informar a configuração necessária em vez de apresentar resultados falsos.

## RESULTADO ESPERADO

Uma aplicação simples, funcional, responsiva e publicável, que execute o fluxo completo:

**Vaga + Currículo → Análise → Match → Palavras-chave → Recomendações → Currículo otimizado → PDF.**

Priorize o funcionamento desse fluxo acima de qualquer funcionalidade complementar.
