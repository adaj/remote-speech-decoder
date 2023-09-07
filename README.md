# Transcription and diarization with a remote microphone

## Installation steps

```
conda create --name <name_your_env> python=3.8
conda activate <name_your_env>
conda install portaudio=19.6.0 pysoundfile=0.12.1 ffmpeg=4.3 -c conda-forge
pip install diart whisper_timestamped
```

Additional GPU setup (if applicable).

```
pip install torch==1.13.1+cu117 --index-url https://download.pytorch.org/whl/cu117
pip install torchaudio==0.13.1+cu117 --index-url https://download.pytorch.org/whl/cu117
```

## Usage

1. Check `.env` for the preferred settings.
2. Run `decoder.ipynb` on the main server.
3. Run `client_mic.py` on the client machine with a microphone.
4. Check the output displayed on the decoder.
