# Incident Report Analysis

## Summary
The organization experienced a denial of service (DoS) attack that disrupted internal network operations for approximately two hours. During the incident, internal network services became unavailable due to a flood of incoming ICMP packets. Normal internal traffic was unable to access network resources, impacting business operations. The incident was resolved after malicious traffic was blocked and critical network services were restored.

## Identify
The cybersecurity team investigated the incident by auditing network devices, firewall configurations, and network traffic logs. The investigation revealed that a malicious actor sent a large volume of ICMP ping requests into the organization’s network. An unconfigured firewall allowed this traffic to pass through unchecked, enabling the attacker to overwhelm network resources. The affected assets included internal network services and network infrastructure responsible for routing and traffic filtering.

## Protect
To improve protection against similar attacks in the future, the organization updated its firewall configuration to limit the rate of incoming ICMP packets. Source IP address verification was enabled on the firewall to detect and block spoofed IP addresses. The organization also implemented intrusion detection and prevention systems (IDS/IPS) to filter suspicious ICMP traffic and reduce the risk of future denial of service attacks.

## Detect
To improve detection capabilities, the organization implemented network monitoring software and firewall logging to continuously monitor inbound and outbound network traffic. An intrusion detection system (IDS) was configured to alert security staff to abnormal traffic patterns, such as unusually high volumes of ICMP packets. These tools will help the organization detect potential network attacks more quickly in the future.

## Respond
During the incident, the incident management team responded by blocking incoming ICMP traffic at the firewall. Non-critical network services were taken offline to reduce system load, while critical services were prioritized and restored. Upper management was informed of the incident, and response procedures were reviewed to ensure faster containment and communication in the event of future attacks.

## Recover
Following containment of the attack, network services were gradually restored to normal operation. The organization verified that systems were functioning correctly before resuming normal business activities. Lessons learned from the incident were used to improve firewall configurations, monitoring capabilities, and response procedures to reduce recovery time and minimize the impact of similar incidents in the future.

