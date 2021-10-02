# Minetest API Types

This project adds type definitions for the [Minetest Modding API](https://github.com/minetest/minetest/blob/master/doc/lua_api.txt)

Requires an IDE with [EmmyLua](https://github.com/EmmyLua) support (or compatible).

## Setup

For the most part, it should be sufficient to clone this repository or copy defns.lua into a project workspace.

This project was written using [lua-language-server](https://github.com/sumneko/lua-language-server) on VSCode. Some additional settings are required to make this work. In VSCode settings, add the following:
```
{
	"Lua.diagnostics.globals": ["minetest", "vector", "dump", "dump2"]
}
```

## Contributing

PRs are welcome. While most of the API is covered, there are areas with incomplete support and the minetest API has many edge cases. The more we can document and restrict with type definitions, the safer and less error prone mod development becomes.

Priorities:

- Documentation comments for most functions / fields
- Bug fixes
- Correct types for remaining "any" placeholders
- README updates / setup instructions for other IDEs