# GIRO X — Empréstimo no Cartão

Site institucional e **calculadora interativa** de empréstimo no cartão da GIRO X — *soluções que cabem no seu bolso*.

Página única (HTML/CSS/JS, sem dependências) com:

- **Calculadora** de parcelas em tempo real, com campo de valor (com botões **+ / −**), slider de R$ 400 a R$ 25.000 e seletor de 1x a 12x.
- **Tabela da promoção** com os valores oficiais (R$ 400 a R$ 25.000).
- Botão **Contratar pelo WhatsApp** com a simulação já preenchida.
- Ícones **VISA** e **Mastercard**.

## Cálculo

Fatores extraídos da tabela promocional:

- **6x** → total = valor × 1,147 (acréscimo de 14,7%)
- **12x** → total = valor × 1,167 (acréscimo de 16,7%)

As parcelas intermediárias (1x–5x, 7x–11x) são interpoladas entre esses dois pontos — ajuste em `FATORES` no `index.html` caso as taxas reais sejam outras.

## Rodar localmente

```bash
python3 -m http.server 4173 --directory .
# abra http://localhost:4173
```
