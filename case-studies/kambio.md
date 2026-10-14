# Kambio

**Plataforma em desenvolvimento para uma comunidade de motoristas em tempo real**  
**Escopo:** aplicativo móvel · API REST · eventos em tempo real  
**Código-fonte:** privado

## Proposta

O Kambio é concebido como uma plataforma que combina aplicativo móvel e backend para interações comunitárias em tempo real. O backend organiza APIs, autenticação e serviços de dados; a camada realtime foi estruturada em torno de Socket.IO, com PostgreSQL e Redis no ambiente local.

## Stack observada no projeto

- Backend em Node.js e Express.
- PostgreSQL e Redis para infraestrutura de dados e serviços auxiliares.
- Socket.IO para comunicação em tempo real.
- Aplicativo móvel e módulos compartilhados no mesmo projeto.

## Evidências de revisão

A cópia privada de staging foi saneada para remover arquivos de ambiente e dados Docker. O Compose exige senha de banco configurada no ambiente e limita as portas do Postgres e Redis ao loopback.

## Bloqueios conhecidos

A aplicação móvel ainda tem inconsistências de dependências e configuração de workspace: a dependência reactNative aparece no lugar de react-native, o lockfile do pacote mobile está vazio e há uma referência de workspace incorreta. Não foram identificados testes automatizados suficientes para confirmar os fluxos de ponta a ponta.

Por isso, este estudo de caso apresenta a arquitetura e o estado técnico, não uma alegação de produto pronto.

## Próximos critérios

1. Corrigir nome e versão das dependências, regenerar lockfile e validar instalação limpa.
2. Corrigir o workspace e padronizar comandos de desenvolvimento.
3. Criar testes de integração de autenticação, API, PostgreSQL, Redis e Socket.IO.
4. Validar o aplicativo móvel em emulador ou dispositivo com dados sintéticos.

## Referências técnicas

- [Express](https://expressjs.com/)
- [PostgreSQL](https://www.postgresql.org/docs/)
- [Redis](https://redis.io/docs/latest/)
- [Socket.IO](https://socket.io/docs/v4/)
- [Node.js](https://nodejs.org/docs/latest/api/)
