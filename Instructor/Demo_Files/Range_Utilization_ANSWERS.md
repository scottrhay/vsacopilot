# Range_Utilization.xlsx — Instructor Answer Key
## Demo D1 expected results
1. Variance formula (ask: percent variance BookedHours vs ActualHours, safe when Booked=0):
   `=IFERROR(([@ActualHours]-[@BookedHours])/[@BookedHours],0)`  — accept IF(BookedHours=0,...) variants. Format as %.
2. 'Explain this formula' target (Notes!B4): a SUMPRODUCT weighted average — revenue-per-hour weighted by actual hours, Pads A/B only, MAX(1,..) guards divide-by-zero. Copilot should say roughly: "average revenue per actual hour across the two main pads, weighted so busier months count more."
3. What-if framing (+2 launches/month): expect Copilot to suggest a scenario column (e.g. AdjActualHours = ActualHours + 2*avg-hours-per-launch) and recomputed Revenue; instructor builds ONE column live, no more.
## Gotchas
- If the table name is lost (opened/re-saved), re-add: select data > Insert > Table > name it RangeOps.
- Numbers vary by build seed; verify the workbook opens with table intact the morning of delivery.
