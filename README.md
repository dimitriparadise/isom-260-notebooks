# ISOM 260 — Workshop Notebooks

Colab notebooks for **ISOM 260: AI for Business**, Suffolk University.

This repository is public for one reason: Colab's `Open in GitHub` loader can
only read public repositories. The course website that links to these notebooks
lives in a separate, private repository.

## Notebooks

| Session | Notebook | Open |
|---|---|---|
| 1 | Hello, Claude — API key setup and your first call | [Open in Colab](https://colab.research.google.com/github/dimitriparadise/isom-260-notebooks/blob/main/session-01/ISOM260_Session1_Hello_Claude.ipynb) |
| 3 | API Workshop — your first AI application | [Open in Colab](https://colab.research.google.com/github/dimitriparadise/isom-260-notebooks/blob/main/session-03/ISOM260_Session3_API_Workshop.ipynb) |
| 4 | Build Your First Agent (Claude) | [Open in Colab](https://colab.research.google.com/github/dimitriparadise/isom-260-notebooks/blob/main/session-04/ISOM260_Session4_Build_Your_First_Agent.ipynb) |
| 4 | Build Your First Agent (Gemini) | [Open in Colab](https://colab.research.google.com/github/dimitriparadise/isom-260-notebooks/blob/main/session-04/ISOM260_Session4_Build_Your_First_Agent_Gemini.ipynb) |
| 5 | Agents Meet the Real World (Claude) | [Open in Colab](https://colab.research.google.com/github/dimitriparadise/isom-260-notebooks/blob/main/session-05/ISOM260_Session5_Agents_Real_World.ipynb) |
| 5 | Agents Meet the Real World (Gemini) | [Open in Colab](https://colab.research.google.com/github/dimitriparadise/isom-260-notebooks/blob/main/session-05/ISOM260_Session5_Agents_Real_World_Gemini.ipynb) |
| 6 | Agent Patterns — ReAct and research agents | [Open in Colab](https://colab.research.google.com/github/dimitriparadise/isom-260-notebooks/blob/main/session-06/ISOM260_Session6_Agent_Patterns.ipynb) |
| 7 | Knowledge Agents — RAG | [Open in Colab](https://colab.research.google.com/github/dimitriparadise/isom-260-notebooks/blob/main/session-07/ISOM260_Session7_Knowledge_Agents_RAG.ipynb) |
| 7 | Homework — build your own knowledge agent | [Open in Colab](https://colab.research.google.com/github/dimitriparadise/isom-260-notebooks/blob/main/session-07/ISOM260_S7_Homework.ipynb) |
| 8 | Multi-Agent Systems — a three-stage pipeline | [Open in Colab](https://colab.research.google.com/github/dimitriparadise/isom-260-notebooks/blob/main/session-08/ISOM260_Session8_Multi_Agent_Systems.ipynb) |
| 8 | Research Agent | [Open in Colab](https://colab.research.google.com/github/dimitriparadise/isom-260-notebooks/blob/main/session-08/ISOM260_Session8_Research_Agent.ipynb) |

Sessions 9–11 have workshop notebooks planned but not yet written. The course
site marks them "coming soon" rather than linking to a missing file.

## API keys

Every notebook reads its key from Colab's secrets manager:

```python
from google.colab import userdata
api_key = userdata.get('ANTHROPIC_API_KEY')
```

Add the key once under the 🔑 icon in Colab's left sidebar and enable it for the
notebook. Never paste a key into a cell — a notebook keeps its output, and a
pasted key travels with any copy you share.

Get a key at [console.anthropic.com](https://console.anthropic.com); the Gemini
variants use [aistudio.google.com](https://aistudio.google.com/apikey).

## Editing

Colab opens these read-only. To change one for everybody:

1. Open it, edit, then **File → Save a copy in GitHub**, targeting this repo,
2. or edit the `.ipynb` locally and push.

Students working through them should use **File → Save a copy in Drive**, which
gives them their own editable copy and leaves this one untouched.

## Naming

Paths are `session-NN/`, matching the session numbering on the course site, so a
link on the site and a file here are easy to line up.
