---
title: "Weekly Product Update: Enhanced Reliability & Key Fixes (Jan 27 - Feb 2)"
description: "This week: Enhanced reliability, faster stuck scan termination, improved Team API data, and fixes for site provisioning & metrics graphs. Get the details here!"
date: 2025-01-31
---

## Weekly Product Changelog Summary (Jan 27, 2025 - Feb 2, 2025)

This week's update focuses on enhancing the reliability and efficiency of several core services, alongside providing more comprehensive data and resolving key issues.

### Enhancements

*   **Improved Team Data Visibility:** The API for retrieving team details now includes a full list of team members and pending invitations in a single request, providing a more complete picture of your team setup.
*   **More Resilient CVE Scan Data Processing:** Our system for processing CVE scan results is now more robust and less susceptible to temporary outages from external vulnerability databases, ensuring more reliable data enrichment.
*   **Faster Stuck Scan Termination:** Scans that become unresponsive will now be automatically terminated after 1 hour instead of 6, freeing up resources and improving scan reliability.
*   **More Reliable Scan Stopping:** We've improved the logic for stopping scans, making the termination process more effective even if a scan is in an intermediate state.
*   **Enhanced VPN Server Stability:** Improvements were made to the VPN server provisioning process and internal synchronization, ensuring new servers are deployed more reliably with correct configurations and ongoing updates are more stable.

### Bug Fixes

*   **Automated Site Provisioning Fixed:** Resolved an issue where essential setup steps (like tunnel IP assignment, API credentials, and policy application) were not always fully initiated for new sites upon creation. This process is now correctly automated.
*   **Accurate WAN Tunnel Ping Stats:** Fixed an issue in the metrics display where graphs for WAN tunnel ping statistics might show gaps. The system now interpolates missing data points to provide a more complete and accurate representation of tunnel performance.
