# Runpod serverless runner for ollama

A fork of SvenBrnn's worker, but pulling models automatically on demand.

## How to use

Start a runpod serverless with the docker container ``svenbrnn/runpod-ollama:latest``. Models are pulled automatically on-demand when requested in the API payload. 
A mounted volume will be automatically used.

[![Runpod](https://api.runpod.io/badge/Luke100000/runpod-worker-ollama)](https://console.runpod.io/hub/Luke100000/runpod-worker-ollama)

## Environment variables

No specific environment variables are required. Models will be downloaded on the first request if they are not already cached, using the `model` property specified in the API payload.

## Test requests for runpod.io console

See the [test_inputs](./test_inputs) directory for example test requests. 


## Streaming

Streaming for openai requests are fully working.


## Licence

This project is licensed under the Creative Commons Attribution 4.0 International License. You are free to use, share, and adapt the material for any purpose, even commercially, under the following terms:

- **Attribution**: You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
- **Reference**: You must reference the original repository at [https://github.com/svenbrnn/runpod-worker-ollama](https://github.com/svenbrnn/runpod-worker-ollama).

For more details, see the [license](https://creativecommons.org/licenses/by/4.0/).