# ollama-openwebui

This project will allow you to run a docker container for both the ollama LLM API framework as well as an Open WebUI container client to interact with LLM API. 

Dependency: 

You will need Docker and Docker Compose installed.

If utilizing a NVidia GPU and you desire to utilize CUDA acceleration, you will need to install the Nvidia container toolkit:

https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/install-guide.html#installation

To start:

1. Run `./local-bin/start` from within the working cloned directory. 
2. Pull desired ollama model (https://ollama.com/search). 
  - We recommend `llama3.2:1b` since it will run on most machines. 
  - Better GPUs will allow for larger models.
  - `docker exec -it ollama ollama pull llama3.2:1b` 
3. Open web browser to the Open WebUI application.
  - `http://localhost:3035`
4. Create an account in the UI.
5. Once logged into the Open WebUI, select the model `llama3.2:1b` (or whatever you pulled) from the drop-down in the top-left.
6. Start Chating with llama!
7. Visit the Ollama and Open WebUI documentaiton sites for more information and resources:
  - Ollama: https://ollama.com/
  - Ollama models search: https://ollama.com/search
  - Ollama Github: https://github.com/ollama/ollama
  - Ollama Docker Hub: https://hub.docker.com/r/ollama/ollama
  - Open Webui: https://openwebui.com/
  - Open WebUI (Docs): https://docs.openwebui.com/
  - Open Webui Github: https://github.com/open-webui/open-webui
  - Open WebUI Docker Hub: https://docs.openwebui.com/