# Whisper and ArgosTranslate Subtitles generator
This project features a streamlined pipeline for audio extraction from video, precise segmentation, and automatic English subtitle generation through OpenAI's Whisper. It seamlessly integrates these subtitles with the original video and employs the ArgosTranslate open-source offline translation library written in Python for effortless translation. The final output is a compressed video within Jupyter/Colab notebooks. Additionally, the project offers user-friendly interaction via Gradio, enabling users to swiftly input their videos and receive subtitled video outputs.

The OpenAI's Whisper can natively generate subtitles in other languages from a video in almost any language, but Whisper's performance varies widely depending on the language, as can be seen in the bellow Language x WER (Word Error Rate) image from [Whisper's paper](https://arxiv.org/abs/2212.04356) 

![Whisper Language Word Error Rate](https://raw.githubusercontent.com/openai/whisper/main/language-breakdown.svg)

For this reason, this code it was used the ArgosTranslate open-source offline translation library. The most optimized subtitle generation pipeline would be to first generate Spanish subtitles with Whisper and then translate them to the desired language using ArgosTranslate, but, for simplicity and to display the video with English subtitles in colab/jupyter notebooks the generated subtitle by Whisper was kept in English.


## Colab Demo

Explore a live demo of the project in Google Colab: [Colab Demo](https://colab.research.google.com/drive/1lXn_ZzV188FhNImboUA8HyG9CwU6iM7G?usp=sharing)

## Contribution

Contributions are welcome! If you'd like to contribute to the project, feel free to contact me.

## License

This project is licensed under the [Apache 2.0 License](LICENSE).
