# Email Processing Agent

An intelligent email processing agent built with LangGraph and OpenAI that:

1. Reads and analyzes incoming emails
2. Classifies emails as spam or legitimate
3. Categorizes legitimate emails (inquiry, complaint, etc.)
4. Drafts appropriate responses for review

## Features

- Smart spam detection with reason identification
- Email categorization
- Automated response drafting
- Workflow managed through LangGraph

## Requirements

- Python 3.8+
- OpenAI API key
- Required packages: langgraph, langchain, langchain_openai

## Setup

1. Clone the repository
2. Install dependencies
3. Set your OpenAI API key
4. Run the agent with `python email-agent.py`

## Architecture

The agent uses a directed graph workflow with nodes for:
- Reading emails
- Classifying content
- Handling spam
- Drafting responses
- Notifying the user 