# Amazon Bedrock Agents Observability with Phoenix/Arize AI

A guide for setting up comprehensive observability for Amazon Bedrock Agents using Phoenix/Arize AI to monitor input messages, LLM thought processes, tool invocations, and final results.

## Overview

This repository provides instructions and code examples for integrating Phoenix/Arize AI observability with Amazon Bedrock Agents. Phoenix/Arize AI offers detailed tracing capabilities that allow you to monitor your agent's complete workflow, including internal reasoning and tool usage.

## Quick Start

### Prerequisites

- AWS Account with appropriate permissions
- SageMaker Notebook Instance (recommended)
- IAM Role with `BedrockFullAccess` permissions

### Setup Instructions

1. **Create SageMaker Environment**
   - Launch a SageMaker Notebook Instance
   - Ensure the instance has an IAM Role with `BedrockFullAccess`

2. **Install and Configure Phoenix**
   - Use the provided Jupyter Notebook: `phoenix_arize_ai_agent_logging.ipynb` (remove .txt extension)
   - Follow the Notebook Option to Launch Phoenix from the setup guide
   - Run the cells to initialize your environment

3. **Access Dashboard**
   - After running the notebook, navigate to the locally hosted Phoenix app dashboard
   - The link will be displayed in the notebook output
   - View comprehensive traces including inputs, outputs, LLM thinking processes, and tool calls

## Features

Phoenix/Arize AI integration provides visibility into:

- **Input Messages**: Complete request data sent to your Bedrock Agent
- **LLM Thought Processes**: Internal reasoning and decision-making steps
- **Tool Invocations**: Function calls and external API interactions
- **Final Results**: Complete response data and outcomes
- **Performance Metrics**: Latency, token usage, and error tracking

## Files Included

- `phoenix_arize_ai_agent_logging.ipynb` - Complete setup notebook with working code examples
- `phoenix_arize_ai_dashboard.png` - Example dashboard screenshot showing trace visualization

## Production Considerations

For production deployments, consider these additional integration options:

- **Strands Agents SDK**: Enhanced integration capabilities for enterprise environments
- **CrewAI Framework**: Multi-agent orchestration with observability
- **Custom Integration**: Direct API integration for specific use cases

## Bedrock AgentCore Support

Phoenix/Arize AI supports integration with Bedrock AgentCore through compatible frameworks like Strands and CrewAI. While direct AgentCore integration documentation is limited, the underlying frameworks provide the necessary connectivity.

## Important Notes

⚠️ **Third-Party Solution**: Phoenix/Arize AI is maintained by Arize, not AWS. Integration capabilities and feature support may vary.

- AWS has limited visibility into Phoenix's internal workings
- For detailed technical support, contact Arize AI/Phoenix developers directly
- Integration levels between Phoenix and different Bedrock features may vary

## Useful Resources

- [Amazon Bedrock Agents Tracing Documentation](https://arize.com/docs/phoenix/integrations/llm-providers/amazon-bedrock/amazon-bedrock-agents-tracing)
- [AWS Blog: Amazon Bedrock Agents Observability using Arize AI](https://aws.amazon.com/blogs/machine-learning/amazon-bedrock-agents-observability-using-arize-ai/)
- [AWS Blog: Observing AI Agentic Workflows with Strands Agents SDK and Arize AX](https://aws.amazon.com/blogs/machine-learning/observing-and-evaluating-ai-agentic-workflows-with-strands-agents-sdk-and-arize-ax/)

## Getting Help

If you encounter issues during setup:

1. Check the provided notebook for working code examples
2. Verify your IAM permissions include Bedrock access
3. Consult the official Phoenix/Arize AI documentation
4. Contact AWS Support for Bedrock-specific questions
5. Reach out to Arize AI support for Phoenix-specific issues

## Contributing

Feel free to submit issues and enhancement requests. When reporting problems, please include:

- Your current environment setup
- Specific error messages
- What you're trying to achieve
- Steps you've already attempted

---

*This guide is based on successful implementation examples and AWS Premium Support recommendations. Results may vary based on your specific use case and environment configuration.*
