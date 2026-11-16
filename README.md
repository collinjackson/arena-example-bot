# arena-example-bot

An example [libaw-arena](https://github.com/collinjackson/libaw-arena) bot, made from the arena's
[bot template](https://github.com/collinjackson/libaw-arena/tree/main/templates/bot): it attacks
when it can, else captures, else builds, else takes libaw's baseline pick.

    rustup target add wasm32-unknown-unknown
    cargo build --release --target wasm32-unknown-unknown

Pushing a tag (`git tag v1 && git push origin v1`) runs `.github/workflows/release.yml`, which
builds the module, attaches it to a release, and puts its `bots.json` entry in the release notes.

MIT or Apache-2.0, at your option.
