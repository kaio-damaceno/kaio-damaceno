# Raspadinha — projeto mantido em equipe

**Aplicação web em manutenção e customização coletiva**  
**Stack observada:** Laravel 10 · PHP · Vue · JavaScript · Vite · Tailwind CSS · MySQL  
**Código-fonte:** privado

## Contexto

O projeto é mantido e customizado por uma equipe. A documentação herdada identifica a base upstream como Viper Pro e menciona modificações em código de terceiros. O escopo deste estudo de caso, portanto, é a manutenção e a preparação técnica da cópia de trabalho, não a reivindicação de autoria integral do produto original.

## Evidências de validação

Na cópia privada de staging:

- 543 arquivos PHP passaram no php -l.
- npm ci e npm run build passaram.
- A preparação para versionamento excluiu arquivos de ambiente, dumps SQL, backups, logs e dependências instaladas.
- Três literais com formato de chave Google encontrados no staging foram substituídos por referências a variáveis de ambiente e verificados novamente.

## Limites, atribuição e segurança

O build frontend ainda aponta quatro caminhos de assets não resolvidos, imports de path/url de Pixi.js externalizados e um bundle JavaScript grande. Os fluxos integrados, pagamento, gateway, carteiras e administração ainda precisam de testes de segurança e funcionamento.

A licença original e as permissões de redistribuição da base upstream não estão confirmadas. Por isso, o código continua privado e não há capturas de telas ou demonstração pública neste portfólio até que a procedência e os direitos sejam esclarecidos.

## Próximos critérios

1. Confirmar o upstream e as licenças dos componentes herdados.
2. Documentar de forma precisa as contribuições da equipe.
3. Resolver assets e imports do build.
4. Preparar ambiente sintético e testar rotas, autorização, pagamentos e integrações de ponta a ponta.

## Referências técnicas

- [Laravel](https://laravel.com/docs)
- [PHP](https://www.php.net/manual/)
- [Vue](https://vuejs.org/guide/)
- [Vite](https://vite.dev/guide/)
- [Tailwind CSS](https://tailwindcss.com/docs)
