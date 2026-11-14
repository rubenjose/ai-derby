# AI Derby

AI models race over fences, and every fence is a question. The films, the results, and a record of each race that anyone can check.

This repo is the site. It is built from the races; nothing here is edited by hand.

## The records

`records/` holds one file per race: the questions, each answer exactly as the model wrote it, how it was marked, and the settings the race ran under. The fingerprint (SHA-256) of each:

| Race | Record | SHA-256 |
| --- | --- | --- |
| The One-Line Chase | [records/creative.json](records/creative.json) | `ba3c84e85dbcd34e417c8e8f7102109d3744e6c65132d70865fd8b082c6752df` |
| The Ledger Stakes | [records/retrieval.json](records/retrieval.json) | `138a6b8f934b357940549a99e93c36c9edadd0cf4f782bfd2ef4b36b5e07c63f` |
| The Abacus Handicap | [records/reasoning.json](records/reasoning.json) | `8c0739480a06a1370ce742493835b86927b1e624501a8ced04978f609759a0c3` |
| The Order Book Chase | [records/json.json](records/json.json) | `a90dd8fae40888c1df383cb2182c7eda6ba57b91060577d1acba18cdf315cc1e` |
| The Order Book Gold Cup | [records/goldcup.json](records/goldcup.json) | `8da62e99f2e2d42c5e37fca4ef269304233e81f3352279dd7f655e6a499d9374` |

To check one: `shasum -a 256 records/creative.json`. The history of this folder shows when each record was published and that none has changed since.
