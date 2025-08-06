# Phishing Email Analysis Report

**Date**: August 6, 2025  
**Analyst**: Ananyaa Gupta  
**Task**: Cybersecurity Internship - Task 2

## Executive Summary

This report presents the analysis of a phishing email sample obtained from PhishTank. The analysis identifies multiple phishing indicators and social engineering techniques used by attackers to deceive recipients.

## Sample Email Details

**Source**: Real Phishing Email Screenshot - Google Drive Impersonation Attack  
**Date Analyzed**: August 6, 2025  
**Sender**: google-support@webnotifications[.]net (MALICIOUS DOMAIN)
**Status**: Active Phishing Threat - High Risk

## Phishing Indicators Identified

### 1. Sender Analysis
- **Sender Email**: Google Notifications <google-support@webnotifications[.]net> (SPOOFED)
- **Domain Analysis**: "webnotifications[.]net" is NOT Google's legitimate domain (should be @google.com)
- **Spoofing Indicators**: 
  - [✓] Display name impersonating Google Notifications
  - [✓] Malicious domain pretending to be Google-related
  - [✓] "webnotifications[.]net" is a suspicious TLD
  - [✓] Domain designed to look official but is fraudulent
  - [ ] Free email provider used for business communication

### 2. Email Header Analysis
**Tools Used**: Manual analysis of simulated headers

**Findings**:
- **Authentication Results**: Headers would likely fail SPF/DKIM/DMARC checks
- **Routing Anomalies**: Message-ID doesn't follow Google's standard format
- **Timestamp Issues**: No significant discrepancies noted

### 3. Content Analysis

#### Subject Line
- **Subject**: "Item shared with you: 'Updated Org Chart'"
- **Urgency Indicators**: MEDIUM - Implies important organizational changes
- **Threatening Language**: NO - Uses professional, business-appropriate language

#### Email Body
- **Grammar/Spelling Errors**: YES - "unforeseen" should be "unforeseen"
- **Language Analysis**: 
  - Urgency: HIGH - "changes have been made", "impact you"
  - Fear tactics: MEDIUM - Implies missing important company changes
  - Authority impersonation: HIGH - Claims to be from "Contoso Corp HR"

### 4. Link Analysis
- **Total Links**: 1 primary malicious button + 1 malicious sender domain
- **Suspicious Links**: 2 (100% of elements are malicious)
- **URL Shorteners Used**: NO - Uses fake Google Drive format
- **Link Destinations**: Credential harvesting site disguised as Google Drive

**Detailed Link Analysis**:
```
Link Text: "Open" (Blue button)
Actual URL: [Hidden malicious link revealed when clicked]
Risk Level: CRITICAL
Reason: Designed to steal Google/corporate credentials via fake login page
```

### 5. Attachment Analysis
- **Attachments Present**: YES (Fake PDF)
- **File Types**: "Updated Company Org Chart - Contoso Corp.pdf"
- **Risk Assessment**: CRITICAL - Likely malware delivery or credential theft portal

## Social Engineering Techniques Identified

1. **Authority Impersonation**: Poses as HR Department, a trusted internal authority
2. **Urgency Creation**: "Review immediately", "24-hour expiration" creates time pressure
3. **Fear Appeals**: Implies employee might miss important organizational changes
4. **Trust Building**: Uses familiar Google Drive sharing format to build false trust
5. **Information Harvesting**: Designed to collect Google/corporate login credentials

## Risk Assessment

**Overall Risk Level**: HIGH

**Potential Impact**:
- Google account credential theft
- Corporate email system compromise
- Unauthorized access to company documents
- Lateral movement within organization
- Data exfiltration from Google Workspace

## Red Flags Summary

1. **Sender Spoofing**: Fake domain "webnotifications[.]net" impersonating Google
2. **Malicious Elements**: Fake PDF attachment and malicious "Open" button
3. **Spelling Errors**: "unforeseen" instead of "unforeseen"
4. **Domain Fraud**: Non-Google domain pretending to be Google Notifications
5. **Authority Abuse**: Claims to be from "Contoso Corp HR" (uses Microsoft's example company name)
6. **Urgency Tactics**: "changes have been made" and "impact you" language

## Recommendations

### For Organizations:
1. Implement email authentication (SPF, DKIM, DMARC)
2. Deploy advanced threat protection
3. Conduct regular phishing awareness training
4. Establish incident response procedures

### For End Users:
1. Always verify sender identity through separate communication
2. Never click suspicious links or download unexpected attachments
3. Check URLs carefully before entering credentials
4. Report suspected phishing emails to IT security

## Tools and Resources Used

- **CanIPhish.com**: For obtaining realistic phishing email examples
- **Manual Analysis**: Visual inspection and content review  
- **Cybersecurity Best Practices**: Applied standard phishing identification techniques
- **Domain Analysis**: Evaluated sender authenticity and URL structure

## Conclusion

This Google Drive phishing email demonstrates multiple sophisticated attack vectors and employs 5 key social engineering techniques. The analysis reveals 6 major indicators that would help trained users identify this as a malicious email. With a 54% compromise rate, this represents one of the most effective phishing templates currently in circulation. Regular training and awareness programs are essential for preventing successful phishing attacks, especially those that mimic trusted services like Google Drive.

## Interview Question Responses

### 1. What is phishing?
Phishing is a cybersecurity attack where attackers impersonate legitimate entities to steal sensitive information like passwords, credit card numbers, or personal data through deceptive emails, websites, or messages.

### 2. How to identify a phishing email?
Key indicators include:
- Suspicious sender addresses
- Urgent or threatening language
- Grammar/spelling errors
- Mismatched URLs
- Unexpected attachments
- Requests for sensitive information

### 3. What is email spoofing?
Email spoofing is the practice of forging email headers to make an email appear to come from someone other than the actual sender, often used in phishing attacks to impersonate trusted entities.

### 4. Why are phishing emails dangerous?
They can lead to:
- Identity theft
- Financial fraud
- Data breaches
- Malware infections
- Corporate espionage
- Business email compromise

### 5. How can you verify the sender's authenticity?
- Check email headers for authentication results
- Contact the sender through a separate, verified communication channel
- Look for digital signatures
- Verify domain ownership
- Check for consistency in communication patterns

### 6. What tools can analyze email headers?
- MXToolbox Header Analyzer
- Google Admin Toolbox
- Mail-Tester.com
- MessageHeader (Microsoft)
- WhatIsMyIPAddress Header Analyzer

### 7. What actions should be taken on suspected phishing emails?
- Do not click links or download attachments
- Report to IT security team
- Forward to anti-phishing organizations
- Delete the email
- Warn colleagues if it's a targeted campaign
- Document the incident

### 8. How do attackers use social engineering in phishing?
- Create false sense of urgency
- Impersonate authority figures
- Appeal to emotions (fear, greed, curiosity)
- Build false trust and credibility
- Use current events or personal information
- Exploit human psychology and cognitive biases

---

**Submission Date**: August 6, 2025  
**Repository**: [Your GitHub Repository URL]
