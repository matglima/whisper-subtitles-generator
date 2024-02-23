# Whisper and ArgosTranslate Subtitles generator

## Overview
This project features a streamlined pipeline for audio extraction from video, precise segmentation, and automatic English subtitle generation through OpenAI's Whisper. It integrates the generated subtitles with the original video and employs the ArgosTranslate open-source offline translation library written in Python for translation. The final output is a compressed video within Jupyter/Colab notebooks. Additionally, the project offers user-friendly interaction via Gradio, enabling users to swiftly input their videos and receive subtitled video outputs.

The OpenAI's Whisper can natively generate subtitles in other languages from a video in almost any language, but Whisper's performance varies widely depending on the language, as can be seen in the bellow Language x WER (Word Error Rate) image from [Whisper's paper](https://arxiv.org/abs/2212.04356) 

![Whisper Language Word Error Rate](https://raw.githubusercontent.com/openai/whisper/main/language-breakdown.svg)

The most optimized and precise subtitle generation pipeline would be to first generate Spanish subtitles with Whisper and then translate them to the desired language using ArgosTranslate, but, for simplicity for displaying the video with English subtitles in colab/jupyter notebooks the generated subtitle by Whisper was kept in English.


## Colab Demo

Explore a live demo of the project in Google Colab: [Colab Demo](https://colab.research.google.com/drive/1lXn_ZzV188FhNImboUA8HyG9CwU6iM7G?usp=sharing)

## Contribution

Contributions are welcome! If you'd like to contribute to the project, feel free to contact me.

## License

This project is licensed under the [Apache 2.0 License](LICENSE).
