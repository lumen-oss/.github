# Lumen

We 💜 Lua
  
Lua continues to be the most used embeddable scripting language on the planet, and yet has an ecosystem that's stuck in the 2000's.
We're here to change that.

Lumen's mission is to boost Lua back into the modern age by revamping:
- 📦 The main package manager (see [Lux](#lux))
- 🚀 The module hosting site (see [Luanox](#luanox))
- ⌨️ Embedding Lux into applications which use Lua as their scripting language (see [other](#other))

## Lux

https://github.com/lumen-oss/lux

Lua's current package manager is difficult to use for the average person and *isn't embeddable in other applications*. Lux aims to change all of that:
* Easy managing of dependencies, build steps and more through a single `lux.toml` file
* Parallel builds and installs :rocket:
* Add/remove dependencies with simple CLI commands
* Automatic generation of rockspecs, removing the need for managing 10 different rockspec files in your source code :tada:
* Seamless integrations with external formatting, linting and typechecking tools
* Powerful lockfile support
* Full compatibility with luarocks itself 🌟

Lux is also fully embeddable as a Rust library but also as a Lua library, meaning that any application can freely use its powerful package management capabilities for free.

## Luanox

https://github.com/lumen-oss/luanox

We're actively working on building a scalable and fast module hosting website for Lua packages, using all of the latest and best security practices. We don't even store usernames/passwords
in our database since we delegate our work to OAuth providers.

Luanox aims to be:
- Simple to use (with a clean, modern look)
- Highly secure (signed JWT tokens instead of often badly protected API keys)
- Immutable (packages cannot be deleted or force pushed, reducing supply chain risk)
- Configurable

Paired with Lux, this turns a hectic and troublesome Lua experience into pure joy 🎉

## Other

Apart from just revamping the ecosystem, we also made it our mission to expand our reach to other communities that also use Lua, specifically Neovim. We believe that Neovim plugins should be distributed as real Lua packages with dependencies, versioning and access to the whole luarocks ecosystem. 

Feel free to check out all of the related links below:

* [rocks.nvim](https://github.com/lumen-oss/rocks.nvim)
* [NURR](https://github.com/lumen-oss/nurr)
