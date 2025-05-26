# Cloud-powered-AI-Agent-for-Business-Assistance
This is a helpful agent which can be used to compute the daily revenue of a retail store
# Tech stack
Amazon bedrock,Lambda,Nova-Micro 1.0
# Architecture
This project uses Amazon Bedrock and Manus AI Agents to build a serverless Business Assistant that can answer business-related queries and optionally perform actions via AWS Lambda.

💡 Workflow:
User Query
A user sends a business-related request (e.g., "Show me today's sales summary").

Manus Agent (Amazon Bedrock)
The Manus agent receives the query and interprets the intent using a foundation model like Anthropic Claude Instant or Amazon Nova-Micro 1.0.

Agent Instructions + Actions

The agent follows predefined instructions to decide whether to respond directly or call an action.

If needed, it invokes an AWS Lambda function (e.g., to fetch sales data from a database).

Lambda Function
The Lambda function performs the business logic (e.g., querying DynamoDB) and returns the result to the agent.

Response
The agent formats the final response and sends it back to the user.

![Screenshot 2025-05-26 141559](https://github.com/user-attachments/assets/71785799-11c4-4fe7-b511-ac52e0c1dce2)

