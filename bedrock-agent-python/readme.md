# Hosted Agent

To run the Agent on `http://localhost:8000`

```bash
python3 my-agent.py
```

Then you can send it an invocation:

```bash
curl -X POST http://localhost:8000/invocations \
  -H "Content-Type: application/json" \
  -d '{"prompt":"EC2"}'
```

## Next Steps

agentcore instructions to have the file:
- Docker file created and .yaml manifest
- Zipped
- Uploaded to S3
- CodeBuild to Container, hosted on ECR
- Deployed to Bedrock Agent Core runtime