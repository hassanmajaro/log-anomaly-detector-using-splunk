# Alert Setup in Splunk

## Alert: Failed Login Surge

1. Go to "Search & Reporting"
2. Paste query from `failed_login_surge.spl`
3. Click "Save As" > Alert
4. Name: Brute Force Alert
5. Trigger: if result count > 0
6. Action: email/webhook

Repeat similar steps for other alert types.
