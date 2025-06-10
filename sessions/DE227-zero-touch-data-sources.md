# Creating Data Pipelines with Zero Touch, DE227

https://reg.summit.snowflake.com/flow/snowflake/summit25/sessions/page/catalog/session/1738698785269001rA2y

- **Date**: June 2, 2025
- **Time**: 13:00 - 13:45
- **Location**: Room 157 (Moscone South, Upper Mezzanine)
- **Session Code**: DE227

> In response to the growing demand for integrating new data into our data platform, the Data Engineering Team at Okta has developed a solution utilizing Snowpark for Python to automate construction of data pipelines. Discover how Okta's Zero Touch Platform creates end-to-end pipelines that ingest events arriving on S3 and transforms data in Snowflake using Streams and Tasks. The platform features integrated capabilities to detect schema changes in data streams, facilitating automatic evolution of Snowflake table schemas. Crafted with privacy in mind, it also allows for data classification through tags and systemically masking data using tag-based masking policies.

## Overview

Session about creating data pipelines with zero touch automation using Snowpark for Python.

## Key Points

- Zero touch data onboarding
- The old way: manual data onboarding, each team owns a section of the pipeline
- Schemas defined by teams closest to the data (shift left)
- Protobuf-driven schemas
- Ad-hoc processes handle backfill
- Protobuf change initiates versioned release, update actions for queue
- Can override default types or transformations
- Context-aware types - e.g., user ID types automatically hashed
- Data quality checks prevent bad data from propagating through system
