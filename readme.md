This is an archive of random neovim plugins I've written. None of these are really designed for general use! Some things may be hardcoded, or there may be edge cases that don't work, or they could be written in a much nicer way...but maybe they'll still be useful to someone.

In the descriptions below `|` indicates the cursor position.

- `breakout.lua`: jump to right after the end of a delimiter pair. For example jumping from `fn example(a, b, |c, d)` to `fn example(a, b, c, d)|`. This was written to make working with auto pair plugins easier.
- `objects.lua`: a simple way to define new text objects using lua patterns.
- `sights.lua`: makes it easier to target text objects by using `hop`. When I need to jump to, for example, an argument in a function call to change it, it's not immediately clear which argument it is, and I don't want to have to count to figure out if it should be `c2ina` or `c3ina` etc. I also frequently mess up the order or hit the wrong number, or the selection is unexpected for nested arguments. This instead lets me do something like `Cia`, then uses hop to hint all valid/visible inner argument regions.
- `francais.lua`: grammar, spellchecking, dictionary, and translation tooling for French. Owes a lot to [dpelle](https://github.com/dpelle) who has two plugins I basically just updated for neovim's built-in diagnostics.
