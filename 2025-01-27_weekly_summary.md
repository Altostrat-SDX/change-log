---
title: "Weekly Update: Enhanced API, Reliable Scans & Site Provisioning"
description: "This week's update brings an enhanced Team API, more reliable CVE scans with faster termination, fixed automatic site provisioning, and improved network statistics graphs."
date: 2025-01-31
---

## Weekly Platform Update: January 27 - February 2, 2025

We've been busy this week delivering improvements and fixes across the platform to enhance your experience and system reliability.

### Enhancements

*   **More Comprehensive Team API:** The API endpoint for retrieving team details now provides a richer response, including the list of team members and pending invitations directly. This allows you to get a complete view of team membership with a single request.
*   **Increased Scan Reliability:** We've made the process for enriching scan data more resilient to temporary issues with external vulnerability databases, ensuring smoother processing of your scan results.
*   **Improved Stuck Scan Handling:** Scans that become unresponsive will now be automatically terminated more quickly (after 1 hour instead of 6), freeing up resources faster. The logic for stopping scans has also been improved for greater reliability.
*   **More Consistent VPN Server Provisioning:** Updates to the server provisioning process ensure core configurations like firewall rules and synchronization scripts are applied correctly, leading to more reliable and consistent new server deployments.

### Bug Fixes

*   **Automatic Site Provisioning Fixed:** Resolved an issue where the essential setup steps for new sites, such as assigning tunnel IPs and generating API credentials, were not always fully initiated upon creation. New sites will now be correctly provisioned automatically, streamlining your onboarding process.
*   **Accurate WAN Tunnel Ping Stats:** Fixed an issue in graphs displaying WAN tunnel ping statistics that could show gaps. The system now provides a more complete representation of tunnel availability and performance over time, even if occasional data points are missed.

This release also includes various internal performance optimizations, logging improvements, and dependency updates to ensure the platform remains stable and performant.