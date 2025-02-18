## Langchain-python

Langchain example from [quickstart](https://python.langchain.com/en/latest/getting_started/getting_started.html).

To interact with langchain, you can just set the `OPENAI_API_BASE` URL and provide a token with a random string.

See the example below:

```
# Clone LocalAI
git clone https://github.com/go-skynet/LocalAI

cd LocalAI/examples/langchain-python

# (optional) Checkout a specific LocalAI tag
# git checkout -b build <TAG>

# Download gpt4all-j to models/
wget https://gpt4all.io/models/ggml-gpt4all-j.bin -O models/ggml-gpt4all-j

# start with docker-compose
docker-compose up -d --build


pip install langchain
pip install openai

export OPENAI_API_BASE=http://localhost:8080
export OPENAI_API_KEY=sk-

python test.py
# A good company name for a company that makes colorful socks would be "Colorsocks".
```