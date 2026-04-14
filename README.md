# StreamX + Adobe Experience Manager Template

This project demonstrates how to use **StreamX as a content delivery and rendering layer for AEM content**, with additional capabilities like search indexing.

The setup focuses on:

* generating **event-driven pages from AEM content**
* exposing content through the **delivery layer at the edge**
* indexing content in **StreamX Search**

---

## Overview

Content is authored in AEM and delivered to StreamX using the StreamX AEM Connector. StreamX then:

* generates **event-driven pages**
* exposes them via the **delivery layer at the edge**
* indexes content for search

---

## Integration with AEM

To connect AEM with StreamX, install the connector:

👉 [https://github.com/streamx-com/streamx-connector-aem](https://github.com/streamx-com/streamx-connector-aem)

### Configuration

After installing the connector on your AEM instance, configure the following environment variables:

```
STREAMX_CLIENT_URL=
STREAMX_CLIENT_AUTH_TOKEN=
```

### Where to get these values?

Both the **URL** and **auth token** are available in the StreamX Console.

For detailed setup instructions, refer to the connector repository.

---

## How it works

1. Content is created and managed in AEM
2. StreamX Connector sends content events to StreamX
3. StreamX:

   * generates **event-driven pages**
   * serves them through the **delivery layer at the edge**
   * indexes content for search
4. The final experience is delivered via the edge layer, not as static site output


