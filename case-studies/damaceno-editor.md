# Damaceno Editor

**Conceito de ambiente de produção audiovisual programável**  
**Arquitetura proposta:** editor visual · Remotion · FFmpeg · automação com agentes  
**Estado:** desenvolvimento; demonstração de exportação pendente

## Objetivo

A proposta é aproximar a liberdade de composição por código do Remotion e do React da ergonomia de um editor visual. A ideia é permitir que edição visual, composição por código e automações trabalhem sobre a mesma estrutura de projeto, reduzindo a necessidade de alternar continuamente entre várias ferramentas.

## Pilares do conceito

- **Editor visual:** canvas, camadas, timeline, movimentação de elementos, cortes e organização de assets.
- **Engine de composição:** Remotion para composição e animação baseada em React/TypeScript.
- **Processamento de mídia:** FFmpeg para operações de mídia e codificação.
- **Automação assistida:** agentes como ferramenta de apoio para tarefas repetitivas, mantendo controle explícito do projeto.

Esses pilares descrevem a direção de arquitetura documentada; não significam que todas as funções previstas já estejam implementadas.

## Evidências e estado

O lint e o build passaram após uma correção registrada na cópia local. A exportação real de um vídeo ainda não foi validada de ponta a ponta, e o bundle gerado tem aproximadamente 617 kB.

Não há afirmação de que o editor esteja pronto para produção ou substitua editores profissionais.

## Próximos critérios

1. Exportar uma composição de teste completa e verificar áudio, vídeo, duração e resolução.
2. Validar a sincronização entre estado visual, estrutura do projeto e renderização.
3. Definir um formato de projeto estável e testes de regressão para edição/exportação.
4. Revisar tratamento de credenciais e chamadas a serviços de IA antes de qualquer demonstração remota.

## Referências técnicas

- [Remotion](https://www.remotion.dev/docs)
- [FFmpeg](https://ffmpeg.org/documentation.html)
- [React](https://react.dev/)
- [TypeScript](https://www.typescriptlang.org/docs/)
