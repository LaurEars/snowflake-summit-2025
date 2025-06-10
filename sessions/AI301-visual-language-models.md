# Build and Deploy Visual Language Models for Unstructured Data Processing

https://reg.summit.snowflake.com/flow/snowflake/summit25/sessions/page/catalog/session/1738696971970001xUxj

[Session lab account](https://go.dataops.live/summit25-unstruct-data-process)

[Quickstart link](https://quickstarts.snowflake.com/guide/extracting-insights-from-video-with-multimodal-ai-analysis)

- **Date**: June 5, 2025
- **Time**: 10:00 - 11:30
- **Location**: Hands-on Labs 3101 (Basecamp, North)
- **Session Code**: AI301

> In this hands-on lab, you’ll deploy visual language models (VLMs) using Snowpark containers to process unstructured, multi-modal data such as images and videos. Learn how VLMs enhance AI assistants and RAG workloads by extracting meaningful insights from these types of complex data. We will review best practices for deploying VLMs in Snowflake, managing governance, and integrating AI-driven image analysis into enterprise workflows. By the end of the session, you’ll have a fully functional VLM-powered pipeline that processes images and generates intelligent insights — all securely within Snowflake.

## Overview

Hands-on lab session about building and deploying visual language models for unstructured data processing.

## Lab Exercises

- Using Qwen for video
- `CORTEX.AI_TRANSCRIBE` for audio
- [Git repo](https://github.com/Snowflake-Labs/sfguide-extracting-insights-from-video-with-multimodal-ai-analysis/)
- "Compute pool like a warehouse but for running container services"
- Image has been pre-uploaded to Snowflake account
- Used Snowflake UI to upload raw files via stage instead of workspace code
- `EXECUTE JOB SERVICE` spins up containerized worker (Qwen)
- Can see status and container states in `Projects/Services and Jobs` menu in Snowflake UI
- AI transcription is in Snowflake private preview
- Video/audio/slides steps can be done in parallel

## Code Snippets

```snowflake
-- to get repository URL for the service yaml
SHOW IMAGE REPOSITORIES IN SCHEMA spcs_db.public;
-- to get tags and image path
SHOW IMAGES IN IMAGE REPOSITORY spcs_db.public.model_repo;
-- then combine and put into image yaml
-- example image: sfsehol-summit25-unstruct-data-process-jfrfsg.registry.snowflakecomputing.com/spcs_db/public/model_repo/model_analysis:v0.1
```
