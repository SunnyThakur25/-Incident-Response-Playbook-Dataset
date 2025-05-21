# -Incident-Response-Playbook-Dataset

🛡️ Incident Response Playbook Dataset

A comprehensive collection of 175 structured incident response playbooks designed to assist cybersecurity researchers, analysts, red teams, and automation engineers in building, simulating, and training robust defense strategies.
📁 Dataset Overview

    Format: JSONL (1 playbook per line)

    Total Entries: 175

    Use Cases:

        Automating SOC workflows

        Simulating incident response scenarios

        Red team/blue team playbook development

        Training ML/LLM-based security agents

📌 Data Schema

Each entry contains:
```{
  "incident_id": "IR-2025-0001",
  "incident_type": "Phishing Attack",
  "target_asset": "Windows AD Server",
  "detection_source": "SIEM Rule",
  "initial_vector": "Email Attachment",
  "tactics_techniques": [
    {"tactic": "Initial Access", "technique": "Phishing"},
    {"tactic": "Execution", "technique": "Command and Scripting Interpreter"},
    {"tactic": "Impact", "technique": "Data Encrypted for Impact"}
  ],
  "severity": "High",
  "playbook_steps": [
    {
      "phase": "Identification",
      "action": "Identification actions for Phishing Attack",
      "tools": ["SIEM", "Logs Review"],
      "response_time_min": 45
    },
    ...
  ],
  "final_status": "Resolved",
  "response_duration_total_min": 215,
  "tags": ["phishing", "data_encrypted_for_impact", "command_scripting"]
}
```
🔍 Key Fields
| Field                | Description                                                  |
| -------------------- | ------------------------------------------------------------ |
| `incident_type`      | Type of cyber incident (e.g., DDoS, Malware, Insider Threat) |
| `initial_vector`     | Entry method used by the attacker                            |
| `tactics_techniques` | Mapped MITRE ATT\&CK tactics and techniques                  |
| `playbook_steps`     | Step-by-step IR actions by phase                             |
| `tools`              | Tools used in each phase                                     |
| `severity`           | Severity classification (Low to Critical)                    |
| `tags`               | Normalized tags for filtering/search                         |
📊 Sample Use Cases

    🔁 Security Automation Pipelines

    🧠 Train LLMs for SOC Agent Simulations

    📚 Education for Incident Responders

    📈 Analytics for MITRE Coverage Gaps

    🧪 Red/Blue Team Simulation Models
    🤝 Contribution

Feel free to open issues or PRs for:

    New attack types

    Playbook enrichment

    Mappings to MITRE updates

📄 License

This dataset is released under the MIT license.
