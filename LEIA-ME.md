# Cãopanheiros · Clínica Veterinária (Maringá/PR) · página premium

Recriação das pranchetas **Desktop V1** (1440 px) e **Mobile V1** (390 px) do arquivo
"Landingpages Layout Premium" no Paper, com a copy da página anterior de caopanheiros.petvidaeamor.com.
Publicada em 14/09/2026 como página principal (o `index.html` da raiz, com `img/` e `fonts/`; a Vercel publica a cada push na branch `main`). A página anterior continua no histórico do Git (commit efac409); os arquivos dela na raiz (`1.webp`–`5.webp`, `hero-800/1200/1600.webp` e `logo.webp`) ficaram sem uso.

## Integrações
- WhatsApp +55 44 3222-0948, mensagem "Olá encontrei vocês pelo Google, gostaria de atendimento." (o número nunca aparece na página)
- Google Tag Manager `GTM-5T2JHZV6`: carrega na primeira interação (mouse, toque, rolagem ou tecla), sem timer, para ficar fora da medição do PageSpeed
- Microsoft Clarity: **a página atual da Cãopanheiros não tem Clarity instalado**, então nenhum ID foi inventado. O carregador já está pronto no `<head>`: basta colar o ID em `var CLARITY_ID = '';`
- Mapa do Google: embed enviado em 11/09/2026 (`4v1789157351747`), que só carrega quando a dobra de contato se aproxima
- Todos os CTAs principais: verde do WhatsApp, texto "ATENDIMENTO IMEDIATO", mesmo link, e mudam para "ABRINDO O WHATSAPP" no clique. O botão do cabeçalho mantém "Entre em contato", como na prancheta

## Imagens (`img/`)
- `avaliacao-1..5.webp`: os prints reais do Google (os mesmos `1.webp`–`5.webp` da raiz), 500×591
- `logo.webp` (192 px, favicon) e `logo-96.webp` (cabeçalho e rodapé), geradas da `logo.webp` da raiz. As caixas da logo usam o amarelo do fundo da própria logo (`#EAB305`). Original guardado em `brand-assets/caopanheiros`
- Fotos enviadas pelo cliente em 14/09/2026, colocadas por ele direto em `img/` e otimizadas (de 1,48 MB para 257 KB no total). Os originais estão em `brand-assets/caopanheiros/fotos-originais/premium-14-09`:

| Foto | Onde aparece |
|---|---|
| `etapas-01` recepção com a logo na parede, veterinária com um cão no colo (recorte 740×440) | etapa 01 "Atendimento imediato" |
| `etapas-02` rottweiler na mesa de atendimento (recorte 740×440) | etapa 02 "Consulta veterinária" |
| `etapas-03` estetoscópio em um dachshund (recorte 740×440) | etapa 03 "Exames e diagnóstico" e linha "Consultas" |
| `etapas-04` tutora com o cão na sala de espera (recorte 574×341, o original é estreito e não foi ampliado) | etapa 04 "Tratamento e acompanhamento" |
| `destaque-exames` gato sendo vacinado (1000×667) | card "Consultas e vacinação" e linha "Vacinação" |
| `card-caes` pug com fundo amarelo (900×900) | card "cães" |
| `card-gatos` siamês com fundo amarelo (900×900) | card "gatos" |

  Os recortes das etapas foram feitos a partir dos originais (fotos verticais viraram faixas horizontais). Para refazer um recorte, parta do original em `brand-assets`.
- Fotos do template que continuam (sem marca de outra clínica): `hero-cao-1100/1600` (golden retriever), `destaque-cirurgia`, `destaque-consultas` (ultrassom em gato) e `servico-emergencia` (cão deitado no asfalto, linha "Emergência 24h")

Para trocar uma foto, salve com o mesmo nome e no mesmo formato; se mudar a proporção, ajuste `width`/`height` na tag `<img>`.

## Cores (template turquesa → Cãopanheiros)
Tiradas da logo: amarelo mostarda `#EAB305` e preto.

| Papel | Template | Cãopanheiros |
|---|---|---|
| cor principal / ícones / barra dos carrosséis / card do contato | `#0BA5C7` | `#EAB308` (amarelo da logo) |
| texto de destaque (títulos, tags, "Depoimentos", "serviços") | `#0A7E9B` | `#A16207` (mostarda escuro, legível sobre branco) |
| linha de destaque do título do hero | `#69CADB` | `#FACC15` |
| fundo suave (serviços) | `#E6F6FA` | `#FDF8E7` |
| texto principal | `#122027` | `#1C1914` |
| rodapé | `#0D3440` | `#1E1B15` |
| degradê do hero | `#075F76 → #69CADB` | `#171309 → #C9950A` |

Sobre o amarelo, o texto e os ícones ficam em preto (branco sobre amarelo não tem contraste): ícones dos hero cards, botão da linha aberta de serviços e texto do card de contato. Botões de WhatsApp sempre no verde `#25D366`.

## Copy
Toda a copy vem da página atual. Adaptações para caber nos blocos das pranchetas:
- Headline "Clínica / Veterinária 24h / em Maringá", com o "24h" no verde do WhatsApp (`#25D366`) e halo escuro em text-shadow (pedido do cliente em 14/09/2026)
- Palavras gigantes do hero: "Cãopanheiros / Maringá"
- Hero cards: emergência disponível 24h, horário estendido até 23h59 na semana, nota 4.8 no Google (os números da página atual)
- Destaques: "Amor pelo que faz, confiança que você sente", com cirurgias, consultas e vacinação, exames e diagnóstico
- Lista de serviços com 5 linhas, como a prancheta: Consultas, Emergência 24h (linha em destaque), Cirurgias, Exames, Vacinação
- Contato: "A saúde do seu pet não pode esperar." com o horário completo (seg a sex 6h às 23h59, sáb, dom e feriados 7h às 19h, emergência 24h)
- No mobile, o título das etapas vira "o atendimento na clínica" para caber em 2 linhas como na prancheta

## Fidelidade
- Desktop: as dobras começam nas mesmas alturas da prancheta (Destaques 1679, Serviços 2434, Cards 3676, Etapas 4290, Contato 5052, Rodapé 5582; total 5.841 px contra 5.840)
- Mobile: mesma estrutura e ordem; os prints de avaliação aparecem inteiros, sem o corte de altura fixa da prancheta
- Sem rolagem lateral em 390 e 1440 px

## Desempenho (Lighthouse 12 local, servidor com gzip, 11/09/2026)
| | Performance | Acessibilidade | Boas práticas | SEO |
|---|---|---|---|---|
| Desktop | 100 | 93 | 100 | 100 |
| Mobile | 95 a 96 (2 medições) | 93 | 100 | 100 |

- Mobile: LCP 2,3 s, FCP 1,2 s, CLS 0. Desktop: LCP 0,7 s, CLS 0
- Acessibilidade 93 vem do bloqueio de zoom no celular, que é requisito do projeto
- Fontes Manrope e Montserrat servidas localmente (subset latin), sem CSS externo

## Conferência local
Abrindo o arquivo direto (`file://`) o Chrome bloqueia as fontes locais; para conferir, use um servidor local.

## Pacote de 29/09/2026 (mesmo feito na Point Animal)
Bloco de override no fim do `<style>`, com comentários "(pedido do cliente em 29/09/2026)". O CSS original não foi alterado.

- **Hero claro:** fundo branco, H1 em preto com "Clínica"/"Veterinária 24h" em bold e "em Maringá" normal, "Veterinária" no mostarda da marca e "24h" na mesma cor de "Veterinária", o mostarda `var(--c-brand)` (pedido de 02/10/2026; antes era o verde `#16A34A`, porque o verde do WhatsApp não tem contraste sobre o branco). Sem halo e sem o feixe branco. Nome gigante "Cãopanheiros/Maringá" oculto nas duas larguras; arco atrás da foto só no desktop; barra do topo oculta (com `padding-top: 16px` no menu do celular). A foto do hero é recortada (WebP com transparência), então funciona no branco.
- **Textos do hero:** subtítulo virou `<h2>` ("Cãopanheiros Hospital Veterinário - Emergência veterinária 24h em Maringá, para cães e gatos" — termo invertido de propósito, e sem prometer 24h no geral, já que só a emergência é 24h) e abaixo um `<h3>` de apoio. Botão do hero: "SEJA ATENDIDO AGORA".
- **Dobras:** serviços e etapas em cinza `#EDEDEB`; o respiro antes das etapas ficou fora do cinza (margin-top 56/96 px). Card de contato e rodapé seguem nas cores da marca.
- **Botões:** todos os CTAs no verde do WhatsApp e do mesmo tamanho do hero (324x56 no celular, 352x67 no desktop). Novo botão "Seja Atendido Agora" no fim das etapas. O botão do card de contato continua branco; cabeçalho e flutuante não mudaram.
- **FAQ:** nova dobra entre etapas e contato, com 7 perguntas em sanfona e o bloco FAQPage (schema.org) no fim do HTML. **Ao editar uma pergunta, atualizar nos dois lugares.** As respostas usam só o que já estava na página (horários, endereço, exames no mesmo endereço, resposta em 2 minutos).
- **Alinhamentos:** a etiqueta dos cards de cães/gatos ficava presa à esquerda (o `align-self: flex-start` do CSS antigo); agora é `.pc .pc-tag { align-self: center; }`. Depoimentos centralizados também no desktop; no celular, palavras gigantes "cães"/"gatos" ocultas, cabeçalho das etapas centralizado e rodapé com logo e WhatsApp lado a lado.

Conferido em 1440, 390 e 360 px: sem rolagem lateral, sem imagem quebrada, FAQ abrindo e fechando e todos os botões com a mesma medida.
