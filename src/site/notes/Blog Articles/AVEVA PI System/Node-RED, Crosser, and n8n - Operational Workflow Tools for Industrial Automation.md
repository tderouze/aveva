---
{"dg-publish":true,"permalink":"/blog-articles/aveva-pi-system/node-red-crosser-and-n8n-operational-workflow-tools-for-industrial-automation/","dgPassFrontmatter":true}
---

Low-code platforms like Node-RED, Crosser, and n8n streamline data flows in operational environments, from edge devices to enterprise systems, each integrating with AVEVA PI System via APIs or dedicated connectors.​

## Node-RED for Flexible Edge Integration

Node-RED excels in event-driven flows for IoT and prototyping, running on lightweight hardware like Raspberry Pi.
It connects to AVEVA PI System through the community node `node-red-contrib-osisoft-web-api`, enabling read/write queries via PI Web API with basic authentication and custom URLs for points or data streams. 
Operators use it for quick setups like pushing sensor data to PI tags or pulling historical values, ideal for field deployments without heavy infrastructure.​

## Crosser for Enterprise IIoT Scalability

Crosser targets industrial-scale operations with central management, high-performance .NET runtime, and built-in AI/ML support for edge analytics.
As an official AVEVA partner, it offers pre-built connectors across the AVEVA portfolio, including PI System, via interactive wizards for data selection and mapping from edge to cloud.
Teams deploy flows across multiple sites, monitor data quality in real-time, and feed processed OT/IT data bidirectionally into PI for unified analytics.​

## n8n for Modern Automation Workflows

n8n focuses on versatile, self-hosted automations blending IT and OT, with strong nodes for APIs, databases, and messaging.
While no native PI connector exists, it interfaces via HTTP/OPC UA nodes to PI Web API or OMF endpoints, routing industrial data like PLC alarms or MQTT streams into PI tags.
It's popular for hybrid setups, such as logging SCADA data to PI then triggering reports, suiting developers familiar with Node.js ecosystems.​

## Comparison for PI System Operations

|Feature|Node-RED|Crosser.io|n8n|
|---|---|---|---|
|Core Strength|Edge prototyping, community nodes|Enterprise scaling, AVEVA partnership|Flexible IT/OT automations|
|PI Integration|Web API community node |Native connectors & wizards​|HTTP/OPC UA to Web API ​|
|Deployment|Single instances, Docker|Central console, multi-edge |Self-hosted workflows |
|Best For|PoCs, home labs|Multi-site IIoT|Custom alerts, reporting |
|Cost|Free open source ​|Subscription plans |Free core, paid cloud |

Choose Node-RED for rapid tests, Crosser for governed production, or n8n for extensible workflows—all enhance PI System by bridging real-time data gaps.​

1. [https://flows.nodered.org/node/node-red-contrib-osisoft-web-api](https://flows.nodered.org/node/node-red-contrib-osisoft-web-api)
2. [https://crosser.io/partners/partner-pages/aveva/](https://crosser.io/partners/partner-pages/aveva/)
3. [https://n8n.io/integrations/](https://n8n.io/integrations/)
4. [https://nodered.org](https://nodered.org/)
5. [https://community.aveva.com/pi-square-community/f/forum/88224/cloud-node-red-connect-to-pi-web-api](https://community.aveva.com/pi-square-community/f/forum/88224/cloud-node-red-connect-to-pi-web-api)
6. [https://community.aveva.com/pi-square-community/f/forum/94920/node-red-pi-omf-connector-weather-underground---getting-it-running](https://community.aveva.com/pi-square-community/f/forum/94920/node-red-pi-omf-connector-weather-underground---getting-it-running)
7. [https://crosser.io/blog/key-differences-between-node-red-and-crosser-in-industrial-iot/](https://crosser.io/blog/key-differences-between-node-red-and-crosser-in-industrial-iot/)
8. [https://crosser.io](https://crosser.io/)
9. [https://www.crosser.io/blog/crosser-announces-a-full-suite-of-aveva-connectors-powered-by-the-new-interactive-wizard/](https://www.crosser.io/blog/crosser-announces-a-full-suite-of-aveva-connectors-powered-by-the-new-interactive-wizard/)
10. [https://crosser.io/blog/how-crosser-complements-osi-soft-pi-system/](https://crosser.io/blog/how-crosser-complements-osi-soft-pi-system/)
11. [https://www.linkedin.com/posts/mohaneee13_how-you-can-use-n8n-in-your-field-plc-activity-7379059390135455744-LxUS](https://www.linkedin.com/posts/mohaneee13_how-you-can-use-n8n-in-your-field-plc-activity-7379059390135455744-LxUS)
12. [https://cdn.mediavalet.com/eunl/content/zknZRgZIdk-tAPjdS7cRgg/WDN5RjMomk62JQ93as4phg/Original/Methanex:%20Unlocking%20AI%E2%80%99s%20Potential%20with%20PI%20System%20Data%20&%20CONNECT:%20A%20Simplified,%20Scalable%20Approach.pdf](https://cdn.mediavalet.com/eunl/content/zknZRgZIdk-tAPjdS7cRgg/WDN5RjMomk62JQ93as4phg/Original/Methanex:%20Unlocking%20AI%E2%80%99s%20Potential%20with%20PI%20System%20Data%20&%20CONNECT:%20A%20Simplified,%20Scalable%20Approach.pdf)
13. [https://hostadvice.com/blog/ai/automation/n8n-vs-node-red/](https://hostadvice.com/blog/ai/automation/n8n-vs-node-red/)
14. [https://en.wikipedia.org/wiki/Node-RED](https://en.wikipedia.org/wiki/Node-RED)
15. [https://crosser.io/platform/features-and-pricing/](https://crosser.io/platform/features-and-pricing/)
16. [https://n8n.io](https://n8n.io/)
17. [https://www.crosser.io/articles/crosser-vs-node-red/](https://www.crosser.io/articles/crosser-vs-node-red/)
18. [https://pisquare.osisoft.com/s/Blog-Detail/a8r1I000000H73uQAC/pi-web-api-and-nodered](https://pisquare.osisoft.com/s/Blog-Detail/a8r1I000000H73uQAC/pi-web-api-and-nodered)
19. [https://revolutionpi.com/en/docs/node-red](https://revolutionpi.com/en/docs/node-red)
20. [https://nodered.org/docs/getting-started/raspberrypi](https://nodered.org/docs/getting-started/raspberrypi)
21. [https://www.aveva.com/en/perspectives/blog/unlocking-operational-excellence/](https://www.aveva.com/en/perspectives/blog/unlocking-operational-excellence/)
22. [https://www.reddit.com/r/nodered/comments/13po2wl/nodered_vs_n8n_how_do_they_compare/](https://www.reddit.com/r/nodered/comments/13po2wl/nodered_vs_n8n_how_do_they_compare/)
23. [https://osisoft.my.site.com/PISquare/s/question/0D51I00004UHmEHSA1/node-red-running-on-raspberry-send-to-pi](https://osisoft.my.site.com/PISquare/s/question/0D51I00004UHmEHSA1/node-red-running-on-raspberry-send-to-pi)
24. [https://crosser.io/partners/partner-pages/aveva/crosser-and-aveva/](https://crosser.io/partners/partner-pages/aveva/crosser-and-aveva/)
25. [https://cdn.osisoft.com/osi/presentations/2022-AVEVA-Amsterdam/UC22EU-D3WI030-AVEVA-Carasso-Integrating-Your-Operational-Data-Infrastructure.pdf](https://cdn.osisoft.com/osi/presentations/2022-AVEVA-Amsterdam/UC22EU-D3WI030-AVEVA-Carasso-Integrating-Your-Operational-Data-Infrastructure.pdf)
26. [https://www.pisolved.in/article/162/integrating-home-automation-and-plc-data-into-your-personal-pi-system-options-challenges-and-developer-tips](https://www.pisolved.in/article/162/integrating-home-automation-and-plc-data-into-your-personal-pi-system-options-challenges-and-developer-tips)
27. [https://www.aveva.com/en/perspectives/success-stories/methanex/](https://www.aveva.com/en/perspectives/success-stories/methanex/)
28. [https://latenode.com/blog/platform-comparisons-alternatives/n8n-alternatives/n8n-alternatives-2025-12-open-source-self-hosted-workflow-automation-tools-compared](https://latenode.com/blog/platform-comparisons-alternatives/n8n-alternatives/n8n-alternatives-2025-12-open-source-self-hosted-workflow-automation-tools-compared)
29. [https://blog.n8n.io/home-automation-with-raspberry-pi-and-n8n-an-interview-with-tephlon/](https://blog.n8n.io/home-automation-with-raspberry-pi-and-n8n-an-interview-with-tephlon/)
30. [https://techagency.com.au/n8n-raspberry-pi-automate-your-iot/](https://techagency.com.au/n8n-raspberry-pi-automate-your-iot/)
31. [https://techsupport.osisoft.com/Products/PI-Interfaces-and-PI-Connectors](https://techsupport.osisoft.com/Products/PI-Interfaces-and-PI-Connectors)
32. [https://thinkrobotics.com/blogs/software-programming/n8n-automation-tutorial-building-backend-workflows-for-iot-and-fleet-management](https://thinkrobotics.com/blogs/software-programming/n8n-automation-tutorial-building-backend-workflows-for-iot-and-fleet-management)
33. [https://docs.n8n.io/integrations/](https://docs.n8n.io/integrations/)
34. [https://community.n8n.io/t/how-to-setup-n8n-on-a-raspberry-pi-5-local-setup/120609](https://community.n8n.io/t/how-to-setup-n8n-on-a-raspberry-pi-5-local-setup/120609)
35. [https://www.youtube.com/watch?v=a1nY54_fyu0](https://www.youtube.com/watch?v=a1nY54_fyu0)
36. [https://n8n.io/integrations/evervault/and/personal-ai/](https://n8n.io/integrations/evervault/and/personal-ai/)
37. [https://community.n8n.io/t/n8n-installation-script-for-raspberry-pi-n8n-pi/1392](https://community.n8n.io/t/n8n-installation-script-for-raspberry-pi-n8n-pi/1392)
38. [https://hackers-arise.com/automating-your-digital-life-with-n8n/](https://hackers-arise.com/automating-your-digital-life-with-n8n/)
39. [https://www.reddit.com/r/SCADA/comments/1nqa8jz/which_remote_monitoring_solution_as_an_iiot/](https://www.reddit.com/r/SCADA/comments/1nqa8jz/which_remote_monitoring_solution_as_an_iiot/)
40. [https://tutoriels.lws.fr/vps/api-n8n-integrer-une-api-dans-un-n8n-auto%E2%80%91heberge](https://tutoriels.lws.fr/vps/api-n8n-integrer-une-api-dans-un-n8n-auto%E2%80%91heberge)
41. [https://smartbrain.io/landing/aveva-pi-system-integration](https://smartbrain.io/landing/aveva-pi-system-integration)