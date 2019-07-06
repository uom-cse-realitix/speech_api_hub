# RealitiX Speech Recognition API Hub

This repository contains a python wrapper for Speech Recognition Engine used for generating speech transcriptions. These transcriptions are fed towards the fusion engine as the primary modality.

## API Hub

An **API Hub** is merely a router which forwards the requests to the respective microservice. In this wrapper, free ASR services provided by IBM (Watson) and Google Cloud are used.

## Setting up

1. Obtain the `API KEY` and `URL` for Speech-to-text engine provided by [IBM Watson](https://cloud.ibm.com/docs/services/speech-to-text?topic=speech-to-text-gettingStarted). 
2. Fill in `config.yaml` using the credentials obtained in the step above.
3. Install relevant dependencies.

```bash
sudo apt-get install portaudio19-dev python-all-dev python3-all-dev
pip install pyyaml
pip install --upgrade pyaudio
pip install --upgrade ibm-watson
```

Make sure you check out the Python-SDK provided by [Watson Developer Cloud](https://github.com/watson-developer-cloud/python-sdk) as well. This code is obtained from that particular repository.

## Running

Run the code using `python sr.py`.

## Contributions

1. [IBM Watson](https://www.ibm.com/watson/services/speech-to-text/)
2. [Pyyaml](https://pyyaml.org/)