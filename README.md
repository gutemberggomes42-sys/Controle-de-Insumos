# CampoFlux — gestão de insumos

Sistema local para cadastro de insumos, apontamento diário de aplicações e entradas, ordens de serviço, saldos, alertas e exportação CSV.

## Abrir

Abra `index.html` em um navegador moderno. Não requer instalação nem servidor. Os registros criados ficam no armazenamento local do navegador usado; faça exportações CSV periódicas como cópia de segurança.

## Primeiro uso

1. Acesse **Estoque de insumos** e edite cada item para informar o saldo físico conferido e, se desejar, o estoque mínimo.
2. Use **Lançamento diário → Novo lançamento** para registrar uma aplicação, entrada ou devolução.
3. Consulte o painel e os relatórios; use **Exportar CSV** para baixar movimentações.

O saldo só é calculado para produtos cujo saldo inicial foi informado. Aplicações e devoluções diminuem o saldo; entradas aumentam. O sistema impede aplicação acima do saldo disponível quando este estiver informado.

## Dados de referência

O sistema inclui produtos, fazendas, frentes, ordens de serviço e linhas de consumo reconhecidas em `DOC-20260406-WA0089.xlsx`. As linhas importadas aparecem como **Histórico importado** e não alteram saldos. A planilha mistura unidades e grafias, preservadas com indicação de aba de origem. Datas e áreas devem ser confirmadas antes de uso em fechamento. Anotações manuscritas da foto não foram inseridas como fatos estruturados.

Dados do sistema ficam no `localStorage` do navegador e não são sincronizados entre dispositivos. Para começar de novo, limpe os dados do site no navegador; essa operação remove os registros locais.
