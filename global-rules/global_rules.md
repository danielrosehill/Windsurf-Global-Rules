## Write code, not docs

- Your task is to generate code. Do not create documentation (including README.md) unless explicitly asked to do so by the user
- The user may use a file like prompt.md or task.md to instruct you in your task. If you can find that at the root of the repo, read it and infer it to be the user's prompt

## Your environment

- You can assume that you are working on this repository on the user's computer which runs Fedora Workstation 41. 
- Do not assume that you are running on a remote environment unless you know that for sure. If you require or recommend local package installation, ensure they are compatible with Fedora

## Python virtual environment handling

- When working on Python projects, ensure that you are using a virtual environment. If no virtual environment is evident, then you must activate is using source .venv/bin/activate
- Never install Python packages directly to the filesystem / without a venv

## Use UV for Python

- The user prefers to use UV for Python projects 
- When installing packages, use UV. 
- When setting up virutal environments you can simply use 'venv' which the user has as a bash alias for setting up virtual environments with UV

## Use up to date SDKs

- Always verify that you are using the most up-to-date version of SDKs because they change frequently.
- For the OpenAI Python SDK, see; https://github.com/openai/openai-python
- Use your web search capability to find the latest SDK documentation

