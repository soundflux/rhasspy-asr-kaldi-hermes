# Rhasspy ASR Kaldi Hermes MQTT Service

![Docker Build/Publish kaldi Armv7 Image](https://github.com/soundflux/rhasspy-asr-kaldi-hermes/workflows/Docker%20Build/Publish%20kaldi%20Armv7%20Image/badge.svg)
![Build x64 Docker Image](https://github.com/soundflux/rhasspy-asr-kaldi-hermes/workflows/Build%20x64%20Docker%20Image/badge.svg)

Implements `hermes/asr` functionality from [Hermes protocol](https://docs.snips.ai/reference/hermes) using [rhasspy-asr-kaldi](https://github.com/rhasspy/rhasspy-asr-kaldi).

## Requirements

* Python 3.7
* [Kaldi](https://kaldi-asr.org)
    * Expects `$KALDI_DIR` in environment
* [Opengrm](http://www.opengrm.org/twiki/bin/view/GRM/NGramLibrary)
    * Expects `ngram*` in `$PATH`
* [Phonetisaurus](https://github.com/AdolfVonKleist/Phonetisaurus)
    * Expects `phonetisaurus-apply` in `$PATH`

See [pre-built apps](https://github.com/synesthesiam/prebuilt-apps) for pre-compiled binaries.

## Installation

```bash
$ git clone https://github.com/rhasspy/rhasspy-asr-kaldi-hermes
$ cd rhasspy-asr-kaldi-hermes
$ ./configure --enable-in-place
$ make
$ make install
```

## Running

```bash
$ ./rhasspy-asr-kaldi-hermes <ARGS>
```
