<div align="center">

<img src="assets/brand/getclipper-logo.png" alt="getclipper" width="140">

# getclipper

**Turn long videos and streams into short vertical clips. Free, open source, runs on your own PC.**

by [getfirstsale](https://github.com/getfirstsale)

</div>

getclipper finds the moments worth posting in a long video or stream, crops them to 9:16 with the
speaker kept in frame, burns in captions and writes titles. Everything runs on your machine:
no account, no upload, no subscription, no watermark.

## Built on open source

getclipper is a modified version of **Clips Studio / Clips Kitty** by
[ColinGPT9](https://github.com/ColinGPT9/clips-studio), released under the
**GNU Affero General Public License v3.0 (AGPL-3.0)**. All the heavy lifting is theirs;
getfirstsale adds the branding, setup guide and presets.

- Original project: <https://github.com/ColinGPT9/clips-studio>
- Original documentation (kept for reference): [docs/UPSTREAM-README.md](docs/UPSTREAM-README.md)
- What we changed: see [NOTICE](NOTICE)

Not affiliated with or endorsed by the original author. "Clips Kitty" belongs to its owner.

## Requirements

|             | Minimum                                       | Recommended                  |
| ----------- | --------------------------------------------- | ---------------------------- |
| **GPU**     | NVIDIA RTX 2060 (6 GB)                        | RTX 3060 12 GB or better     |
| **CPU**     | Intel Core i3-9100 / AMD Ryzen 3 3200G (2019) | 6 cores or more              |
| **RAM**     | 16 GB                                         | 16 GB or more                |
| **Disk**    | ~20 GB, plus room for the videos you clip     |                              |
| **OS**      | Windows 10 or 11                              |                              |

Below the minimum it may still run, but slowly and without support.

## Set it up with Claude Code

1. Install [Git](https://git-scm.com), [Python 3.10+](https://www.python.org), [Node.js 18+](https://nodejs.org)
   and [Claude Code](https://claude.com/claude-code).
2. Clone and open the folder:
   ```bash
   git clone https://github.com/getfirstsale/getclipper.git
   cd getclipper
   claude
   ```
3. Tell Claude: **"Set up getclipper on this PC and clip this video: <link>"**.
   Claude installs the dependencies, starts the engine and runs the job for you.

Prefer the terminal? The manual route:

```bash
pip install -r requirements.txt
python main.py process "https://www.youtube.com/watch?v=VIDEO_ID"
python main.py status
```

Full options, models and platform guides are in the [original documentation](docs/UPSTREAM-README.md)
and the [docs/](docs/) folder.

## Licence

AGPL-3.0-or-later. See [LICENSE](LICENSE) and [NOTICE](NOTICE). If you modify getclipper and share it
or run it as a service for others, you must offer them your source under the same licence.
Your videos and clips are yours.
