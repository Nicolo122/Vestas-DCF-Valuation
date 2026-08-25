# Vestas Wind Systems A/S — DCF Valuation and Investment Memo

**HOLD · DKK 176 implied vs DKK 205 market · Enterprise value EUR 22.0bn · WACC 9.3% · August 2026**

A discounted cash flow valuation of Vestas Wind Systems A/S (VWS DC), built from the
company's 2023, 2024 and 2025 annual reports. This was my first full valuation project.
The method is deliberately simple, and the section at the bottom says where that
simplicity binds.

---

## Valuation summary  (v2, August 2026)

| | EUR m |
|---|---:|
| Present value of explicit free cash flow (2026E–2030E) | 6,078 |
| Present value of terminal value (Gordon, g = 2.0%) | 15,903 |
| **Enterprise value** | **21,981** |
| (+) Net cash | 1,174 |
| **Equity value** | **23,155** |

| | |
|---|---:|
| Implied value per share — Gordon growth | DKK 175.8 |
| Implied value per share — exit EV/EBITDA (10.0x) | DKK 230.8 |
| Current share price | DKK 204.5 |
| Upside / (downside), Gordon growth | (14)% |
| Terminal value as % of enterprise value | 72.3% |
| Reverse DCF — perpetuity growth the market is pricing | 3.3% |
| **Recommendation** | **HOLD** |

Rule stated in advance: above +15% BUY, below −15% SELL, otherwise HOLD.

Unlevered free cash flow over the explicit period, discounted at a 9.3% WACC on a
mid-year convention:

| EUR m | 2026E | 2027E | 2028E | 2029E | 2030E |
|---|---:|---:|---:|---:|---:|
| Unlevered free cash flow | 1,293 | 1,362 | 1,547 | 1,669 | 1,766 |

The two terminal value methods disagree by DKK 55 per share, which is the honest width
of this valuation. Gordon growth implies a 6.9x exit EV/EBITDA; the 10.0x exit multiple
implies 4.2% perpetual growth, above nominal GDP. The truth sits between them, which is
why the recommendation is HOLD and not a target price carried to one decimal.

## The business

Vestas runs two segments. **Power Solutions** — turbine design, manufacturing,
installation and project development — generated EUR 15.1bn in 2025, roughly 80% of an
EUR 18.8bn top line. **Service** — operation and maintenance, spare parts and digital
optimisation — generated EUR 3.77bn on contracts running ten to twenty-five years.

The hybrid is the whole point: the project business is cyclical and priced against
aggressive Chinese competition, while the service book is recurring, high-margin and
gives the cash flows visibility that a pure OEM would not have. Group EBIT was
EUR 1.015bn in 2025.

## What the valuation actually says

At 72.3% of enterprise value, the terminal value still carries most of the answer — the
number is a statement about the 2030s, not about Vestas today. Extending the horizon from
four years to five brought that down from over 85%, which is progress rather than a cure.

The cross-check that matters is the reverse DCF: at DKK 204.5 the market is pricing 3.3%
of perpetual growth, against a 2.0% base case. That gap is the whole disagreement, and it
is small enough that the honest answer is HOLD.

## Files

| File | What it is |
|---|---|
| `Vestas_DCF_Model_v1.xlsx` | The original April 2026 model. Five tabs. This is what the memo documents. |
| `Vestas_DCF_Model_v2.xlsx` | The August 2026 rebuild. Twelve tabs. See below. |
| `Vestas_Investment_Memo.pdf` | Sixteen-section write-up: business model, value drivers, cost structure, competitive landscape, valuation, risks, thesis |

Both versions are kept deliberately. The distance between them is the point of this
repository.

## Method notes

- Five-year explicit forecast (2026E–2030E), mid-year discounting, two terminal value
  methods: Gordon growth at g = 2.0% and an exit EV/EBITDA of 10.0x.
- WACC 9.3%, built up rather than assumed: risk-free 3.26% (German 10Y Bund, 20-Aug-2026;
  Denmark is AAA and DKK is pegged to EUR under ERM II), ERP 5.0%, levered beta 1.35,
  after-tax cost of debt 3.2%, equity weight 89.1%.
- 2026E revenue of EUR 21.0bn and a 7.0% EBIT margin both sit inside company guidance.
- Vestas is **net cash** of EUR 1,174m, so it is added to enterprise value, not subtracted.
- Built from the FY2023, FY2024 and FY2025 annual reports. The reports are not
  redistributed here — references are in the memo.

## Version note

**v1 — April 2026.** Five tabs, four-year forecast, single terminal value method,
enterprise value as the final output. The memo documents this version.

**v2 — August 2026.** Rebuilt after finishing a much larger valuation of Novo Nordisk,
which made clear what v1 was missing. v2 adds a
five-year forecast to 2030, a second terminal value method (exit EV/EBITDA), a full
enterprise-value-to-equity bridge with an implied share price in DKK, a CAPM build-up
with dated and sourced inputs, trading comparables, four sensitivity grids, three live
scenarios, a football field chart, a reverse DCF, and twelve integrity checks.

## What I would do differently, and did

Written after the Novo Nordisk project. These are the three things v1 got wrong:

1. **The horizon was too short.** A four-year forecast for a business whose value is a
   bet on the 2030s pushes the entire argument into the terminal value. The explicit
   period should be long enough to contain the thing being argued about.
2. **It stopped at enterprise value.** No per-share number, no comparison to the market
   price, therefore no recommendation. A valuation that does not commit to a view is an
   exercise, not an analysis.
3. **There was no cross-check.** One method, with 85% of the value resting on two
   assumptions, needs triangulation — comparables, an exit multiple, and a reverse DCF
   asking what the market would have to believe.

And one outright error, which is the reason this repository keeps v1 rather than quietly
replacing it: **v1 treated Vestas's EUR 1,174m of net cash as net debt and subtracted it.**
Getting that sign wrong moves equity value by twice the amount. v1 also hardcoded an 8.0%
WACC with no build-up behind it, which is too low against a 3.26% risk-free rate — the
corrected build-up gives 9.3%. Between the sign, the discount rate and the extra forecast
year, v1's EUR 13.9bn equity value becomes EUR 23.2bn.

## Disclaimer

Personal academic exercise, prepared for educational purposes only. Not investment
advice and not a recommendation to buy or sell any security. Based solely on publicly
available information.
