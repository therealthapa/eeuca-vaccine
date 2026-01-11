# Shared Task on Multimodal Vaccine Critical Meme Detection (VaxMeme) at EEUCA 2026

Competition Link:

[Codabench](https://www.codabench.org/competitions/12085/)

**Multimodal Vaccine Critical Meme Detection**

Memes have become a powerful and fast-spreading medium for sharing information online, especially around high-impact public health issues such as COVID-19 vaccination. While memes can be used to promote awareness and positive behavior, they are also frequently used to spread misinformation, skepticism, and vaccine-critical narratives, often through sarcasm and implicit context that make automated analysis challenging. This shared task is based on the VaxMeme dataset, a collection of over 10,000 manually annotated vaccination-related memes, designed to support multimodal vaccine-critical meme detection. The task invites participants to develop models that jointly leverage both visual and textual representations to capture the global and local contextual cues embedded in memes. By focusing on fine-grained multimodal understanding, this challenge aims to advance more reliable systems for monitoring vaccine-related discourse, supporting myth debunking efforts, and informing the design of effective public health communication strategies on social media platforms.

## Task

**Vaccine Stance Classification:** The aim is to classify the stance of a given meme towards vaccination. The dataset for this task uses the following labels: *Pro-vaccine*, *Vaccine critical*, and *Neutral*.

**To learn more about the dataset**: please refer to the [VaxMeme paper](https://dl.acm.org/doi/10.1145/3539597.3570450).

## Participation

Join our Codabench competition: [Codabench link](https://www.codabench.org/competitions/12085/)

## Dataset

All the memes have a unique identifier called "index". The labels for training data are organized in the folder provided. For evaluation and testing, the submission format is mentioned below.

**Data**

  * [Training Data](https://drive.google.com/drive/folders/1lNIYxygV1ofUklPMyo26UvVnN7lLLZNg?usp=sharing)
  * [Evaluation Data (Without Labels)](https://drive.google.com/drive/folders/1e4UIJLiMUNAbYVg2CopsUPwswv-WJeXl?usp=sharing)

## Use of External Data

The use of external datasets is permitted. You should also mention your external data usage in your paper write-up. Participants may find datasets such as MMCoVaR or other meme analysis datasets useful for transfer learning experiments.

## Evaluation

All the images have a unique identifier called "index". The labels for training data are organized in the folder provided. For evaluation and testing, the script takes one prediction file as input. 

Your submission file must be a .csv file named ‘predictions.csv’ with columns 'index' and ‘label’. You must zip this file and submit the zipped archive file. Ensure that the zip does not have any sub-directories or any files besides the 'predictions.csv' file. The system only recognizes the first file in the zip folder. Ensure that the index order in the submission file is in ascending order. A sample submission file is available [here](https://github.com/therealthapa/eeuca-vaccine/blob/main/sample_submission.csv).

| index | label |
|----------|----------|
|12345.jpg|	0|
|15001.jpg|	1|
|20524.jpg|	1|
|35231.jpg|	0|
|65102.jpg|	1|

The labels should be mapped to the following integers:

  * 0: *Vaccine critical*
  * 1: *Neutral*
  * 2: *Pro-vaccine*

The performance will be ranked by **F1-score** (Macro).

## Publication

Participants in the Shared Task are expected to submit a paper to the EEUCA 2026 workshop. Papers must follow the workshop submission instructions and will undergo regular peer review. Their acceptance will not depend on the results obtained in the shared task but on the quality of the paper. All the accepted papers will be published in the ACL Anthology.

## Timeline of the Events

  * Start of the Competition: Dec 10, 2025
  * Eval Phase Start: Dec 10, 2025
  * Test Phase Start: Jan 15, 2026
  * Test Phase End: March 15, 2026
  * Paper Submission Deadline: March 28, 2026
  * Notification of acceptance: April 28, 2026
  * Camera-ready paper due: May 12, 2026

## Organizers

* Surendrabikram Thapa (Virginia Tech, USA)
* Shuvam Shiwakoti (Virginia Tech, USA)
* Siddhant Bikram Shah (Northeastern University, USA)
* Kritesh Rauniyar (Delhi Technological University, India)
* Surabhi Adhikari (Columbia University, USA)
* Kristina T. Johnson (Northeastern University, USA)
* Hristo Tanev (European Commission, Joint Research Centre (EU JRC)
* Ali Hürriyetoğlu (Wageningen Food Safety Research, Netherlands)
* Usman Naseem (Macquarie University, Australia)

## Contact

If there are any questions related to the competition, please contact the organizers at rauniyark11@gmail.com. Participants in this shared task are encouraged to reach out with any concerns or questions to any of the shared task organizers.

## References

Naseem, U., Kim, J., Khushi, M., & Dunn, A. G. (2023, February). A multimodal framework for the identification of vaccine critical memes on Twitter. In Proceedings of the Sixteenth ACM International Conference on Web Search and Data Mining (pp. 706-714).
