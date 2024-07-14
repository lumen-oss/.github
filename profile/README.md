# nvim-neorocks

Neovim ❤️ LuaRocks

Neorocks aims at encouraging good software practice in the neovim plugin ecosystem,

One major addition in nvim compared to vim is the native support of an
existing scripting language aka Lua, with numerous packages available (yaml/json
loaders, testing libraries like busted etc)

This favors code reuse, a rare sight in vimscript land, and makes it possible
for plugin to focus on their primary objective, without reinventing the wheel.

These dependencies can be installed via the historical Lua package manager
www.luarocks.org. We want to encourage plugin authors to specify their plugin
dependencies in the luarocks package format: aka
[rockspec](https://github.com/luarocks/luarocks/wiki/Rockspec-format) (see the
[rocks.nvim](https://github.com/nvim-neorocks/rocks.nvim) rockspec for an
[example](https://github.com/nvim-neorocks/rocks.nvim/blob/master/rocks.nvim-scm-1.rockspec)).

This allows to shift the burden of specifying plugin dependencies from
the users to the plugin authors. The plugin author can change the plugin
dependencies without breaking its users configurations. Fewer support issues it
is a win-win !
And between our [github
action](https://github.com/nvim-neorocks/luarocks-tag-release/) and our
own [repository][NURR] of luarocks package definitions, it has never been easier
to publish a package to luarocks.org.

We at neorocks want to promote the semantic versioning of plugins: instead of
blindly cloning plugins from git with the hope the update does not break one's
own config, pin the plugin version.
For instance [rocks.nvim][rocks.nvim] asks you if you really want to update a
plugin with a major version change.

We encourage plugin authors to test their plugins now that luarocks provides
good testing libraries like busted. It has never been this easy to test your
plugin using neovim as a lua interpreter with [nlua].

Our member @mrcjkb also
[explains](https://mrcjkb.dev/posts/2023-08-22-setup.html) why entangling installation and configuration
makes plugin manager work harder.
He also published a
[guide](https://github.com/nvim-neorocks/nvim-best-practices) on good practice for neovim plugin development.


[rocks.nvim]: https://github.com/nvim-neorocks/rocks.nvim
[nlua]:  https://github.com/mfussenegger/nlua
[NURR]: https://github.com/nvim-neorocks/nurr


<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
