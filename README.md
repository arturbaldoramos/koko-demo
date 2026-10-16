# koko-demo

Demonstrações de site da Koko. Cada pasta é uma proposta de trabalho, publicada em URL
temporária para o lead ver antes de decidir.

## Regras deste repositório

- Toda página leva `<meta name="robots" content="noindex, nofollow">`. Nenhuma é indexável.
- Nenhuma página é linkada a partir da raiz: o acesso é só por link direto.
- Nenhuma página vai ao ar em domínio do cliente, nem passa por site oficial dele.
- Nenhuma foto, logo ou material do cliente é usado sem autorização.
- Texto de exemplo (sem dado real confirmado) é marcado visualmente na própria página.
- Qualquer pedido de remoção é atendido na hora.

## Conteúdo

| Pasta | Proposta |
|---|---|
| `nutri-blumenau/` | Página de Nível 1 — nutricionista, Blumenau/SC |

## Sem `robots.txt` de bloqueio — de propósito

Este é um GitHub Pages de projeto, servido em um subcaminho. Um `robots.txt` na raiz do
repositório é servido em `/koko-demo/robots.txt`, e buscadores só leem `robots.txt` na raiz
do host — então ele seria ignorado. Além disso, `Disallow` impediria o rastreador de ler a
própria meta tag `noindex`, o que é pior: a URL poderia acabar indexada sem conteúdo.
O controle correto aqui é a meta tag `noindex`, que está em todas as páginas.
