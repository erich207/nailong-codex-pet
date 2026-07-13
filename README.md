# Nailong Codex Pet codex宠物 奶龙

An unofficial soft toy-style animated Codex pet inspired by the yellow Nailong character references. The pet uses the Codex v2 spritesheet format with 11 animation rows and 8 columns.

![Nailong Codex Pet](https://raw.githubusercontent.com/erich207/nailong-codex-pet/main/spritesheet.webp)

## Files

- `pet.json` - Codex pet manifest.
- `spritesheet.webp` - v2 animated pet atlas, 1536 x 2288, RGBA WebP.
- `pet/` - same install-ready files grouped as a package.
- `qa/` - validation and visual QA artifacts.

## Install

Copy the root manifest and spritesheet into your Codex pets folder:

```bash
mkdir -p ~/.codex/pets/nailong-toy
cp pet.json spritesheet.webp ~/.codex/pets/nailong-toy/
```

The manifest includes:

```json
{
  "id": "nailong-toy",
  "displayName": "奶龙",
  "spriteVersionNumber": 2,
  "spritesheetPath": "spritesheet.webp"
}
```

Restart or refresh Codex after installation if the pet does not appear immediately.

## QA

The installed spritesheet was validated with the hatch-pet v2 atlas validator:

- Format: WebP RGBA
- Size: 1536 x 2288
- Grid: 8 columns x 11 rows
- `spriteVersionNumber`: 2
- Validation errors: none

The generated direction blind-review workers were unavailable during packaging because the account hit a usage limit. The final package was accepted after labeled direction review, deterministic atlas validation, chroma despill validation, and user confirmation.

## License

MIT. See `LICENSE`.

