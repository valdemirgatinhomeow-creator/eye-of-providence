---
name: eye-of-providence
description: "Eye of Providence", o olho que tudo vê. Varredura completa do projeto atual: entende o conceito, ABRE e USA o app/site/programa de verdade (clica em todos os botões e funções), caça bugs, erros, lentidão e melhorias, e corrige tudo como uma "versão 2.0" sem renomear nada. Use quando o usuário disser "usa a Eye of Providence", "dá uma olhada geral", "caça bugs", "revisa tudo".
---

# Eye of Providence: o olho que tudo vê

## Regra de ouro
**Teste de verdade.** "Rodei e não deu erro" NÃO vale. Só conta como testado o que foi aberto e usado como o usuário usaria: site no navegador, app/programa rodando, arquivo aberto. Se não deu para abrir, diga isso claramente; nunca finja.

## Regra dos nomes
Melhorar como se fosse uma versão 2.0, mas **NUNCA** renomear o projeto, arquivos, pastas, funções ou telas para "v2", "2.0", "novo", "final" etc. Os nomes continuam os mesmos; só a qualidade sobe.

## Passo a passo
1. **Entender:** leia o README, as notas do projeto (se houver) e a estrutura. Resuma em 3 linhas o que é o projeto, para quem ele serve e como funciona.
2. **Rodar:** descubra como o projeto inicia (package.json, launch.json, scripts) e abra-o:
   - Site/web app: servidor local + navegador.
   - App desktop/Electron/programa: rode o executável e use computer-use/screenshot.
   - Script/CLI: execute com entradas reais, inclusive entradas erradas.
3. **Usar tudo:** clique em TODO botão, link, menu, formulário e atalho. Teste o caminho feliz, entradas vazias ou inválidas, voltar, recarregar, tela de celular (375px) e tema escuro. Leia o console e as requisições de rede de cada tela.
4. **Caçar:**
   - Bugs e erros (console, logs, crashes, telas quebradas).
   - Lentidão: tempo de carregamento, travadas, delay ao clicar, arquivos pesados, chamadas repetidas.
   - Código: duplicado, morto, frágil, sem tratamento de erro, inseguro (chaves expostas).
   - Experiência: textos confusos, falta de feedback, acessibilidade.
5. **Listar** os achados por gravidade (crítico, importante, melhoria) antes de mexer. Para mudanças grandes de conceito ou de visual, peça o ok do usuário.
6. **Corrigir:** comece pelos críticos. Depois de cada correção, **abra e teste de novo de verdade** a parte que mudou e o que estiver ao redor dela.
7. **Provar:** entregue o que foi testado (com print ou medição quando fizer sentido), o que foi corrigido, o que ficou pendente e o porquê.
8. **Registrar:** faça o commit por etapa e anote o resultado nas notas do projeto.

## Checklist extra (aplicar o que couber no projeto)
1. Medir o tempo de carregamento antes e depois de cada correção e mostrar a diferença.
2. Tirar prints antes e depois das telas que mudaram.
3. Rodar Lighthouse (desempenho, acessibilidade, SEO) em sites.
4. Procurar chaves de API e senhas no código e no histórico do git.
5. Checar dependências desatualizadas ou vulneráveis (`npm outdated`, `npm audit`).
6. Achar arquivos, funções e imagens que não são usados.
7. Comprimir imagens e vídeos pesados.
8. Testar em celular (375px), tablet (768px) e desktop.
9. Testar com internet lenta (simular 3G).
10. Testar sem internet: o projeto precisa mostrar um erro amigável.
11. Achar links quebrados.
12. Revisar textos com erro de português ou confusos.
13. Checar contraste e navegação só pelo teclado.
14. Ver vazamento de memória em uso longo (apps que ficam horas abertos).
15. Modo "só olhar": se o usuário pedir, só listar, sem mexer em nada.
16. Dar uma nota de 0 a 10 por área (bugs, velocidade, código, visual, segurança).
17. Comparar com a varredura anterior (salva nas notas do projeto) e mostrar o que melhorou ou piorou.
18. Criar testes automáticos para os bugs encontrados, para que não voltem.
19. Sugerir funções novas que combinem com o conceito do projeto (sem implementar sem ok).
20. Oferecer uma varredura automática semanal (tarefa agendada), só com o ok do usuário.

## Economia
Prefira ler o texto da página a tirar screenshots, filtre os logs e não releia arquivos à toa.
