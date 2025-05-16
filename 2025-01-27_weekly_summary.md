---
title: "Weekly Product Update: Team API, Site Provisioning, and Scan Reliability"
description: "This week's update brings enhancements to the Team API, fixes automatic site provisioning, boosts CVE scan reliability, and improves WAN tunnel stats display. Get the details!"
date: 2025-01-31
---

This week, we've focused on enhancing core functionalities and improving the reliability of several key areas of the platform. Read on for the highlights:

### Enhancements

*   **Comprehensive Team API:** The API endpoint for retrieving team details (`GET /teams/{team}`) now provides a more complete view by including the list of team members and pending invitations directly in the response. This allows you to get all essential team membership information with a single request.
*   **More Resilient Scan Data Processing:** Our process for enriching scan data with vulnerability information is now more robust. It's better equipped to handle temporary issues with external vulnerability databases, leading to more reliable and uninterrupted processing of your scan results.
*   **Faster Stuck Scan Termination:** Scans that become unresponsive or get stuck in a running state will now be automatically terminated after 1 hour of inactivity (previously 6 hours). This improvement helps free up resources more quickly and enhances overall scan reliability.
*   **Improved Scan Termination Logic:** We've enhanced the logic used to stop scans, making the termination process more reliable across various scan states.
*   **Reliable VPN Server Provisioning:** Improvements were made to the VPN server provisioning process to ensure core configuration files and settings, such as firewall rules and synchronization scripts, are correctly applied when new instances are deployed. This enhances the reliability and consistency of new servers.

### Bug Fixes

*   **Automatic Site Provisioning Fixed:** Resolved an issue where the automatic provisioning of new sites was not fully initiated upon creation. This update ensures that essential setup steps, such as tunnel IP assignment, API credential generation, and policy application, are now automatically triggered for all new sites, streamlining the site onboarding process.
*   **Improved WAN Tunnel Ping Stats Display:** Fixed an issue where graphs displaying WAN tunnel ping statistics might show gaps when data points were occasionally missed. The system now interpolates missing 5-minute intervals with 100% packet loss, providing a more complete and accurate representation of tunnel availability and performance over time.
