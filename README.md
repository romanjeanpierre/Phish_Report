 <h1>Phishing Report Writing Example </h1>

   <h2>Project Description</h2>
    <p>This document presents a comprehensive analysis of a phishing email incident. The report is structured to provide detailed insights into the nature of the email, the artifacts collected, and the subsequent analysis carried out. It concludes with suggested defensive measures to mitigate future risks, thereby enhancing the organization's cybersecurity posture.</p>

   <h2>Section 1: Email Description and Artifacts Collected</h2>
  
  <p>
        <strong>Sending Address:</strong> emailsecalert1@gmail.com<br>
        <strong>Subject Line:</strong> Your Email Will be Locked! Act NOW!<br>
        <strong>Recipients:</strong>
      <ul>
            <li>john.smith@dicksonunited.co.uk</li>
            <li>alice.cooper@dicksonunited.co.uk</li>
            <li>jacon.long@dicksonunited.co.uk</li>
            <li>fred.johnson@dicksonunited.co.uk</li>
            <li>pickle.rick@dicksonunited.co.uk</li>
        </ul>
        <strong>Sending Server IP:</strong> 209.85.222.173<br>
        <strong>Reverse DNS:</strong> mail-qk1-f173.google.com (Gmail)<br>
        <strong>Reply-To:</strong> emailsecalert1@gmail.com<br>
        <strong>Date and Time:</strong> 3:21 PM Monday 1st June 2020<br>
        <strong>Full URL (sanitized):</strong> hxxps://outlook-security.emailsecalerts[.]net/index/2020/OWA.php?<br>
        <strong>Root Domain:</strong> hxxps://emailsecalerts[.]net<br>
    </p>


  <h2>Section 2: Artifact Analysis</h2>

   <p>
        <strong>Email Analysis:</strong> The email impersonates an Outlook security alert and uses Outlook branding. It warns recipients that their mailboxes will be closed unless they confirm their identity by clicking a provided button.<br>
       <strong>Reverse DNS Analysis:</strong> Confirms that the email originated from Gmail.<br>
        <strong>URL Analysis:</strong> URL2PNG indicates the URL hosts an Outlook credential harvester. VirusTotal flags the domain for malicious/phishing activity.<br>
        <strong>Network Analysis:</strong> SIEM and EDR checks confirm no network connections to the malicious domain. The email gateway shows no responses sent to the email.<br>
        <strong>Domain Analysis:</strong> The domain emailsecalerts[.]net appears to be a case of typo squatting, posing as a legitimate email security alert domain.<br>
        </p>

  
  <h2>Section 3: Suggested Defensive Measures</h2>

   <p>
        <strong>Email Block:</strong> Request an email gateway block for “emailsecalert1@gmail.com” to prevent further malicious emails from this sender.<br>
        <strong>Domain Block:</strong> Block “hxxps://emailsecalerts[.]net” on the web proxy. The domain is identified as malicious with no legitimate use, hosting a credential harvester. This action prevents employee access and future phishing attempts using this domain.<br>
    </p>

