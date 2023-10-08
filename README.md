# whisper-subtitles-generator
This project features a streamlined pipeline for audio extraction from video, precise segmentation, and automatic English subtitle generation through OpenAI's Whisper. It seamlessly integrates these subtitles with the original video and employs the ArgosTranslate open-source offline translation library written in Python for effortless translation. The final output is presented as a compressed video within Jupyter/Colab notebooks. Additionally, the project offers user-friendly interaction via Gradio, enabling users to input their videos and receive subtitled video outputs swiftly.

The OpenAI's Whisper can natively generate subtitles in other languages from a video in almost any language, but the performance is not optimal in every language, as can be see in the bellow Language x WER (Word Error Rate) from [Whisper's paper](https://arxiv.org/abs/2212.04356) 

![Whisper Language Word Error Rate](https://raw.githubusercontent.com/openai/whisper/main/language-breakdown.svg)

For this reason in this code it was used the ArgosTranslate open-source offline translation library.
