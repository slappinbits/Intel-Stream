# Intel-Stream
📌 README.md — IOC Extraction & Enrichment Pipeline (n8n + LLMs)
IOC Extraction & Automated Threat Enrichment Pipeline

Built with n8n, Python, VirusTotal, Google Gemini, and Sigma-to-KQL/Raptor/Uptycs translation

<img width="1024" height="430" alt="image" src="https://github.com/user-attachments/assets/bdb05b4a-5e25-4dcb-974c-70086fa47696" />


🔎 Overview
This project is an end-to-end automated threat-intel and detection content generation pipeline, designed to take raw unstructured threat reports, extract Indicators of Compromise (IOCs), enrich them with VirusTotal, and automatically generate:

Sigma detection rules  
Mapped detection queries for:  
Microsoft Defender (KQL)  
CrowdStrike Falcon (Raptor)    
Uptycs (SQL)

The workflow demonstrates agentic AI, multi-stage automation, threat enrichment, IOC classification, and cross-platform detection engineering at scale.

🧠 Architecture Summary
Key Capabilities:  
Extracts IOCs from raw HTML, pasted text, or PDF-converted text  
Cleans and normalizes content (undoing obfuscation like hxxp://, [.], etc.)  
Classifies IOCs into domains, IPs, and hashes  
Calls VirusTotal API to enrich IOCs  
Filters malicious/suspicious indicators  
Auto-generates threat-hunting queries for:  
✔ Microsoft Defender (KQL)  
✔ CrowdStrike (Raptor)  
✔ Uptycs (SQL)  
Auto-generates Sigma rules using Google Gemini  
Translates Sigma rules into detection queries  
Converts output into downloadable files  
