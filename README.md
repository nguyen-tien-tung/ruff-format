# ruff.toml

line-length = 100
indent-width = 4

[format]
quote-style = "single"
indent-style = "space"
docstring-code-format = true

[lint]
select = ["E","F","UP","B","SIM","I","N","C4","PYI","TID","TCH","ARG","W"]

[lint.flake8-bugbear]
extend-immutable-calls = ["fastapi.Depends", "fastapi.params.Depends", "fastapi.Query", "fastapi.params.Query", "fastapi.Security", "fastapi.params.Security"]
