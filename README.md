## SexTok Dataset

[Paper @ ACL 2023](https://aclanthology.org/2023.findings-acl.365/) | [Data](data/) | [Workshop For Online Abuse and Harms](https://web.archive.org/web/20231207030147/https://www.workshopononlineabuse.com/programme.html) | [Video](https://aclanthology.org/2023.findings-acl.365.mp4)
  
It’s not Sexually Suggestive; It’s Educative | Separating Sex Education from Suggestive Content on TikTok videos (George & Surdeanu, Findings 2023)

### Example 

<img src="docs/images/example.png" alt="Example" width="500">

### Results
| Methods               | Accuracy | **Micro** Precision | **Micro** Recall | **Micro** F1 | **Macro** Precision | **Macro** Recall | **Macro** F1 |
|-----------------------|----------|---------------------|------------------|--------------|----------------------|------------------|--------------|
| All–text Bert         | 68%      | 76%                | 50%             | 60%         | 71%                 | 63%             | 64%         |
| Non–empty Text Bert   | 75%      | 78%                | 54%             | 64%         | 74%                 | 65%             | 68%         |
| Visual–VideoMAE       | 70%      | 61%                | 51%             | 55%         | 68%                 | 57%             | 61%         |
| Slowfast*              | 80%      | 95%                | 63%             | 76%         | 81%                 | 73%             | 76%         |
| Timesformer*           | 75%      | 93%                | 52%             | 66%         | 75%                 | 65%             | 68%         |
| ResNet*               | 77%      | 90%                | 75%             | 63%         | 77%                 | 64%             | 67%         |
| Uniformer*           | 74%      | 93%                | 55%             | 69%         | 73%                 | 66%             | 68%         |
| **[Zhou, Di, et al(2025)*](https://dl.acm.org/doi/abs/10.1007/978-981-96-5809-1_10)**                  | **86%**  | **97%**            | **81%**         | **88%**     | **85%**             | **84%**         | **84%**     |

Results marked with * are reported from the Zhou, Di, et al(2025) paper.

### Publications Using SexTok

| Year | Paper                                                                                                               | 
| ---- | ------------------------------------------------------------------------------------------------------------------- | 
| 2025 | Balle, Mary et al. **[“Choking on TikTok: Memetic Content and CRAAP Analysis of Educative and Entertaining #Chokekink Videos.”](https://pubmed.ncbi.nlm.nih.gov/40960736/)** Journal of sex research, 1-19. 17 Sep. 2025, doi:10.1080/00224499.2025.2550014 | 
| 2025 | Zhou, Di, et al. **"[Consensus-Aware Balance Learning for Sexually Suggestive Video Classification.](https://dl.acm.org/doi/abs/10.1007/978-981-96-5809-1_10)"** International Conference on Computational Visual Media. Singapore: Springer Nature Singapore, 2025. |

*If you’ve used SexTok in your work, we would love to know! Please email us enfafane \< at \> gmail.com to be included!*

### Citation  
 ```
@inproceedings{george-surdeanu-2023-sexually,
    title = "It{'}s not Sexually Suggestive; It{'}s Educative | Separating Sex Education from Suggestive Content on {T}ik{T}ok videos",
    author = "George, Enfa  and
      Surdeanu, Mihai",
    editor = "Rogers, Anna  and
      Boyd-Graber, Jordan  and
      Okazaki, Naoaki",
    booktitle = "Findings of the Association for Computational Linguistics: ACL 2023",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.findings-acl.365/",
    doi = "10.18653/v1/2023.findings-acl.365",
    pages = "5904--5915",
    abstract = "We introduce SexTok, a multi-modal dataset composed of TikTok videos labeled as sexually suggestive (from the annotator{'}s point of view), sex-educational content, or neither. Such a dataset is necessary to address the challenge of distinguishing between sexually suggestive content and virtual sex education videos on TikTok. Children{'}s exposure to sexually suggestive videos has been shown to have adversarial effects on their development (Collins et al. 2017). Meanwhile, virtual sex education, especially on subjects that are more relevant to the LGBTQIA+ community, is very valuable (Mitchell et al. 2014). The platform{'}s current system removes/punishes some of both types of videos, even though they serve different purposes. Our dataset contains video URLs, and it is also audio transcribed. To validate its importance, we explore two transformer-based models for classifying the videos. Our preliminary results suggest that the task of distinguishing between these types of videos is learnable but challenging. These experiments suggest that this dataset is meaningful and invites further study on the subject."
}
 ```
