# IndicTrans2 Model Distribution

This directory documents the expected location and package layout for the offline IndicTrans2 translation model used by Vidya Trace AI.

## Where to put the model

Place the final Android-compatible IndicTrans2 model package under:

`models/indictrans2/v1/`

Do **not** commit the large model binary/files to the normal source tree. The final distributable model should be attached to a GitHub Release as a release asset.

Expected release asset name:

`vidya-trace-indictrans2-v1.zip`

The SHA-256 checksum of that exact asset must be recorded in `manifest.json`.

## Expected package contents

The ZIP should contain the model files required by the Android inference runtime, for example:

- model weights
- tokenizer files
- configuration files
- runtime metadata

The exact files depend on the chosen IndicTrans2 Android-compatible conversion/runtime.
