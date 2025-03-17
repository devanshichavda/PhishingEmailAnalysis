# PhishingEmailAnalysis

Objective

The Phishing Email Analysis lab's aim was to analyze a potentially malicious email and its attachments, utilizing various analysis techniques such as email header analysis, base64 decoding, file signature analysis, and hexadecimal analysis to uncover hidden content and ultimately reveal the concealed message.

Skills Learned

- Email Header Analysis: Gained proficiency in analyzing email headers (SPF, DKIM, DMARC) to assess email authenticity and identify potential phishing or spoofing indicators.
- Base64 Decoding: Enhanced skills in decoding base64 encoded content within emails and attachments to uncover hidden information and malicious payloads.
- File Signature Analysis: Developed expertise in identifying file types through hexadecimal inspection of file signatures, even when file extensions are manipulated or disguised.
- Hexadecimal Analysis: Strengthened skills in using hexadecimal editors (HxD) to examine file structures, metadata, and identify anomalies.

Tools Used

- BlueTeamLabs Online & Text Editor: For accessing the challenge and analyzing data.
- Base64 Decoder & File Archiver: For decoding content and extracting files.
- HxD Hex Editor: For in-depth file analysis.
- UTM Virtual Machine: For secure analysis

Steps

1) Accessed the Challenge: Registered and accessed the "Planet's Prestige" challenge on the BlueTeamLabs Online platform.
2) Retrieved the Suspicious Email: Downloaded the provided suspicious email for analysis.<img width="1203" alt="Screenshot 2025-03-17 at 11 28 12 AM" src="https://github.com/user-attachments/assets/311c3b1b-c576-485a-8b2c-9908cbb3f67b" />

3) Analyzed Email Headers: Examined the email headers, including SPF, DKIM, and DMARC records, to assess the email's authenticity and identify potential red flags.
4) Decoded Email Content: Decoded the base64 encoded content within the email body to reveal further information.<img width="1190" alt="Screenshot 2025-03-17 at 11 33 29 AM" src="https://github.com/user-attachments/assets/6ecdb0cc-5496-4dab-9bf5-fbde196bf450" />
<img width="1184" alt="Screenshot 2025-03-17 at 11 40 45 AM" src="https://github.com/user-attachments/assets/803dbfc2-8981-4cfa-a6d9-3acce62e41ab" />

5) Identified and Decoded Attachment: Located a base64 encoded attachment within the email and decoded it.<img width="840" alt="Screenshot 2025-03-17 at 11 42 49 AM" src="https://github.com/user-attachments/assets/b721b870-1321-4abd-96b0-fc181f4fcfdc" />

6) Performed File Signature Analysis: Analyzed the first bytes of the decoded attachment in hexadecimal format to determine the true file type, revealing it to be a ZIP archive despite a misleading extension.<img width="1180" alt="Screenshot 2025-03-17 at 11 46 41 AM" src="https://github.com/user-attachments/assets/e01926aa-a7b9-422d-a6b3-612ea7bb049f" /><img width="690" alt="Screenshot 2025-03-17 at 3 15 43 PM" src="https://github.com/user-attachments/assets/312df7d5-23a4-4d44-96a3-9519c63308d4" />


7) Extracted Archive Contents: Extracted the contents of the ZIP archive, noting any hidden files or unusual file structures.<img width="1180" alt="Screenshot 2025-03-17 at 11 48 52 AM" src="https://github.com/user-attachments/assets/0a87f451-a53b-4c21-b226-86030af9f945" />

8) Utilized Hexadecimal Analysis: Employed a hexadecimal editor (HxD) to further examine the extracted files and confirm their types.<img width="1181" alt="Screenshot 2025-03-17 at 2 20 02 PM" src="https://github.com/user-attachments/assets/1ae0339f-3a39-4e98-9d30-4c8a8057ffcb" />

9) Decoded Final Payload: Identified and decoded a base64 encoded Excel file within the extracted archive, revealing the final hidden message.<img width="1194" alt="Screenshot 2025-03-17 at 2 30 50 PM" src="https://github.com/user-attachments/assets/bcabfca3-0b47-4b06-b108-22368c8b36c4" />
<img width="1198" alt="Screenshot 2025-03-17 at 2 32 04 PM" src="https://github.com/user-attachments/assets/b4a55a50-39c9-49a2-b551-08217cbeed69" />
<img width="1192" alt="Screenshot 2025-03-17 at 2 36 15 PM" src="https://github.com/user-attachments/assets/2ada0d04-028a-4a2f-bc37-e280f3d1c89e" />
