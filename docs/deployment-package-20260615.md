# Deployment package - 2026-06-15

This document records the latest local app build and data backup prepared from the connected Google Drive/card usage workflow.

## Google Drive backups

- Latest HTML app backup: https://drive.google.com/file/d/1-9_RCTZVd4ciu9vgW1RdZRsmV3hApxLS/view?usp=drivesdk
- Update README: https://drive.google.com/file/d/1grdxQlOnNTpYIpn8I3Dy_TnQtfAADStq/view?usp=drivesdk
- Parsed usage data text backup: https://drive.google.com/file/d/1nuctBgv9RxbTqG-m08HzYrrn7Wxoy5G1/view?usp=drivesdk
- Embedded app preset text backup: https://drive.google.com/file/d/1lX3ts2uxadBn9020pXlWGxjVHeSQjdp1/view?usp=drivesdk

## Local build summary

- Source HTML: `outputs/improved-index.html`
- Usage data source: Woori Card XLS, Samsung Card PDF, Naver Hyundai Card XLS
- Usage period: 2025-07-06 to 2026-06-15
- Transactions: 321
- Total amount: 12,614,100 KRW
- Monthly average: 1,051,175 KRW

## Included local UI changes

- Existing card benefit/performance check for Samsung taptap O, Woori DA@, Hana Any PLUS, and Naver Hyundai Card
- Benefit category icon grid inspired by card search/category workflows
- Imported card usage preset and detailed merchant rows
- May/June monthly usage workflow
- Next-month spending forecast
- New-card expected benefit comparison workflow
- Readability cleanup for merchant rows and owned-card summaries

## Deployment note

The full `index.html` build is available in the Drive HTML backup above. Publishing it to GitHub Pages requires pushing that HTML into `index.html` on the deployment branch or `main`. The local environment currently has GitHub CLI installed but not authenticated, so the large HTML file could not be pushed from the local filesystem in this session.