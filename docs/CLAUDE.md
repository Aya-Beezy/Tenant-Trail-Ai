# Tenant Trail AI Project Guide

## Communication Preferences
- Explain concepts in beginner-friendly terms with clear explanations
- Provide context and reasons behind technical recommendations
- Break down complex ideas into simpler steps
- Avoid assuming prior knowledge of programming concepts

## Project Information
- Project: AI-Driven Tenant Lead Identification System
- Path: /Users/bharat/Library/CloudStorage/GoogleDrive-bharat.singh@sitacltd.com/My Drive/Non Pvt/SITAC Group/Berlin/Tenant Marketing/Tech Outreach/Tenant Trail Ai

## Project Overview
This system autonomously identifies, qualifies, and facilitates outreach to businesses showing expansion or relocation signals by monitoring diverse data sources. It uses specialized agents for different source types and enhanced data processing capabilities.

## Architecture
The system employs a hybrid architecture combining:
- **CrewAI**: Source-specialized agent teams with domain expertise
- **LangGraph**: Workflow control and complex reasoning chains
- **ChromaDB**: Intelligent document storage and semantic retrieval
- **LlamaIndex**: Advanced document processing and PDF/image analysis
- **Instructor/Pydantic**: Structured data extraction with validation

## Key Components
1. Source-Specialized Signal Detection (13 dedicated agent teams)
2. Advanced Context Management (vector-based semantic memory)
3. Multi-Step Signal Validation (cross-source correlation)
4. Structured Data Extraction (Pydantic models)
5. Automated Outreach Orchestration (template-based communication)

## Implementation Details
- Source-specific agents for different signals (funding, press releases, job openings, etc.)
- Structured Pydantic models for data extraction
- Processing flow: Signal → Extraction → Qualification → Prioritization → Outreach
- Technology stack includes Docker/Kubernetes, PostgreSQL, Redis, RabbitMQ, N8N, Jaeger

## Coding Guidelines
- PEP 8 conventions
- Black formatting (88 character line length)
- Type hints required
- Google-style docstrings
- 85% minimum code coverage
- Async operations for I/O-bound tasks
- Feature branches and descriptive commit messages

## Useful Commands
- To be added as needed (build commands, run commands, etc.)

## Project Structure
- config/ - Configuration files
- docs/ - Documentation (including architecture diagrams)
- src/ - Source code
- tests/ - Test files (unit tests, integration tests)

## Development Priorities
1. Signal detection from diverse sources
2. Cross-validation to minimize false positives
3. Lead scoring and prioritization
4. Human-in-the-loop review capability
5. Continuous learning from results

## Security Standards
- Environment variables for secrets
- Proper authentication and authorization
- Input validation and sanitization
- Principle of least privilege

## AI Component Guidelines
- Include prompt templates in version control
- Document model parameters and versions
- Validate AI outputs for critical operations
- Implement fallbacks for AI component failures
- Monitor token usage with cost safeguards