# Author reconciliation notes — keep out of submission

This LaTeX project uses the official WACV 2027 author kit in anonymous review mode, Applications track. Replace the placeholders and move the paper ID only after enrollment. The main source contains TODO markers and figure placeholders where information was absent.

## Reconcile before submission

- Seed list is inconsistent: seed 42, 2026, 2016, and 512 appear across different summaries. Recover completed runs for each E1–E4 model.
- E1 validation R² standard deviation is 0.030 in the aggregate table but 0.000 in prose. Recompute all means and standard deviations from raw results.
- Keep test metrics for final evaluation only; confirm checkpoint/model selection used validation data.
- Rejected patch reason counts sum to 99, while 118 patches are excluded. Explain overlap or missing categories. The retained samples account for 7,522 of 8,063 initially valid GEDI cells; explain the remaining 541.
- Confirm all models use the same 812 validation cells and 163 test cells.
- Add verified sensor processing, GEDI filtering, CRS, exact architecture, loss/reduction, optimizer and schedule, training settings, seed list, software/hardware, and parameter counts.
- Add study area/split map, architecture figure, prediction diagnostics, height-bin results, and dense-map panel from actual project outputs. No figure placeholders are data.
- State code/data access accurately.

The reported aggregate test metrics currently favor dual encoders (MAE 2.362 ± 0.137 m; RMSE 3.123 ± 0.179 m), but these remain provisional until seed reconciliation.
