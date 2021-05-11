# transcribe-anything
Input a local file or url and this service will transcribe it using Mozilla Deepspeech 0.9.3.

# Quick start

## Optional: Create a virtual python package
  * Works for Ubuntu/MacOS bash or win32 git-bash
  * `mkdir transcribe_anything`
  * `cd transcribe_anything`
  * Download and install virtual env:
    * `curl -X GET https://raw.githubusercontent.com/zackees/make_venv/main/make_venv.py -o make_env.py`
    * `python make_env.py`
  * Enter the environment:
    * `source activate.sh`

The environment is now active and the next step will only install to the local python. If the terminal
is closed then to get back into the environment `cd transcribe_anything` and execute `source activate.sh`

## Required: Install to current python environment
  * `pip install transcribe-anything`
    * The command `transcribe_anything` will magically become available.
  * `transcribe_anything <YOUTUBE_URL> out_subtitles.txt`
  * -or- `transcribe_anything <MY_LOCAL.MP4/WAV> out_subtitles.txt`

# Tech Stack
  * Mozilla DeepSpeech: https://github.com/mozilla/DeepSpeech
  * mic_vad_streaming: https://github.com/hadran9/DeepSpeech-examples/tree/r0.9/mic_vad_streaming
  * youtube-dl:
    * github: https://github.com/ytdl-org/youtube-dl
  * static-ffmpeg
    * github: https://github.com/zackees/static_ffmpeg
    * pypi: https://pypi.org/project/static-ffmpeg/
