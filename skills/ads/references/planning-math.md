# Paid-media arithmetic

Use consistent windows, currency and attribution definitions. Show each input and unit. These formulas support planning, not a guarantee of results. Check arithmetic using an available permitted deterministic calculator when possible; report whether that check actually ran.

| Metric | Formula | Caveat |
| --- | --- | --- |
| CTR | clicks / impressions | Undefined when impressions are zero/missing |
| Click-to-conversion rate | qualified conversions / clicks | Use one explicit conversion definition |
| CPA | ad spend / qualified conversions | Undefined when no conversions; report spend and zero conversions separately |
| CPC | ad spend / clicks | Undefined when no clicks |
| ROAS | attributed revenue / ad spend | Revenue return is not contribution profit |
| Contribution per first order | revenue − variable product/service/fulfillment/payment costs | Must use supplied cost assumptions; exclude fixed costs only explicitly |
| First-order break-even CPA | first-order contribution per acquired customer | Ignores overhead, return rates and longer-term value unless included |
| Break-even ROAS | 1 / contribution-margin fraction | Valid only when that margin definition includes the intended variable costs |
| Modeled clicks | allocated media budget / assumed CPC | CPC and delivery vary; no impression-volume promise |
| Modeled conversions | modeled clicks × assumed conversion rate | Conditional scenario |
| CPA-based modeled acquisitions | allocated media budget / assumed CPA | Conditional; keep modeled fractional counts visible |
| Flat daily allocation | allocated channel budget / number of days | State actual date window and reserve |

For lead generation, contribution per lead can be modeled as qualified-lead-to-customer rate × contribution per acquired customer, minus lead handling costs if included. An assumed close rate is not an observed rate. For subscriptions/apps, use a specified payback window and validated cohort contribution rather than invented lifetime value.

## Worked planning fixture — synthetic

Media budget USD 1,500 for 30 days: Google USD 900, Meta USD 450, unspent reserve USD 150. Allocations total USD 1,500. Scheduled channel amounts are USD 30/day and USD 15/day; planned active spend totals USD 45/day × 30 = USD 1,350. The USD 150 reserve is not automatically spent.

At a target CPA assumption of USD 80, active planned spend models 16.875 acquisitions; the full USD 1,500 would model 18.75 only if the reserve is separately allocated. Neither is a forecast. If first-order contribution is USD 120/customer, a USD 80 CPA leaves a modeled USD 40 contribution after ads/customer before any omitted costs. First-order break-even CPA is USD 120 under those assumptions. Never describe the reserve-inclusive count as the active-spend count.

At assumed Google CPC USD 3 and click-to-customer conversion rate 4%, USD 900 models 300 clicks and 12 customers, implying USD 75 CPA. A downside 2% rate models 6 customers and USD 150 CPA. This sensitivity exceeds the USD 120 first-order break-even boundary; the plan needs a bounded test and a decision rule rather than a confident profitability claim.

Do not average CPC, CPA, CVR or ROAS across rows without their denominators. Do not add NO_DATA/nulls as zeroes or combine incompatible attribution windows. Stop rules should consider conversion lag, spend exposure, sample size and cash capacity; fixed CPA multiples are labeled heuristics, not universal proof.
