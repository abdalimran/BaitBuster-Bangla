# BaitBuster-Bangla: A Comprehensive Dataset for Clickbait Detection in Bangla with Multi-Feature and Multi-Modal Analysis

## Description
This dataset is a multi-feature and multi-modal dataset for Bangla clickbait detection in video sharing platforms. The dataset is collected from YouTube using its official public API with the objective of classifying clickbait content in the Bangla language. The dataset consists of 253,070 entries with 18 columns covering a curated list of 28 Not Clickbait, and 26 Clickbait Bangla youtube channels. The dataset provides valuable information for studying clickbait content and includes various metadata related to the videos, user engagement statistics, and labels. The dataset has been labeled in three different strategies: i) pre-defined auto labels, ii) labels by human annotator, and iii) labels by fine-tuned AI model. However, human labels are are available for 10000 entries. The dataset is available in three different formats: xlsx, csv, and parquet.

## Data Dictionary

| **Feature Type**          | **Feature Name**     | **Data Type** | **Definition**                                               |
|----------------------------|----------------------|---------------|--------------------------------------------------------------|
| Metadata                   | channel_id           | string        | ID of the YouTube channel                                    |
| Metadata                   | channel_name         | string        | Name of the YouTube channel                                  |
| Metadata                   | channel_url          | string        | URL of the YouTube channel                                   |
| Metadata                   | video_id             | string        | ID of the video                                              |
| Metadata                   | publishedAt          | datetime      | Date and time when the video   was published                 |
| Primary   Data             | title                | string        | Title of the video                                           |
| Primary   Data (Processed) | title_debiased       | string        | Debiased title of the video                                  |
| Primary   Data             | description          | string        | Debiased description of the   video                          |
| Primary   Data (Processed) | description_debiased | string        | Description of the YouTube   video without bias              |
| Metadata                   | url                  | string        | URL of the video                                             |
| Engagement   Stats         | viewCount            | int           | Number of views the video has   received                     |
| Engagement   Stats         | commentCount         | int           | Number of comments on the video                              |
| Engagement   Stats         | likeCount            | int           | Number of likes on the video                                 |
| Engagement   Stats         | dislikeCount         | int           | Number of dislikes on the video                              |
| Metadata                   | thumbnails           | string        | URL of the thumbnail for the   video                         |
| Label                      | auto_labeled         | string        | Automatically labeled using   manual review                  |
| Label   (Processed)        | human_labeled        | string        | Labeled by human                                             |
| Label   (Processed)        | ai_labeled           | string        | Labeled by an AI model   fine-tuned on human labeled data    |

## Paper
* **Data in Brief**: https://doi.org/10.1016/j.dib.2024.110239
* **arXiv Link**: https://arxiv.org/abs/2310.11465

## Dataset
* **Mendeley**: https://data.mendeley.com/datasets/3c6ztw5nft/
* **Kaggle**: https://www.kaggle.com/datasets/abdalimran/baitbuster-bangla
* **Huggingface**: https://huggingface.co/datasets/abdalimran/BaitBuster-Bangla

## Citation
### MLA
```Al Imran, Abdullah, Md Sakib Hossain Shovon, and M. F. Mridha. "BaitBuster-Bangla: A Comprehensive Dataset for Clickbait Detection in Bangla with Multi-Feature and Multi-Modal Analysis." Data in Brief (2024): 110239.```

### BibText
```
@article{IMRAN2024110239,
title = {BaitBuster-Bangla: A Comprehensive Dataset for Clickbait Detection in Bangla with Multi-Feature and Multi-Modal Analysis},
journal = {Data in Brief},
pages = {110239},
year = {2024},
issn = {2352-3409},
doi = {https://doi.org/10.1016/j.dib.2024.110239},
url = {https://www.sciencedirect.com/science/article/pii/S2352340924002105},
author = {Abdullah Al Imran and Md Sakib Hossain Shovon and M.F. Mridha},
keywords = {Bangla clickbait dataset, YouTube clickbait, Multi-modal clickbait dataset, Multi-feature clickbait dataset, Bangla natural language processing, User behavior modeling, Social Media Analysis},
abstract = {This study presents a large multi-modal Bangla YouTube clickbait dataset consisting of 253,070 data points collected through an automated process using the YouTube API and Python web automation frameworks. The dataset contains 18 diverse features categorized into metadata, primary content, engagement statistics, and labels for individual videos from 58 Bangla YouTube channels. A rigorous preprocessing step has been applied to denoise, deduplicate, and remove bias from the features, ensuring unbiased and reliable analysis. As the largest and most robust clickbait corpus in Bangla to date, this dataset provides significant value for natural language processing and data science researchers seeking to advance modeling of clickbait phenomena in low-resource languages. Its multi-modal nature allows for comprehensive analyses of clickbait across content, user interactions, and linguistic dimensions to develop more sophisticated detection methods with cross-linguistic applications.}
}
```
