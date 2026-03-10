# Contexto Técnico Inicial - LogiTrack

## Sistemas mapeados
- `route-planner`: calcula rotas e janelas de entrega.
- `fleet-tracker`: recebe telemetria dos veículos.
- `delivery-core`: consolida status das entregas.
- `customer-portal`: consulta de pedidos por clientes.

## Integrações conhecidas
- `fleet-tracker` envia eventos para `delivery-core`.
- `delivery-core` publica status para `customer-portal`.
- `route-planner` consome dados de trânsito de fornecedor externo.

## Lacunas atuais
- Não há diagrama consolidado.
- Responsabilidades entre `delivery-core` e `route-planner` não estão totalmente claras.
- Dependências críticas externas não possuem SLA documentado.
