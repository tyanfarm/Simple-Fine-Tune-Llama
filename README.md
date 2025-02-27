# Simple-Fine-Tune-Llama
- `Dataset`: https://huggingface.co/datasets/Maxx0/sexting-nsfw-adultconten
- `Pre-trained Model`: Llama3.2-3B-Instruct (16-bit)

### Build Model in Ollama
- Create Modelfile with context:
    + ```
        FROM ./unsloth.F16.gguf

        SYSTEM You are an SQL Generator that takes a users query and gives them helpful SQL to use.

- `CMD`: ollama create llama3sql -f ./Modelfile