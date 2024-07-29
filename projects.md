# Projects

## Synthetic image evolution using decoded neurofeedback

This is the topic of my PhD dissertation which will began in September 2023 and will progress until about August 2026. Essentially, we are trying to create a **BOGARt (Biometric Optimization of Generated Affective Representations)**, or a machine which adapts to your fears (or insert other emotional response) and generates images that maximally activate that emotion. Why? Partly, just to see if we can. However, the differences between images generated using conscious self-reports and neural or other physiological correlates may help us to understand what kind of information is represented using these different measurement schemes.

This project is in the development stage, and is accessible through multiple GitHub repos:

[Decoder Construction](https://github.com/dariusvalevicius/decoder-construction): This contains the code for fast preprocessing of fMRI data in native space, which is necessary to be able to replicate the same pipeline in a realtime experiment. A model script shows the steps involved in coming up with a classification model that uses a combination of PCA and logistic regression to get a generalizable model of whole-brain activity which can predict emotion responses.

[Realtime Evolution](https://github.com/dariusvalevicius/realtime-evolution): This repository contains the code for the real-time experiment. The experiments are split across two computers: A stimulus presentation computer, which runs the PsychoPy script presenting the generated images and recomputes new embeddings based on a fitness function, and a support computer, which runs the preprocessing, model prediction, and image generation programs asynchronously.

## Biofeedback tone therapy

Another project, similar to my PhD project, is a method of optimizing peripheral biometric measures (that's things like heartrate and skin conductance) using a kind of adaptive tone therapy - or as my collaborator [Danny Barwick](https://www.instagram.com/dannybarwickmusic) puts it, creating "a song that listens to your body". More on this soon...