# q-base

or

## How to share a Qlty configuration (Part 1)

This repo works in concert with [q-shared](https://github.com/rsl/q-shared) to provide simple documentation about how to use shared configuration for Rubocop in Qlty.

This repo is an example of how to consume shared Qlty configuration. The first step would be to make sure you've [setup Qlty](https://docs.qlty.sh/cli/quickstart) in your repo.

The meat of getting things done is this bit you want to add to your `qlty.toml`. All the other (shared) configuration should reside in the other repo you're putting as a source.

```
[[source]]
name = "q-shared"
repository = "https://github.com/rsl/q-shared.git"
branch = "main"
```

Obviously, point this at your own repo and all. See the [full file](https://github.com/rsl/q-base/blob/main/.qlty/qlty.toml) itself for how little you need in the base repo to pull in the shared.

## TODO

Add Reek
