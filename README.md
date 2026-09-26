# town-hall-qa-log

Transcribes a town hall meeting and logs every question asked and the answer given, on-device. Built with [Tether's QVAC SDK](https://github.com/tetherto/qvac) — the model runs on-device, so nothing leaves your machine.

## What it does

Transcribes a town hall meeting and logs every question asked and the answer given, on-device.

**QVAC functions used:** `loadModel`, `transcribe` and `completion`.

![town-hall-qa-log demo](demo.png)

## Why I built it

Town halls promise follow-ups that nobody writes down.

## Requirements

- Node.js >= 22
- `@qvac/sdk` `^0.19.0` (installed automatically via `npm install`)

## Install

```bash
git clone https://github.com/YURIIMII-byte/town-hall-qa-log.git
cd town-hall-qa-log
npm install
```

## Run

```bash
node index.js path/to/town-hall.wav
```

See the comments at the top of `index.js` for the exact input this app expects. On first run, QVAC downloads the model it needs once and caches it locally; every run after that is fully offline.

## SDK version used

`@qvac/sdk` `0.19.1`

## License

MIT — see [LICENSE](LICENSE).
