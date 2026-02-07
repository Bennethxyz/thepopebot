**Task**: Update the Telegram notification formatting to properly format GitHub file links with correct paths

**Specific Requirements**:
1. Analyze the current `event_handler/tools/telegram.js` and related Telegram notification code
2. Identify where GitHub file links are being formatted (the issue shows "financialreport.md" instead of the full path)
3. Fix the link formatting to show the complete repository path (e.g., "operating_system/research_agent/financialreport.md")
4. Ensure links are properly formatted as HTML `<a href="url">text</a>` tags for Telegram
5. Test the formatting to make sure it works correctly in Telegram messages
6. If there's a `telegram.md` or similar configuration file in `operating_system/`, update it with proper formatting guidelines
7. Make sure the fix applies to all file change notifications, not just specific file types

**Context**: 
- The user reported that in job completion notifications, GitHub file links are showing only the filename (e.g., "financialreport.md") instead of the full path
- Telegram uses HTML formatting, not Markdown
- The file links should point to the actual GitHub file URLs and display the full repository path
- This is part of the job completion notification system that runs after auto-merge

**Expected Output**:
- Fixed Telegram notification formatting 
- Proper GitHub file links showing full paths
- Updated documentation if needed
- Test to ensure the fix works correctly