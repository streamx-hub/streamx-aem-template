# StreamX + Adobe Experience Manager Template

This project demonstrates how to use **StreamX as a static site generator** for content managed in AEM, with additional capabilities like search indexing.

The setup focuses on:

* generating **static pages from AEM**
* indexing content in **StreamX Search**

---

## Overview

Content is authored in AEM and delivered to StreamX using the StreamX AEM Connector. StreamX then:

* generates static pages
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
2. StreamX Connector sends content to StreamX
3. StreamX:

    * generates static pages
    * indexes content for search
4. The final site is served as a static website


