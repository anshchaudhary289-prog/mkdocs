# Command Line Interface

::: mkdocs-click
    :module: mkdocs.__main__
    :command: cli
    :prog_name: mkdocs
    :style: table
    :list_subcommands: true

## Troubleshooting

### `mkdocs serve` fails with `OSError: [Errno 98] Address already in use`

This means that another process is already listening on the address
that `mkdocs serve` tries to use (by default `localhost:8000`). Either
stop the other process, or serve on a different address with `-a`:

```bash
mkdocs serve -a 127.0.0.1:8001
```
