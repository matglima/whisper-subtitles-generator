# Whisper and ArgosTranslate Subtitles generator
This project features a streamlined pipeline for audio extraction from video, precise segmentation, and automatic English subtitle generation through OpenAI's Whisper. It seamlessly integrates these subtitles with the original video and employs the ArgosTranslate open-source offline translation library written in Python for effortless translation. The final output is presented as a compressed video within Jupyter/Colab notebooks. Additionally, the project offers user-friendly interaction via Gradio, enabling users to input their videos and receive subtitled video outputs swiftly.

The OpenAI's Whisper can natively generate subtitles in other languages from a video in almost any language, but Whisper's performance varies widely depending on the language, as can be see in the bellow Language x WER (Word Error Rate) image from [Whisper's paper](https://arxiv.org/abs/2212.04356) 

![Whisper Language Word Error Rate](https://raw.githubusercontent.com/openai/whisper/main/language-breakdown.svg)

For this reason, in this code it was used the ArgosTranslate open-source offline translation library. The most optimized subtitle generation pipeline would be to first generate spanish subtitles with Whisper and then translate it to the desired languge using ArgosTranslate, but, for simplicity and to display the video with english subtitles in colab/jupyter notebooks the generated subtitle by Whisper was kept in english.


## Colab Demo

Explore a live demo of the project in Google Colab: [Colab Demo](https://colab.research.google.com/drive/1lXn_ZzV188FhNImboUA8HyG9CwU6iM7G?usp=sharing)

## Contribution

Contributions are welcome! If you'd like to contribute to the project, feel free to contact me.

## License

This project is licensed under the [MIT License](LICENSE).
