# Eu Presidente

**Simulador de carreira política e eleições em ambiente 2.5D**  
**Tecnologias:** Vite · JavaScript · HTML · CSS  
**Estado:** protótipo com sistemas extensos; bloqueado para showcase até corrigir QA de navegação

## Ideia de produto

O jogo combina exploração de ambientes isométricos com progressão política, decisões de campanha e gestão de recursos. A intenção é conectar a movimentação entre espaços, interações com personagens e sistemas eleitorais para que decisões de campanha tenham consequência no estado do jogo.

## Sistemas presentes no projeto

- Ambientes e salas com projeção isométrica e movimentação por tiles.
- Personagens, interações, eventos e agenda.
- Recursos de campanha, apoio segmentado, reputação e caixa.
- Decisões políticas, atividades de campanha e simulação eleitoral.
- Testes separados para renderer, campanha e eleição.

## Evidências e bloqueios

Os testes dedicados de renderer, campanha e eleição passaram na revisão registrada. A suíte E2E mais ampla ainda falha em cenários de navegação: houve casos em que hover/clique e movimento do avatar não chegaram ao tile esperado. Por isso, o jogo não é apresentado como concluído ou pronto para produção.

## Próximos critérios

1. Restaurar a invariância entre posição lógica, renderização, hover, clique, movimento e pathfinding.
2. Repetir toda a suíte E2E em ambientes e salas distintos.
3. Testar a progressão de campanha até vitória/derrota, reinício e persistência.
4. Conferir direitos e procedência dos assets antes de distribuir a demonstração.

Não há código-fonte, saves de usuário ou artefatos brutos de QA publicados aqui.
