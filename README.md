## System requirement

- Python3, pip
- google protobuf for python `pip3 install protobuf`

### Full OTA

- ./extract.py [--skip_hash] --output_dir output/ payload.bin
- This will start to extract the images within the payload.bin file to the output folder you are in.

### Incremental OTA

- Copy original images (from full OTA or dumped from devices) to old folder
- ./extract.py [--skip_hash] --output_dir output/ --old_dir old/ payload.bin
