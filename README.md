# ChatGPT-cli

ChatGPT Natural language Command Line Interface

## Quick Setup

1. Setup virtual environment and install `source .venv/bin/activate && pip install -e .`
2. Register for an account on OpenAI https://beta.openai.com
3. Create API key at https://beta.openai.com/account/api-keys'
4. Add key to shell config so for zshell `echo export OPENAI_API_KEY=NEW_KEY >> ~/.zshrc`
5. bin/chatgpt PROMPT

## Example Use Cases

```
$ bin/chatgpt git log pretty
>>> Run:  git log --pretty=format:"%h %ad | %s%d [%an]" [y/N]: y
$ git log --pretty=format:"%h %ad | %s%d [%an]"

$  bin/chatgpt set kubernetes namespace
>>> Run:  kubectl config set-context default --namespace=kube-system [y/N] y
$ kubectl config set-context default --namespace=kube-system

$  bin/chatgpt exec into the docker image called foobar
>>> Run:  docker exec -it foobar bash [y/N]: y
$ docker exec -it foobar bash
```

## Background

Simple cli wrapper for OpenAI's ChatGPT which was created from the Natural Language shell tutorial https://openai.com/blog/openai-api/

Last 15 lines from /Users/paulwilson/Library/Logs/Homebrew/chatgpt/20.pip:
/opt/homebrew/Cellar/chatgpt/0.2.0/libexec/bin/pip
install
-v
--no-deps
--no-binary
:all:
--use-feature=no-binary-enable-wheel-cache
--ignore-installed
/private/tmp/chatgpt-20230505-73454-na7ccp/chatgpt-cli-0.2.0

Using pip 23.0.1 from /opt/homebrew/Cellar/chatgpt/0.2.0/libexec/lib/python3.10/site-packages/pip (python 3.10)
ERROR: Directory '/private/tmp/chatgpt-20230505-73454-na7ccp/chatgpt-cli-0.2.0' is not installable. Neither 'setup.py' nor 'pyproject.toml' found.

[notice] A new release of pip is available: 23.0.1 -> 23.1.2
[notice] To update, run: python3.10 -m pip install --upgrade pip

Do not report this issue to Homebrew/brew or Homebrew/homebrew-core!

Error: Your Xcode (14.2) is outdated.
Please update to Xcode 14.3 (or delete it).
