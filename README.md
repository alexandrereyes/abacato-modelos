# Modelos do Abacato

Espelho dos modelos que o app Abacato baixa no aparelho. Cada release é uma versão de um modelo, publicada como release imutável: os arquivos de uma versão nunca mudam, e uma versão nova é outra release.

## kroko-pt-d0472d06

Reconhecimento de fala em português, streaming (Zipformer2 transducer, ONNX), para sherpa-onnx.

Endereço-base: `https://github.com/alexandrereyes/abacato-modelos/releases/download/kroko-pt-d0472d06/`

| Arquivo | Bytes | SHA-256 |
| --- | ---: | --- |
| `encoder.onnx` | 154878660 | `336b9a62fd37d8b94855fcbe0414000aa5f1bd75d4cb907e112bd6b7ef97c52e` |
| `decoder.onnx` | 617488 | `2380832dbb1867779a550aea3948776d6a53ffa1cccd075bb7592ebaf21b7638` |
| `joiner.onnx` | 336817 | `de7afbc23e7e55af7fed85780690b8f883c62b881fe14d546d9677151581962f` |
| `tokens.txt` | 6239 | `ff7e774b59714285d211a524223885fd9884cb878af97635d10042f56dbc56cd` |

### Origem

O modelo é o **Kroko PT Community 64 L Streaming 001**, da Kroko ASR (Banafo), publicado em <https://huggingface.co/Banafo/Kroko-ASR> como `Kroko-PT-Community-64-L-Streaming-001.data` (155839360 bytes, SHA-256 `36c4a92f25c9243cbd8f007cfc624b09986debf2919a1e397891e62e063d0e61`).

Esse arquivo é um contêiner: um cabeçalho JSON e, em seguida, o encoder, o decoder, o joiner e o vocabulário, cada um precedido do seu tamanho. Os quatro arquivos daqui são fatias exatas dele, sem nenhuma alteração nos bytes (o `tokens.txt` mantém os 4 bytes de tamanho do início). Foram obtidos de <https://huggingface.co/kouhxp/sherpa-onnx-streaming-zipformer-pt-kroko> (revisão `d0472d0660a2f6040132e42da37d6906368bcbb7`), onde alguém os separou assim, e conferidos byte a byte contra o arquivo oficial.

### Licença e atribuição

Os modelos Community da Kroko são licenciados pela Kroko ASR (Banafo) sob **CC BY-SA** (Creative Commons Atribuição-CompartilhaIgual), conforme <https://huggingface.co/Banafo/Kroko-ASR>, <https://github.com/kroko-ai/kroko-onnx> e <https://docs.kroko.ai/on-premise/>. A versão da licença não é indicada pelo autor; a versão atual é a 4.0: <https://creativecommons.org/licenses/by-sa/4.0/>.

> "Kroko PT Community 64 L Streaming 001", de Kroko ASR (Banafo), <https://huggingface.co/Banafo/Kroko-ASR>, licenciado sob CC BY-SA. Redistribuído sem alterações no conteúdo, apenas separado do contêiner `.data` original em arquivos ONNX.

Estes arquivos continuam sob a mesma licença CC BY-SA. Este repositório não concede nenhum direito além dela.
