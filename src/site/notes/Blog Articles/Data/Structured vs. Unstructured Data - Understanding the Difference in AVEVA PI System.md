---
{"dg-publish":true,"tags":["OperationalData","TechInsider","TechComparison"],"permalink":"/blog-articles/data/structured-vs-unstructured-data-understanding-the-difference-in-aveva-pi-system/","dgPassFrontmatter":true}
---

In the world of industrial data management, understanding the difference between structured and unstructured data is crucial for effective data handling and analysis. As AVEVA PI System users, it's essential to grasp these concepts to maximize the value of your data. Let's dive into the key differences and their implications for PI System users.

![](https://i.imgur.com/9nc3G11.png)

## Structured Data
Structured data follows a predefined format and organization, making it easily readable and processable by machines[1]. In the context of AVEVA PI System, structured data is typically stored in the PI Data Archive and includes:
- Time-stamped process variables (PI Points)[2]
- Asset attributes in PI Asset Framework (AF)[2]
- Predefined data types such as Boolean, Byte, and DateTime[4]

Structured data in PI System is organized in a tabular format, with each column representing an attribute (e.g., time, temperature, pressure) and each row containing a single record with associated values[1][2].

## Unstructured Data
Unstructured data lacks a predefined data model or schema, making it more complex to organize and analyze[1][3]. In industrial settings, unstructured data may include:
- Maintenance logs
- Operator notes
- Equipment manuals
- Images and videos of plant operations
- Audio recordings from control rooms

While PI System primarily deals with structured data, it can also handle some forms of unstructured data through its Asset Framework (AF) and PI Vision capabilities[2].

## Key Differences

![](https://i.imgur.com/M4pTlsh.png)

1. **Data Format**: Structured data in PI System adheres to specific formats like PI Points and AF attributes, while unstructured data comes in various formats such as text documents, images, and audio files[1][7].
2. **Storage**: Structured data is efficiently stored in the PI Data Archive, optimized for quick retrieval. Unstructured data may be stored in file systems or linked to AF elements as external references[2].
3. **Querying and Analysis**: Structured data in PI System can be easily queried and analyzed using tools like PI Vision and PI DataLink. Unstructured data often requires more advanced techniques for meaningful analysis[5].
4. **Data Volume**: While structured data in PI System is compact and efficient, unstructured data typically requires more storage space and grows at a faster rate[5].
5. **Integration**: PI System excels at integrating structured data from various sources (PLCs, DCS, SCADA) into a unified data model. Integrating unstructured data may require additional tools or custom solutions[2].

## Leveraging Both Data Types in AVEVA PI System
To maximize the value of both structured and unstructured data:
1. Use PI Asset Framework to create a comprehensive asset model that incorporates both structured (PI Points) and unstructured (document links, notes) data[2].
2. Utilize PI Vision to create dashboards that combine structured data visualizations with links to relevant unstructured data sources[2].
3. Implement data contextualization strategies to add structure to unstructured data, making it more searchable and analyzable within the PI System ecosystem.
4. Consider integrating advanced analytics tools that can process both structured and unstructured data to gain deeper insights from your industrial data.

By understanding and effectively managing both structured and unstructured data, AVEVA PI System users can create a more comprehensive and insightful view of their industrial operations, leading to better decision-making and improved operational efficiency.

<u>Citations:</u>
[1] https://aws.amazon.com/compare/the-difference-between-structured-data-and-unstructured-data/
[2] http://cdn.osisoft.com/learningcontent/pdfs/VisualizingPISystemDataWorkbook.pdf
[3] https://www.datamation.com/big-data/structured-vs-unstructured-data/
[4] https://docs.aveva.com/bundle/pi-server-l-af-pse/page/1020031.html
[5] https://www.integrate.io/blog/structured-vs-unstructured-data-key-differences/
[6] https://docs.aveva.com/bundle/pi-interface-for-opc-da/page/1010893.html
[7] https://www.altexsoft.com/blog/structured-unstructured-data/
[8] https://docs.aveva.com/bundle/pi-server-l-builder/page/1022629.html
[9] https://www.ibm.com/think/topics/structured-vs-unstructured-data
