# MQKit engines

Unchanged copies of the files [MQKit](https://github.com/MQKit/app) downloads when a tool
first needs them: AI models, a portable Python and the Python packages some tools run on.

The app downloads each file from its own source. When that source is unavailable, or the
file there has changed, it falls back on the copy here. Either way it accepts a file only
with the size and SHA-256 written in its catalog
([engines.toml](https://github.com/MQKit/app/blob/main/src-tauri/engines.toml),
[engines.python.toml](https://github.com/MQKit/app/blob/main/src-tauri/engines.python.toml)),
so a copy here can never be anything other than the original.

Each engine and version is a [release](https://github.com/MQKit/engines/releases) named
`<engine>-<version>`, with the licence, the source and the SHA-256 of every file in its
notes. Packages under the AGPL come with their source code.

FFmpeg and LibreOffice are not copied here: their builds contain many libraries under the
GPL and LGPL, whose source code would have to be hosted alongside them.

A daily check in the app's repository verifies every source and every copy.
