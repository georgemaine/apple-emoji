Apple emoji images, sprite sheets and search keywords, as static files.

## Usage

Install it in your project:

```bash
yarn add "@georgemaine/apple-emoji@https://github.com/georgemaine/apple-emoji.git#tag=v1.0.0"
```

Serve the `emoji/` folder as static files, then point your emoji picker at it:

```
emoji/
├── emoji/<codepoints>.webp            one image per emoji
├── sprite-sheets/<category>-64x64.*   one sheet per category, avif and webp
└── search/<locale>.json               keyword → emoji lists
```

## License

Apple images, Copyright © Apple Inc. For personal, non-commercial use only. See [LICENSE.md](LICENSE.md).
