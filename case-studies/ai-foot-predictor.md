# AI Foot Predictor

**Experimento de engenharia de dados e análise de futebol**  
**Stack planejada:** Python · FastAPI · PostgreSQL · Redis · React · TypeScript · Vite  
**Código-fonte:** privado

## Objetivo

Explorar um pipeline para coleta e preparação de dados de futebol, engenharia de atributos, experimentação com modelos e disponibilização de resultados por API e interface web.

## Componentes do projeto

- Coleta e preparação de dados.
- Rotinas de engenharia de features e experimentação com modelos estatísticos e de machine learning.
- API Python e infraestrutura local para dados.
- Frontend React/TypeScript separado da API.

As bibliotecas listadas no projeto indicam a direção técnica; não significam que cada modelo ou integração tenha sido validado de ponta a ponta.

## Evidências de validação

Na revisão privada registrada:

- A compilação sintática dos módulos Python selecionados passou.
- A configuração do Docker Compose passou na validação de sintaxe/configuração.
- O build do frontend Vite passou.

## Limites e segurança

Nenhuma métrica de desempenho preditivo foi medida de forma reproduzível. As metas de acurácia que apareciam em documentação herdada não são resultados e não são apresentadas como tal.

Há também trabalho de segurança pendente: o frontend tem uma configuração que pode incluir chave de API no bundle do navegador, e a política CORS da API precisa ser revisada. Por esse motivo, o projeto não é descrito como serviço de apostas, recomendação financeira ou sistema pronto para produção.

## Próximos critérios

1. Mover chamadas que exijam segredo para o backend e revisar CORS.
2. Documentar fonte e licença de cada dataset.
3. Definir validação temporal, baseline e métricas reproduzíveis por temporada.
4. Executar avaliação fora da amostra e documentar limitações e riscos de vazamento de dados.
5. Validar API, banco e frontend integrados com dados sintéticos.

## Referências técnicas

- [Python](https://docs.python.org/3/)
- [FastAPI](https://fastapi.tiangolo.com/)
- [scikit-learn](https://scikit-learn.org/stable/)
- [React](https://react.dev/)
- [Vite](https://vite.dev/guide/)
