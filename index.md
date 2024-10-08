<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CTI</title>
   <style>
        table {
            border-collapse: collapse;
            width: 130%;
            margin: 0 auto;
        }

        th, td {
            border: 1px solid black;
            padding: 8px;
            text-align: left;
        }

        th {
            background-color: #2874A6;
        }

        td:nth-child(2) {
            cursor: pointer;
            text-decoration: underline;
            color: blue;
        }
        
        td.analytics {
    width: 40%; 
    white-space: pre-line;
    color:black;
        }

        /* Define colors for different tactics */
        .reconnaissance { background-color: #CCCCCC; } 
        .resource-development { background-color: #808080; } 
        .initial-access { background-color: #87CEEB; } /* Sky Blue */
        .execution { background-color: #FFB6C1; } /* Light Pink */
        .persistence { background-color: #FFA07A; } /* Light Salmon */
        .privilege-escalation { background-color: #98FB98; } /* Pale Green */
        .defense-evasion { background-color: #FFDAB9; } /* Peach Puff */
        .credential-access { background-color: #ADD8E6; } /* Tomato */
        .discovery { background-color: #7FB3D5; } /* Light Blue */
        .lateral-movement { background-color: #2E86C1; } /* Orange Red */
        .collection { background-color: #737373; } /* Light Sea Green */
        .command-and-control { background-color: #FF69B4; } /* Hot Pink */
        .exfiltration { background-color: #00CED1; } /* Dark Turquoise */
        .impact { background-color: #FF8C00; } /* Dark Orange */
    </style>
</head>
<body>

<h2>MITRE ATT&CK® Techniques and Tactics mapper</h2>

<table>
    <tr>
        <th>Tactic</th>
        <th>Technique + Sigma rules</th>
        <th>ID</th>
        <th>Atomics</th>
    </tr>
    <tr>
<tr class="initial-access">
        <td>Initial Access</td>
        <td>Valid accounts</td>
        <td>T1078</td>
            <td class="analytics">
            <a href="https://atomicredteam.io/initial-access/T1078.001" target="_blank">Valid accounts: Default</a>
            <a href="https://atomicredteam.io/initial-access/T1078.003" target="_blank">Valid accounts: Local</a>
            <a href="https://atomicredteam.io/initial-access/T1078.004" target="_blank">Valid accounts: Cloud</a> 
    </td>
    </tr>
    <tr>
<tr class="initial-access">
        <td></td>
         <td>Exploit public-facing application</td>
        <td>T1190</td>
            <td></td>
    </tr>
    <tr>
<tr class="initial-access">
        <td></td>
         <td>External Remote Services</td>
        <td>T1133</td>
            <td class="analytics">
            <a href="https://atomicredteam.io/initial-access/T1133" target="_blank">External remote services</a><br>
    </td>
    </tr>
    <tr>
<tr class="execution">
        <td>Execution</td>
        <td>Command and Scripting Interpreter</td>
        <td>T1059</td>
        <td class="analytics">
            <a href="https://atomicredteam.io/execution/T1059.001" target="_blank">Command and Scripting Interpreter: Powershell</a>
            <a href="https://atomicredteam.io/execution/T1059.003" target="_blank">Command and Scripting Interpreter: CMD</a>
            <a href="https://atomicredteam.io/execution/T1059.004" target="_blank">Command and Scripting Interpreter: Bash</a>
            <a href="https://atomicredteam.io/execution/T1059.005" target="_blank">Command and Scripting Interpreter: VB</a>
            <a href="https://atomicredteam.io/execution/T1059.006" target="_blank">Command and Scripting Interpreter: Python</a>
            <a href="https://atomicredteam.io/execution/T1059.007" target="_blank">Command and Scripting Interpreter: Javascript</a>         
        </td>
    </tr>
    <tr>
<tr class="execution">
        <td></td>
        <td>User Execution: Malicious File</td>
        <td>T1204.002</td>
        <td class="analytics">
            <a href="https://atomicredteam.io/execution/T1204.002" target="_blank">User Execution: Malicious File</a>
        </td>
    </tr>
    <tr>
<tr class="execution">
        <td></td>
        <td>Windows Management Instrumentation</td>
        <td>T1047</td>
        <td class="analytics">
            <a href="https://atomicredteam.io/execution/T1047" target="_blank">WMI</a><br>
        </td>
    </tr>
    <tr>
<tr class="persistence">
        <td>Persistence</td>
        <td>Create or Modify System Process: Windows Service</td>
        <td>T1543.003</td>
            <td class="analytics">
            <a href="https://atomicredteam.io/atomics/#persistence" target="_blank">Atomics: Persistence</a><br>
        </td>
    </tr>
    <tr>
<tr class="persistence">
        <td></td>
        <td>Boot or Logon Autostart Execution</td>
        <td>T1547</td>
            <td></td>
    </tr>
    <tr>
<tr class="persistence">
        <td></td>
        <td>Boot or Logon Initialization Scripts</td>
        <td>T1037</td>
            <td></td>
    </tr>
    <tr>
<tr class="persistence">
        <td></td>
        <td>Scheduled Task/Job</td>
        <td>T1053</td>
            <td></td>
    </tr>
    <tr>
<tr class="persistence">
        <td></td>
        <td>BITS Jobs</td>
        <td>T1197</td>
            <td></td>
    </tr>
    <tr>
<tr class="privilege-escalation">
        <td>Privilege Escalation</td>
        <td>Access Token Manipulation</td>
        <td>T1134</td>
                <td class="analytics">
            <a href="https://atomicredteam.io/atomics/#privilege-escalation" target="_blank">Atomics: Privesc</a><br>
        </td>
    </tr>
    <tr>
<tr class="privilege-escalation">
        <td></td>
        <td>Exploitation for Privilege Escalation</td>
        <td>T1068</td>
            <td></td>
    </tr>
    <tr>
<tr class="privilege-escalation">
        <td></td>
        <td>Bypass User Account Control</td>
        <td>T1548.002</td>
            <td></td>
    </tr>
    <tr>
<tr class="privilege-escalation">
        <td></td>
        <td>Account Manipulation</td>
        <td>T1098</td>
            <td></td>
    </tr>
    <tr>
<tr class="privilege-escalation">
        <td></td>
        <td>Process Injection</td>
        <td>T1055</td>
            <td></td>
    </tr>
    <tr>
<tr class="defense-evasion">
        <td>Defense Evasion</td>
        <td>Impair Defenses</td>
        <td>T1562</td>
            <td class="analytics">
            <a href="https://atomicredteam.io/atomics/#defense-evasion" target="_blank">Atomics: Defense Evasion</a><br>
        </td>
    </tr>
    <tr>
<tr class="defense-evasion">
        <td></td>
        <td>Indicator Removal</td>
        <td>T1070</td>
            <td></td>
    </tr>
    <tr>
<tr class="defense-evasion">
        <td></td>
        <td>Obfuscated Files or Information</td>
        <td>T1027</td>
            <td></td>
    </tr>
    <tr>
<tr class="defense-evasion">
        <td></td>
        <td>Deobfuscate/Decode Files or Information</td>
        <td>T1140</td>
            <td></td>
    </tr>
    <tr>
<tr class="defense-evasion">
        <td></td>
        <td>System Binary Proxy Execution</td>
        <td>T1218</td>
            <td></td>
    </tr>
    <tr>
<tr class="defense-evasion">
        <td></td>
        <td>Masquerading</td>
        <td>T1036</td>
            <td></td>
    </tr>
    <tr>
<tr class="credential-access">
        <td>Credential Access</td>
        <td>Brute Force</td>
        <td>T1110</td>
            <td class="analytics">
            <a href="https://atomicredteam.io/atomics/#credential-access" target="_blank">Atomics: Credential access</a><br>
        </td>
    </tr>
    <tr>
<tr class="credential-access">
        <td></td>
        <td>Steal Application Access Token</td>
        <td>T1528</td>
            <td></td>
    </tr>
    <tr>
<tr class="credential-access">
        <td></td>
        <td>Credentials from Web Browsers</td>
        <td>T1555.003</td>
            <td></td>
    </tr>
    <tr>
    <tr class="credential-access">
        <td></td>
        <td>Steal Web Session Cookie</td>
        <td>T1539</td>
                <td></td>
    </tr>
    <tr>
<tr class="credential-access">
        <td></td>
        <td>OS Credential Dumping</td>
        <td>T1003</td>
            <td></td>
    </tr>
    <tr>
<tr class="discovery">
    <td>Discovery</td>
    <td>Account Discovery</td>
    <td>T1087</td>
            <td class="analytics">
            <a href="https://atomicredteam.io/atomics/#discovery" target="_blank">Atomics: Discovery</a><br>
        </td>
</tr>

<tr class="discovery">
    <td></td>
    <td>Network Share Discovery</td>
    <td>T1135</td>
            <td></td>
</tr>

<tr class="discovery">
    <td></td>
    <td>File and Directory Discovery</td>
    <td>T1083</td>
            <td></td>
</tr>

<tr class="discovery">
    <td></td>
    <td>Process Discovery</td>
    <td>T1057</td>
            <td></td>
</tr>

<tr class="discovery">
    <td></td>
    <td>Remote System Discovery</td>
    <td>T1018</td>
            <td></td>
</tr>

<tr class="discovery">
    <td></td>
    <td>System Information Discovery</td>
    <td>T1082</td>
            <td></td>
</tr>

<tr class="discovery">
    <td></td>
    <td>System Network Connections Discovery</td>
    <td>T1049</td>
            <td></td>
</tr>

<tr class="discovery">
    <td></td>
    <td>System Owner/User Discovery</td>
    <td>T1033</td>
            <td></td>
</tr>

<tr class="lateral-movement">
    <td>Lateral Movement</td>
    <td>Remote Services</td>
    <td>T1021</td>
            <td class="analytics">
            <a href="https://atomicredteam.io/atomics/#lateral-movement" target="_blank">Atomics: Lateral movement</a><br>
        </td>
</tr>

<tr class="lateral-movement">
    <td></td>
    <td>Lateral Tool transfer</td>
    <td>T1570</td>
            <td></td>
</tr>

<tr class="command-and-control">
    <td>Command and Control</td>
    <td>Application Layer Protocol</td>
    <td>T1071</td>
            <td class="analytics">
            <a href="https://atomicredteam.io/atomics/#command-and-control" target="_blank">Atomics: C2</a><br>
        </td>
</tr>

<tr class="command-and-control">
    <td></td>
    <td>Ingress Tool Transfer</td>
    <td>T1105</td>
            <td></td>
</tr>
<tr class="command-and-control">
    <td></td>
    <td>Proxy</td>
    <td>T1090</td>
            <td></td>
</tr>

<tr class="exfiltration">
    <td>Exfiltration</td>
    <td>Exfiltration Over C2 Channel</td>
    <td>T1041</td>
            <td class="analytics">
            <a href="https://atomicredteam.io/atomics/#exfiltration" target="_blank">Atomics: Exfiltration</a><br>
        </td>
</tr>

<tr class="exfiltration">
    <td></td>
    <td>Exfiltration to Cloud Storage</td>
    <td>T1567.002</td>
            <td></td>
</tr>

<tr class="impact">
    <td>Impact</td>
    <td>Inhibit System Recovery</td>
    <td>T1490</td>
            <td class="analytics">
            <a href="https://atomicredteam.io/atomics/#impact" target="_blank">Atomics: Impact</a><br>
        </td>
</tr>

<tr class="impact">
    <td></td>
    <td>Service stop</td>
    <td>T1489</td>
            <td></td>
</tr>

<tr class="impact">
    <td></td>
    <td>Data Encrypted for Impact</td>
    <td>T1486</td>
            <td></td>
</tr>
<tr class="impact">
    <td></td>
    <td>Network Denial of Service</td>
    <td>T1498</td>
            <td></td>
</tr>

<script>
    // Function to handle technique hyperlink clicks for MITRE ATT&CK
    function redirectToMitre(techniqueID) {
        // Replace dot with a forward slash
        const formattedTechniqueID = techniqueID.replace(/\./g, '/');
        
        // Open the link in a new tab
        window.open(`https://attack.mitre.org/techniques/${formattedTechniqueID}/`, '_blank');
    }

    // Function to handle technique ID clicks for detection.fyi
    function redirectToDetectionFyi(techniqueID) {
        // Convert Technique ID to lowercase
        const lowercaseTechniqueID = techniqueID.toLowerCase();

        // Open the link in a new tab
        window.open(`https://detection.fyi/tags/attack.${lowercaseTechniqueID}/`, '_blank');
    }

    // Add event listeners to the technique cells for hyperlink functionality
    document.querySelectorAll('td:nth-child(2)').forEach((nameCell) => {
        if (nameCell.innerText.trim() !== '') {
            nameCell.style.cursor = 'pointer';
            nameCell.addEventListener('click', () => {
                const techniqueID = nameCell.nextElementSibling.innerText.trim();
                redirectToDetectionFyi(techniqueID);
            });
        }
    });

    // Add event listeners to the technique cells for hyperlink functionality
    document.querySelectorAll('td:nth-child(3)').forEach((idCell) => {
        if (idCell.innerText.trim() !== '') {
            idCell.style.cursor = 'pointer';
            idCell.addEventListener('click', () => {
                const techniqueID = idCell.innerText.trim();
                redirectToMitre(techniqueID);
            });
        }
    });
</script>

