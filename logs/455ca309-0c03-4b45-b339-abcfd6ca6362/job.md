Create a financial advisor agent system with the following components:

1. **operating_system/FINANCIAL_ADVISOR/FINANCIAL_ADVISOR.md** - Define the bot's daily morning routine including:
   - Pre-market research tasks (economic indicators, overnight news, futures, etc.)
   - Data sources to check using Brave search
   - Analysis methodology
   - Report generation process

2. **operating_system/FINANCIAL_ADVISOR/FINANCIAL_REPORT_TEMPLATE.md** - Create a structured template defining:
   - Market overview section
   - Key economic indicators
   - Sector analysis
   - Notable stock movements
   - Risk factors and opportunities
   - Daily recommendations format

3. **operating_system/FINANCIAL_ADVISOR/FINANCIAL_REPORT.md** - The final daily report output location

4. **Update CRONS.json** - Add a daily 6am cron job that:
   - References the operating_system/FINANCIAL_ADVISOR/FINANCIAL_ADVISOR.md instructions
   - Uses Brave search for all market research
   - Generates the daily report following the template structure
   - Saves output to operating_system/FINANCIAL_ADVISOR/FINANCIAL_REPORT.md

The system should be designed for daily automated execution with comprehensive market analysis using Brave search before trading hours begin.