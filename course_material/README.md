# Table of contents

This folder contains a list of notebooks prepared for MIR course for the [Master in Sound and Music Computing](https://www.upf.edu/web/smc) at Universitat Pompeu Fabra.

In the notebooks folder, there exist two types of notebooks for some of the tasks (example: *review_lecture-part_1-hello_spectrum.ipynb* and *review_lecture-part_1-hello_spectrum-complete.ipynb*). *-complete.ipynb* includes the complete version, and the others simply have some spaces for you to fill in as an exercise. 

## Review lectures

The MIR course is offered in the second trimester of the Master in Sound and Music Computing program and assumes the students have already taken the [Audio Signal Processing for Music Applications course](https://www.upf.edu/web/smc/audio-signal-processing-for-music-applications). As some of the brain cells and connections get deleted during the Christmas break, it is a good idea to consider a few review tasks. The following notebooks are prepared to help you warm up. 

**"Hello world" examples for sound processing:**
* [Review lecture part 1: "Hello Spectrum"](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/review_lectures/review_lecture-part_1-hello_spectrum.ipynb): Read a sound file, plot the log amplitude spectrum of the signal. ([the complete notebook](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/review_lectures/review_lecture-part_1-hello_spectrum-complete.ipynb))
* [Review lecture part 2: Energy of a signal](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/review_lectures/review_lecture-part_2-energy_of_a_signal.ipynb): Computing  low-level feature and plotting synchronously with waveform of the sound signal ([the complete notebook](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/review_lectures/review_lecture-part_2-energy_of_a_signal-complete.ipynb))
* [Review lecture part 3: "Hello Spectrogram"](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/review_lectures/review_lecture-part_3-hello_spectrogram.ipynb): Read a sound file, plot amplitude spectrogram ([the complete notebook](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/review_lectures/review_lecture-part_3-hello_spectrogram-complete.ipynb)) 

## Introduction to MIR lectures:

### Lecture 1:
In the first lecture we aim to review basic flow in an MIR classification task and also start considering low-level feature extraction tasks.

* [Lecture 1 part 0: Intro with a case study](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/lectures/lecture_1/lecture_1-part_0-intro_with_a_case_study.ipynb) discusses the task of automatic musical instrument classification on a limited sized dataset. The notebook includes implementation for: raw data analysis and preprocessing(segmentation), feature extraction using Essentia, analysis and preprocessing of features(normalisation), classifier design using an SVM model, testing of the classifier, finally comparative tests using various classifiers
* [Lecture 1 part 1: Low-level features](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/lectures/lecture_1/lecture_1-part_1-low-level_features.ipynb) considers low-level feature extraction, statistical feature extraction and further visualizing samples on statistical feature spaces ([the complete notebook](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/lectures/lecture_1/lecture_1-part_1-low-level_features-complete.ipynb)). 
* [Lecture 1 part 2: Using Essentia.standard](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/lectures/lecture_1/lecture_1-part_2-using_essentia_standard.ipynb) demonstrates use of Essentia-standard for feature extraction within the same settings.
* [Lecture 1 part 3: Cepstrum](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/lectures/lecture_1/lecture_1-part_3-cepstrum.ipynb) demonstrates computation of the cepstrum and use of it for computing spectral envelope. 
* [Lecture 1 part 4: Essentia MFCC example](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/lectures/lecture_1/lecture_1-part_4-essentia_mfcc_example.ipynb) which is an example of Essentia - MFFC function application on the same sound signal. 

### Lecture 2:

In the second lecture we discuss the pitch space. Here are the notebooks:
* [Lecture 2 part 1: F0 auto correlation](Lecture2_step1_F0AutoCorr.ipynb) is on implementing autocorralation based pitch detector ([the completed notebook](Lecture2_step1_F0AutoCorr_solution.ipynb)).
* [Lecture 2 part 2: Essentia predominant melody](Lecture2_step2_EssPreDomMel.ipynb) demonstrates the use of the predominant melody extraction function of Essentia, discusses the influence of analysis parameters on the estimated pitch info and also demonstrate use of [mir_eval](https://github.com/craffel/mir_eval) library to evaluate performance of a pitch extractor. 
* [Lecture 2 part 3: Summing band energies](Lecture2_step3_summingBandEnergies.ipynb) considers chromagram computation ([the completed notebook](Lecture2_step3_summingBandEnergies.ipynb)) 
* [Lecture 2 part 4: Chord detection demo](Lecture2_step4_ChordDetectionDemo.ipynb) demonstrates automatic chord detection using chroma features.

### Lecture 3:
In Lecture 3, we discuss the rhythm aspect. 
* In [Lecture 3 part 1: Novelty functions](Lecture3_step1_noveltyFunctions.ipynb), some common novelty functions are implemented ([the completed notebook](Lecture3_step1_noveltyFunctions_solution.ipynb)) 
* [Lecture 3 part 2: Onset and beat detection](Lecture3_step2_Onset_Beat_Detection.ipnb) demonstrates the use of Essentia onset detection functions (using HFC and complex spectral difference) and a beat-tracker.
* [Lecture 3 part 3: Tempogram auto correlation](Lecture3_step3_Tempogram_autoCorr.ipynb) includes a simple tempogram computation and demonstration

### Lecture 4:
Lecture 4 considers MIR for mon-Western music traditions:
* [Lecture 4 part 1: Download all Saraga content](Lecture4_1_downloadAllSARAGAContent.ipynb) includes sample code to download Hindustani and Carnatic music data from CompMusic servers
* [Lecture 4 part 2: Visualize annotations](Lecture4_2_visualizeAnnotations.ipynb) aims at demonstrating some of the contents of Saraga database annotations: sections, typical phrases, sama and tempo annotations.
* [Lecture 4 part 3: Tuning analysis - Single recording](Lecture4_3_tuningAnalysis_SingleRecording.ipynb) considers tuning analysis of a recording of Turkish makam music 
* [Lecture 4 part 4: Tuning analysis - Set of recordings](Lecture4_4_tuningAnalysis_SetOfRecordings.ipynb) does the same job and merges the outputs to gather information required for building a makam scale model. 

### Lecture 5:
Introduction to MIR using symbolic data
* [Lecture 5 part 1: Introduction to music21](Lecture5_music21_intro.ipynb) is a very short introduction to music21, a toolkit for computational aided musicology
* [Lecture 5 part 2: Melodic segmentation](Lecture5_melodicSegmentation.ipynb) Melodic segmentation using Local Boundary Detection Model (LBDM by Cambouropoulos, E. (2001)).
* [Lecture 5 part 3: Matching time series data](Lecture5_matchingTimeSeriesData.ipynb) discusses the problem of matching time-series data (such as finding short melody sequences within songs)

## MIR application tutorials

### Automatic music tagging and classification (by Minz Won)
* [Slides](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/mir_applications/automatic_music_tagging_and_classification/automatic_music_tagging_tutorial.pdf)

### NLP for MIR (by Sergio Oramas)
* [Slides part 1](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/mir_applications/nlp_for_mir/nlp_for_mir_tutorial_part1.pdf)
* [Slides part 2](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/mir_applications/nlp_for_mir/nlp_for_mir_tutorial_part2.pdf)

### Music version identification (by Furkan Yesiler)
* [Jupyter notebook](#)

### Audio source separation (by Jordi Pons)
* [Slides](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/mir_applications/audio_source_separation/audio_source_separation_tutorial.pdf)
