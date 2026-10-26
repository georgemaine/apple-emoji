Apple emoji images, sprite sheets and search keywords, as static files.

## Usage

Install it in your project:

```bash
yarn add "@georgemaine/apple-emoji@https://github.com/georgemaine/apple-emoji.git#tag=v1.0.1"
```

Serve `node_modules/@georgemaine/apple-emoji/emoji/` as static files, then point your emoji picker at it.

## What's inside

```
emoji/                   the folder you serve
├── sprite-sheets/       one image per category (food, flags…), every emoji a 64×64 tile
│                        in .avif, with .webp for browsers without avif; draws the picker grid
├── emoji/               one .webp per emoji, named by code point (1f355.webp = 🍕);
│                        for showing a single emoji, e.g. a reaction
└── search/              one .json per language, keyword → emoji ("pizza" → 🍕)
```

The grid loads one sprite sheet per category instead of thousands of single files. The search
box loads only the file for the page's language.

`SHA256SUMS` lists a checksum for every file in `emoji/`. Check them with
`shasum -a 256 -c SHA256SUMS`.

## License

Apple images, Copyright © Apple Inc. For personal, non-commercial use only. See [LICENSE.md](LICENSE.md).
