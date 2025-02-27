# Coding Guidelines for AI-Driven Tenant Lead Identification System

## Code Structure and Organization
- Follow modular design principles with clear separation between:
  - Business logic (core algorithms and processing)
  - Data access (database and API interactions)
  - Presentation layer (API endpoints or UI)
- Use class-based organization for agents and components
- Implement dependency injection for better testability
- Keep modules focused on single responsibilities

## Python Style Guidelines
- Follow PEP 8 conventions
- Use Black formatting with a line length of 88 characters
- Include type hints for all function signatures
- Use Google-style docstrings for all modules, classes, and functions
- Avoid global variables and state when possible
- Use meaningful variable and function names that clearly indicate purpose

## Documentation Requirements
- All public functions and classes must have comprehensive docstrings
- Include examples in docstrings for non-trivial functions
- Document expected exceptions and error cases
- Maintain up-to-date architecture diagrams in `/docs`
- Provide clear instructions for local setup and testing

## Testing Standards
- Write unit tests for all business logic components
- Create integration tests for agent interactions
- Mock external API calls in tests
- Achieve minimum 85% code coverage
- Include performance tests for critical paths
- Test edge cases and failure scenarios

## Error Handling
- Use custom exception classes for domain-specific errors
- Implement proper logging with appropriate levels
- Validate all inputs at system boundaries
- Provide meaningful error messages
- Include context information in exceptions

## Performance Considerations
- Optimize token usage in LLM interactions
- Implement caching for expensive operations
- Use async operations for I/O-bound operations
- Batch database operations when possible
- Profile and optimize critical paths

## Security Standards
- Encrypt sensitive data at rest and in transit
- Use environment variables for secrets
- Implement proper authentication and authorization
- Validate and sanitize all user inputs
- Apply principle of least privilege

## GitHub Workflow
- Use feature branches for all changes
- Write descriptive commit messages following conventional commits
- Require tests to pass before merging
- Perform code reviews for all non-trivial changes
- Tag releases with semantic versioning

## AI Component Guidelines
- Include prompt templates in version control
- Document model parameters and versions used
- Validate AI outputs before using in critical operations
- Implement fallbacks for AI component failures
- Monitor token usage and implement safeguards against cost overruns
