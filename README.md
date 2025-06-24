## Prepare the environment

```bash
cd src
dapr init
pip install dapr-agents
pip install -r requirements.txt
```

## Create a .env file with the following content:

```bash
AZURE_OPENAI_API_KEY="<your-azure-openai-api-key>"
AZURE_OPENAI_ENDPOINT="<your-azure-openai-endpoint>"
AZURE_OPENAI_DEPLOYMENT="gpt-4.1"
AZURE_OPENAI_API_VERSION="2024-12-01-preview"
DAPR_LLM_COMPONENT_DEFAULT="openai"
MINECRAFT_SERVER="<your-minecraft-server>"
```

## Run the demos

```bash
dapr run -f dapr.yaml
```