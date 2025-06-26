+++
date = '2025-05-28T08:52:11+03:00'
draft = false
title = 'SpaceX ELT Pipeline'
description = "Designed a modular ELT pipeline to ingest and transform SpaceX launch data using Python, Singer, and dbt."
tags = ["Python", "Singer", "Snowflake", "dbt", "Airflow"]
+++

## What

I built a modular ELT pipeline that ingests SpaceX launch data from a public REST API and loads it into Snowflake. Data extraction is handled via a custom Singer tap, while dbt manages the downstream transformations and model orchestration.

## Why

I wanted to simulate a production-grade ingestion workflow using cloud-native tools. The goal was to sharpen my skills in building reliable, testable pipelines with clear separation between ingestion, transformation, and analytics layers.

## How

- Developed a custom Python-based Singer tap to extract launch data and manage incremental loads  
- Used dbt for staging, transforming, and testing data models inside Snowflake  
- Managed orchestration via Airflow to simulate a real deployment DAG  
- Ensured idempotency, handled flaky upstream responses, and logged pipeline metrics for observability

## Learnings

This project taught me the importance of small, composable tasks and early testing in pipeline design. I deepened my understanding of rate-limit management, schema evolution, and pipeline resiliency under real-world data conditions.

🔗 [View GitHub Repo](https://github.com/ivanovyordan/course-data-engineering-spacex)
