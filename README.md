# Task-2-Identify-phishing-characteristics-in-a-suspicious-email-sample-

Phishing Email Analysis Report
Subject of the Email: Urgent: Your Account Has Been Locked!
Sender Address: support@paypall.com

1. Spoofed Sender Address
Finding: The sender is claimed to be from "PayPal" but the domain is "paypall.com" (additional 'l'), an old spoofing technique.
Risk: Users might trust the name "PayPal" without paying attention to the minute domain variation.

2. Email Header Inconsistencies
Tool Utilized: MxToolbox Email Header Analyzer
Discoveries:
SPF check failed: The email was not sent from a proper PayPal server.
DKIM and DMARC authentication failed.
Origin IP leads to a suspicious ISP in another country than PayPal HQ.

3. Suspicious Links
Hyperlink Text: "Restore your account"
Actual URL (hover): http://secure-paypal-verification.com/verify
Indicator: Mismatched and not legit domain. Not HTTPS-secured and not within PayPal's official domain.

4. Attachments
File Name: AccountUpdateForm.zip
Indicator: Compressed file, maybe malicious. Legitimate companies don't usually send ZIP attachments to verify an account.

5. Urgent or Threatening Language
Examples:
"Immediate action required!"
"Failure to respond will result in permanent account suspension.
Purpose: To instill fear and elicit quick, unthinking action.

6. Spelling and Grammar Mistakes
Examples:
"Your acount was suspend due to unusual activiti."
"Please verify immidiately to aviod ban."
Indicator: Poor language quality is a prevalent indication of phishing.

7. Generic Salutation
Text: "Dear Customer,"
Indicator: Legitimate business entities typically personalize emails with your full name.

Summary of Phishing Indicators:
Spoofed domain name (paypall.com)
Failed SPF/DKIM/DMARC authentication
Unusual and mismatched URLs
Threatening text that creates a sense of urgency
Poor grammar and spelling mistakes
Generic salutation

Attachment containing potentially malicious material
