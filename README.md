# n8n_NaturalQueryAgent

#  Natural Language - to - SQL Query Agent

## Overview
This project implements an AI-powered analytics agent that converts natural language business questions into accurate PostgreSQL queries and executes them on a real analytics database.

This system is designed to bridge the gap between business users and analytical databases by eliminating the need for manual SQL writing. It uses an AI agent to interpret the intent behind natural language questions and map them to the correct fact and dimension tables within a star-schema PostgreSQL database. The agent is constrained to use database execution tools, ensuring that all responses are derived from real data rather than generated assumptions. 

Workflow orchestration is handled using n8n, which manages user input, AI reasoning, SQL execution, and response delivery in a controlled sequence. Each generated query is validated through direct database execution, ensuring accuracy and reliability of analytical results. This approach demonstrates how AI can be safely integrated into data workflows to support trustworthy decision-making.

## What It Does
- Accepts plain English analytics questions
- Converts them into SQL using a schema-aware AI agent
- Executes queries on PostgreSQL
- Returns verified, real-time results

## Tech Stack
- PostgreSQL (Supabase)
- n8n (Workflow Automation)
- Google Gemini LLM
- Star Schema Data Model

## Example Queries
- Sales quantity for India in 2020
- Sales quantity for India in 2019
- Country with highest sales

## Validation
All AI-generated outputs were validated by executing the equivalent SQL queries directly in PostgreSQL.

## Artifacts
- n8n workflow export
- Architecture documentation
 
