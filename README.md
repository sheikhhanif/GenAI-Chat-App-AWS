## LLM based Chat App using AWS serverless

Here is the architecture of an LLM-based chatbot app using AWS services. The core features include:

- Secure Login: Utilizes AWS HTTP API Gateway for a safe and secure login process.
- WebSocket API Gateway: Establishes a persistent connection between the client and the backend for real-time interactions.
- Decoupled Chat Function: Uses AWS SNS to handle chat functions asynchronously. LLM API providers typically require more than 30 seconds to generate a response, which exceeds the HTTP API Gateway's 30-second timeout limit.
- Vector Store: RDS PostgreSQL database with PGVector for efficient data storage and retrieval.
- User Feedback Recording: Stores user feedback in an S3 bucket for analysis and improvement.

Feel free to use this architecture for your GenAI apps!
