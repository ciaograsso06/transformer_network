# Transformer Network

Este repositório contém a implementação de uma rede Transformer para classificação de textos. O modelo utiliza embedding, codificação posicional e camadas de atenção multi-head para processar os dados.

## Estrutura do Repositório

```
Transformer_Network/
│-- model/                      
│-- notebook/Transformer.ipynb                                 
│-- README.md                  
```

## Dependências

Instale os pacotes necessários executando:
```bash
pip install -r requirements.txt
```

## Treinamento do Modelo

Para treinar o modelo, execute:
```bash
python train.py
```

Isso irá carregar os dados, treinar o modelo e salvá-lo no diretório `model/`.

## Inferência

Após o treinamento, você pode testar o modelo executando:
```bash
python inference.py "Seu texto aqui"
```

## Estrutura do Modelo

O modelo consiste nas seguintes camadas:
- **Embedding Layer:** Converte palavras em vetores de tamanho fixo.
- **Positional Encoding:** Adiciona informações de posição aos embeddings.
- **Multi-Head Attention Layers:** Permite que o modelo capture relações contextuais entre palavras.
- **Feed-Forward Layers:** Processa as saídas da atenção.
- **Output Layer:** Camada final para prever a classe do texto.

## Salvamento do Modelo

O modelo treinado é salvo no formato `.keras` dentro do diretório `model/`:
```python
model.save("model/transformer_imdb_model.keras")
```

## Contribuição

Sinta-se à vontade para contribuir enviando pull requests ou abrindo issues.

## Licença

Este projeto está sob a licença MIT.

