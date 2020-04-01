## Table of contents

This folder contains a list of notebooks prepared for MIR course for the [Master in Sound and Music Computing](https://www.upf.edu/web/smc) at Universitat Pompeu Fabra.

In the notebooks folder, there exist two types of notebooks for some of the tasks (example: *review_lecture-part_1-hello_spectrum.ipynb* and *review_lecture-part_1-hello_spectrum-complete.ipynb*). *-complete.ipynb* includes the complete version, and the others simply have some spaces for you to fill in as an exercise. 

## Review lectures

The MIR course is offered in the second trimester of the Master in Sound and Music Computing program and assumes the students have already taken the [Audio Signal Processing for Music Applications course](https://www.upf.edu/web/smc/audio-signal-processing-for-music-applications). As some of the brain cells and connections get deleted during the Christmas break, it is a good idea to consider a few review tasks. The following notebooks are prepared to help you warm up. 

**"Hello world" examples for sound processing:**
* [Review lecture part 1: "Hello Spectrum"](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/review_lectures/review_lecture-part_1-hello_spectrum.ipynb): Read a sound file, plot the log amplitude spectrum of the signal. ([the complete notebook](https://github.com/furkanyesiler/MIRCourse/blob/master/course_material/review_lectures/review_lecture-part_1-hello_spectrum-complete.ipynb))
* [Review lecture part 2: Energy of a signal](ReviewLecture_2_EnergyOfASignal.ipynb): Computing  low-level feature and plotting synchronously with waveform of the sound signal ([the complete notebook](ReviewLecture_2_EnergyOfASignal_solution.ipynb))
* [Review lecture part 3: "Hello Spectrogram"](ReviewLecture_3_HelloSpectrogram.ipynb): Read a sound file, plot amplitude spectrogram ([the complete notebook](ReviewLecture_3_HelloSpectrogram_solution.ipynb)) 

## Lecture 1:
In the first lecture we aim to review basic flow in an MIR classification task and also start considering low-level feature extraction tasks.

* [Lecture 1 part 0: Intro with a case study](Lecture1_IntroWithACaseStudy.ipynb) discusses the task of automatic musical instrument classification on a limited sized dataset. The notebook includes implementation for: raw data analysis and preprocessing(segmentation), feature extraction using Essentia, analysis and preprocessing of features(normalisation), classifier design using an SVM model, testing of the classifier, finally comparative tests using various classifiers
* [Lecture 1 part 1: Low-level features](Lecture1_step1.ipynb) considers low-level feature extraction, statistical feature extraction and further visualizing samples on statistical feature spaces ([the complete notebook](Lecture1_step1_solution.ipynb)). 
* [Lecture 1 part 2: Using Essentia.standard](Lecture1_step2_usingEssentiaStandard.ipynb) demonstrates use of Essentia-standard for feature extraction within the same settings.
* [Lecture 1 part 3: Cepstrum](Lecture1_step3_cepstrum.ipynb) demonstrates computation of the cepstrum and use of it for computing spectral envelope. 
* [Lecture 1 part 4: Essentia MFCC example](Lecture1_step4_essentiaExample_MFCC.ipynb) which is an example of Essentia - MFFC function application on the same sound signal. 

## Lecture 2:

In the second lecture we discuss the pitch space. Here are the notebooks:
* [Lecture2_step1_F0AutoCorr](Lecture2_step1_F0AutoCorr.ipynb) is on implementing autocorralation based pitch detector ([the completed notebook](Lecture2_step1_F0AutoCorr_solution.ipynb)).
* [Lecture2_step2_EssPreDomMel](Lecture2_step2_EssPreDomMel.ipynb) demonstrates the use of the predominant melody extraction function of Essentia, discusses the influence of analysis parameters on the estimated pitch info and also demonstrate use of [mir_eval](https://github.com/craffel/mir_eval) library to evaluate performance of a pitch extractor. 
* [Lecture2_step3_summingBandEnergies](Lecture2_step3_summingBandEnergies.ipynb) considers chromagram computation ([the completed notebook](Lecture2_step3_summingBandEnergies.ipynb)) 
* [Lecture2_step4_ChordDetectionDemo](Lecture2_step4_ChordDetectionDemo.ipynb) demonstrates automatic chord detection using chroma features.

## Lecture 3:
In Lecture 3, we discuss the rhythm aspect. 
* In [Lecture3_step1_noveltyFunctions](Lecture3_step1_noveltyFunctions.ipynb), some common novelty functions are implemented ([the completed notebook](Lecture3_step1_noveltyFunctions_solution.ipynb)) 
* [Lecture3_step2_Onset_Beat_Detection](Lecture3_step2_Onset_Beat_Detection.ipnb) demonstrates the use of Essentia onset detection functions (using HFC and complex spectral difference) and a beat-tracker.
* [Lecture3_step3_Tempogram_autoCorr](Lecture3_step3_Tempogram_autoCorr.ipynb) includes a simple tempogram computation and demonstration

## Lecture 4:
Lecture 4 considers MIR for mon-Western music traditions:
* [Lecture4_1_downloadAllSARAGAContent](Lecture4_1_downloadAllSARAGAContent.ipynb) includes sample code to download Hindustani and Carnatic music data from CompMusic servers
* [Lecture4_2_visualizeAnnotations](Lecture4_2_visualizeAnnotations.ipynb) aims at demonstrating some of the contents of Saraga database annotations: sections, typical phrases, sama and tempo annotations.
* [Lecture4_3_tuningAnalysis_SingleRecording](Lecture4_3_tuningAnalysis_SingleRecording.ipynb) considers tuning analysis of a recording of Turkish makam music and [Lecture4_4_tuningAnalysis_SetOfRecordings](Lecture4_4_tuningAnalysis_SetOfRecordings.ipynb) does the same job and merges the outputs to gather information required for building a makam scale model. 

## Lecture 5:
Introduction to MIR using symbolic data
* [Lecture5_music21_intro](Lecture5_music21_intro.ipynb) is a very short introduction to music21, a toolkit for computational aided musicology
* [Lecture5_melodicSegmentation](Lecture5_melodicSegmentation.ipynb) Melodic segmentation using Local Boundary Detection Model (LBDM by Cambouropoulos, E. (2001)).
* [Lecture5_matchingTimeSeriesData](Lecture5_matchingTimeSeriesData.ipynb) discusses the problem of matching time-series data (such as finding short melody sequences within songs)

... to be continued