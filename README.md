# python-tts-example

## Requirements

```
pip install pyaudio
```

## Setting your DEEPGRAM_API_KEY Env Var

```
export DEEPGRAM_API_KEY=xxx
```

## Choosing your audio output devive

The first time you run this code find the correct audio device that you want to send the audio to

```
Device 0: HD Web Camera: USB Audio (hw:0,0) - Input Channels: 1 - Output Channels: 0
Device 1: Dell Universal Dock D6000: USB Audio (hw:1,0) - Input Channels: 2 - Output Channels: 6
Device 2: sof-hda-dsp: - (hw:2,0) - Input Channels: 2 - Output Channels: 2
```

Once you have found which Device ID you want to play the audio on update the value [here](https://github.com/DamienDeepgram/python-tts-example/blob/main/main.py#L28)

```output_device_index = 2```

## Running

```
python main.py
```

## Streaming vs Download

To download before playing the audio set this flag to False

[STREAM_AUDIO](https://github.com/DamienDeepgram/python-tts-example/blob/main/main.py#L5-L6)
