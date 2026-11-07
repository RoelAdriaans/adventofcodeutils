# Advent of Code Utils

This repository contains some utils used by my advent of code projects.

## Installation

Requires Python 3.14 or newer.

```shell
uv add git+https://github.com/RoelAdriaans/adventofcodeutils
```

## Usage

```python
from adventofcodeutils.queue import Queue
from adventofcodeutils.stack import Stack

q: Queue[int] = Queue()
q.push(1)
q.pop()
```

Available modules: `generic_search` (BFS/DFS), `graph`, `node`, `parsing`,
`point`, `priority_queue`, `queue` and `stack`.

## Development

```shell
uv sync                         # install dependencies
uv run pytest                   # tests
uv run ruff check src tests     # lint
uv run ruff format src tests    # format
uv run mypy src                 # type check
uv run pre-commit install       # enable git hooks
```
