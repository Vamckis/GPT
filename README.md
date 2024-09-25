## GPT

### Setting Up ShellGPT
 - apt-get install git jq
 - export OPENAI_API_KEY= <Key from OpenAI>
 - export CHATGPT_KEY= <Key from Open AI>
 - pip install shell-gpt
 - pip install shell-gpt[litellm]

### Setting up Ollama
 - curl -fsSL https://ollama.com/install.sh | sh
 - ollama run llama3
 - If ollma dont run, execute: ollama serve
 - ollama list

### Modify ShellGPT configuration
 - nano ~/.config/shell_gpt/.sgptrc
`
DEFAULT_MODEL = ollama/llama3:latest
OPENAI_USE_FUNCTIONS = false
USE_LITELLM = true
`

 - Open-webUI:
`docker run -d --network=host -v open-webui:/app/backend/data -e OLLAMA_BASE_URL=http://127.0.0.1:11434 --name open-webui --restart always ghcr.io/open-webui/open-webui:main`

 - Install pyenv

### Prompt 
 - sgpt --shell "What is capital of India"
 - sgpt --interaction "What is my current system Ip address"
 - sgpt --code "Write basic HTML code for a web app"

### References:
- https://github.com/TheR1D/shell_gpt/wiki/Ollama
- https://rohanadhvaryu.medium.com/bwapp-buggy-web-application-web-app-setup-on-your-localhost-kali-linux-6d2dd49badbc
- https://github.com/nishantshah977/medium-free
- https://www.youtube.com/watch?v=WxYC9-hBM_g&list=LL&index=1
- https://medium.com/@docteur_rs/installing-privategpt-on-wsl-with-gpu-support-5798d763aa31
