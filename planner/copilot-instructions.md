# Copilot Instructions — Holiday Sync Planner

When the user asks to update or generate holiday plans:

1. **Tool location**: `holiday-planner.html` in this directory
2. **Self-contained**: Single HTML file, open directly in browser, no dependencies
3. **How to update Chinese holidays**: Edit the `getHolidays()` function's CN section — each year the State Council (国务院) publishes official dates, update `offDays` and `workDays` arrays accordingly
4. **How to update Australian holidays**: Edit the AU section — holidays follow fixed rules except Easter (auto-calculated)
5. **Adding a new year**: Extend the lookup maps in `chineseNewYear()`, `duanwu()`, `midAutumn()` etc.

## Data Sources
- 🇨🇳 China: [国务院办公厅关于节假日安排的通知](http://www.gov.cn)
- 🇦🇺 Australia (NSW): [NSW Public Holidays](https://www.nsw.gov.au/about-nsw/public-holidays)

## Customization
- Change AU state: modify AU holidays in `getHolidays()`
- Change default leave days: edit `value` attribute on the `<input>` elements
- Add more third-country destinations: edit the Tips section at the bottom
