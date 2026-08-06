# Castavox downloads

Installers for **Castavox** and **Pulpitry**. This repository holds no source
code — only released binaries, so that the download links are public while the
projects themselves are not.

The installers are **release assets**, not files in this repository — GitHub
caps repository files at 100 MB and Castavox is nearly three times that. So
there is nothing to see in the file list above; the downloads are here:

| | macOS (Apple silicon) | Windows | Linux |
|---|---|---|---|
| **Castavox** | [0.1.0 · 272 MB](https://github.com/aysmart/castavox-downloads/releases/download/castavox-v0.1.0/Castavox-0.1.0-macos-arm64.dmg) | not published yet | not published yet |
| **Pulpitry** | [0.1.0 · 60 MB](https://github.com/aysmart/castavox-downloads/releases/download/pulpitry-v0.1.0/Pulpitry-0.1.0-macos-arm64.dmg) | not published yet | not published yet |

All releases, with notes: [Releases](../../releases). Or use
[castavox.com/download](https://castavox.com/download).

## These builds are not signed

Neither macOS nor Windows builds are code signed yet.

- **macOS** marks anything downloaded from the internet as quarantined. Because
  the app is unsigned, Gatekeeper refuses to open it and reports that it is
  damaged. It is not. Either right-click the app and choose Open, or clear the
  flag:

  ```
  xattr -dr com.apple.quarantine /Applications/Castavox.app
  ```

- **Windows** SmartScreen will warn that the publisher is unknown. Choose
  "More info", then "Run anyway".

- **Linux** packages are unaffected; that platform does not gate on a signature.

Check what you downloaded against `SHA256SUMS.txt` on the release if you want to
be sure it arrived intact.

## Source code

**Pulpitry** is proprietary. No source is offered.

**Castavox** is a derivative work of [OBS Studio](https://obsproject.com) and is
licensed under the **GNU General Public License, version 2 or later**. If you
have received a Castavox binary, you are entitled to its complete corresponding
source code.

### Written offer

In accordance with GPLv2 section 3(b), the copyright holder hereby offers, valid
for **three years** from the date each binary was distributed, to give any third
party a complete machine-readable copy of the corresponding source code for the
version of Castavox they received, for no more than the cost of physically
performing the distribution.

To request it, open an issue on this repository or write to the address on
[castavox.com](https://castavox.com). The source will be supplied on the same
terms as the licence requires, whether or not you are the person who downloaded
the binary.

OBS Studio is copyright Lain Bailey and contributors. Castavox's changes are
additions to their work, not a replacement for it, and their notices remain in
the About box and in the source.
