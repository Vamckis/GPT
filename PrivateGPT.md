### Ollama
- curl -fsSL https://ollama.com/install.sh | sh
- ollama run llama2

## Installing PrivateGPT on wsl

### Prerequisites
- sudo apt-get update
- sudo apt-get upgrade
- sudo apt-get install build-essential

### CLoning PrivateGPT repo
- git clone https://github.com/imartinez/privateGPT

### Setting up Python Environmnet
- sudo apt-get install git gcc make openssl libssl-dev libbz2-dev libreadline-dev libsqlite3-dev zlib1g-dev libncursesw5-dev libgdbm-dev libc6-dev zlib1g-dev libsqlite3-dev tk-dev libssl-dev openssl libffi-dev
- curl https://pyenv.run | bash
- export PATH="/home/$(whoami)/.pyenv/bin:$PATH"

#### Add below lines in .bashrc file
` 
export PYENV_ROOT="$HOME/.pyenv"
[[ -d $PYENV_ROOT/bin ]] && export PATH="$PYENV_ROOT/bin:$PATH"
eval "$(pyenv init -)"
`

#### Reload terminal
- source .bashrc

### Install pyenv resources
sudo apt-get install lzma
sudo apt-get install liblzma-dev

### Insta;; pyenv 3.11
- pyenv install 3.11
- pyenv global 3.11
- pip install pip --upgrade
- pyenv local 3.11

### Install poetry to manage dependencies:
- curl -sSL https://install.python-poetry.org | python3 -
#### Add below line in .bashrc
` 
export PATH="/home/vamc/.local/bin:$PATH"
`
- source  .bashrc
- 
