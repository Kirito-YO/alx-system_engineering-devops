                                           Postmortem Report

![It Hero](https://github.com/Kirito-YO/alx-system_engineering-devops/assets/106101462/031724d1-fd44-435c-b9f8-f0161f719516)
Why did the IT hero bring a ladder to the park?
Because he heard the network was experiencing an outage, and he wanted to "raise" the bar on connectivity! 🦸‍♂️🌐



**Issue Summary:**

Between 6:47 AM and 7:35 AM, an internet outage occurred at Site X, attributable to a power supply malfunction in the core switch.


**Timeline:**

- *6:47 AM:* Outage initiated
- *6:47 AM:* Pagers activated to alert teams
- *7:05 AM:* IT team identified the main issue and initiated troubleshooting
- *7:20 AM:* Second power supply plugged in
- *7:20 AM:* Switch rebooted
- *7:35 AM:* Full restoration, 100% of traffic back online


**Root Cause and Resolution:**

At 6:47 AM, the primary power supply of the core switch failed, and the backup power supply was not connected. Consequently, the backup did not assume the role following the primary failure. At 7:20 AM, the IT team successfully plugged in the second power supply, initiating the switch's reboot. By 7:35 AM, all services were restored.


**Corrective and Preventative Measures:**

In the aftermath of the incident, we have conducted a comprehensive internal review. To address the underlying causes and prevent future occurrences, the following corrective and preventative measures have been implemented:
- Ensure that all IT equipment is connected to two independent power sources.
- Maintain backup systems on standby for all IT equipment (High Availability).
- Configure all IT equipment for High Availability, allowing the standby unit to automatically assume the primary role in the event of a failure.
