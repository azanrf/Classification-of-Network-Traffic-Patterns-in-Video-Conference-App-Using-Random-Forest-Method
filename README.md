# Classification of Network Traffic Patterns in Video Conference Application Using Random Forest Method

Implementation Random Forest for Network Traffic Pattertn Classification on Video Conference Application.
- Software that i use:
  - Zoom
  - Wireshark
  - Netlimiter
  - Jupyter Notebook

My own Experimental scenario:
|Experiment     |Bandwidth      |video Conference App|Duration|
|:---:          |:---:          |:---:               |:---:   |
| Data 1        | 16KB          |Zoom                |5 Minute|
| Data 2        | 32KB          |Zoom                |5 Minute|
| Data 3        | 64KB          |Zoom                |5 Minute|
| Data 4        | 128KB         |Zoom                |5 Minute|

After the data is collected, I determine the data labels based on the Quality of Service (TIPHON):
|Experiment|Throughput|Packet Loss|Delay|Jitter|Index|Labels|
|:---:     |:---:     |:---:      |:---:|:---: |:---:|:---: |
| Data 1   |1         |3          |4    |3     |2.75 |0     |
| Data 2   |1         |3          |4    |3     |2.75 |0     |
| Data 3   |3         |3          |4    |3     |3.25 |1     |
| Data 4   |3         |3          |4    |3     |3.25 |1     |

The parameter of Random Forest that i use:
|Experiment  |max_depth|n_estimators|criterion|
|:---:       |:---:    |:---:       |:---:    |
|Experiment 1|2        |50          |gini     |
|Experiment 2|3        |50          |gini     |
|Experiment 3|4        |50          |gini     |
|Experiment 4|2        |100         |gini     |
|Experiment 5|3        |100         |gini     |
|Experiment 6|4        |100         |gini     |

### Result Confusion Matrix
- Confusion Matrix Experiment 1:
  - |10028|3165 |
    |:---:|:---:| 
    |**1535** |**22272**|
- Confusion Matrix Experiment 2:
  - |11129|2064 |
    |:---:|:---:| 
    |**73** |**23734**|
- Confusion Matrix Experiment 3:
  - |12151|1042 |
    |:---:|:---:| 
    |**89** |**23718**|
- Confusion Matrix Experiment 4:
  - |11211|1982 |
    |:---:|:---:| 
    |**68** |**23739**|
- Confusion Matrix Experiment 5:
  - |11815|1378 |
    |:---:|:---:| 
    |**82** |**23725**|
- Confusion Matrix Experiment 6:
  - |13009|184 |
    |:---:|:---:| 
    |**70** |**23921**|    
    
### Result with Accuracy, TPR, FPR, TNR, and FNR
|Experiment  |Accuracy |TPR   |FPR   |FPR   |TNR   |FNR   |
|:---:       |:---:    |:---: |:---: |:---: |:---: |:---: |
|Experiment 1|87%      |87%   |23%   |23%   |76%   |6%    |
|Experiment 2|94%      |91%   |15%   |23%   |84%   |0.3%  |
|Experiment 3|96%      |95%   |7%    |23%   |92%   |0.3%  |
|Experiment 4|94%      |92%   |15%   |23%   |84%   |0.2%  |
|Experiment 5|96%      |94%   |10%   |23%   |89%   |0.3%  |
|Experiment 6|99%      |99%   |1%    |23%   |98%   |0.2%  |

### 📫 How to reach me:
<p align="left"> 
  <a href="https://www.linkedin.com/in/muhammad-rizki-fauzaan-a32a94176/" target="_blank"><img align="left" alt="Muhammad Rizki Fauzaan | Linkedin" src="https://img.shields.io/badge/LinkedIn-%230077B5.svg?&style=flat-square&logo=linkedin&logoColor=white"/></a>
  <a href="https://twitter.com/azanrf" target="_blank" target="_blank"><img align="left" alt="azanrf | Twitter" src="https://img.shields.io/badge/Twitter-%231877F2.svg?&style=flat-square&logo=twitter&logoColor=white"/></a>
  <a href="https://www.instagram.com/rizki.fauzaan/" target="_blank"><img align="left" alt="Muhammad Rizki Fauzaan | Instagram" src="https://img.shields.io/badge/Instagram-%23E4405F.svg?&style=flat-square&logo=instagram&logoColor=white" alt="Instagram"/></a>
  <a href="https://www.facebook.com/azanrf" target="_blank"><img align="left" alt="azanrf | Facebook" src="https://img.shields.io/badge/Facebook-%231877F2.svg?&style=flat-square&logo=facebook&logoColor=white" alt="Facebook"/></a>
  <a href="https://open.spotify.com/user/azanrf" target="_blank"><img align="left" alt="azanrf | Spotify" src="https://img.shields.io/badge/Spotify-%231ED760.svg?&style=flat-square&logo=spotify&logoColor=white" alt="Spotify"></a>
  <a href="mailto:rizkifauzaan08@gmail.com" target="_blank"><img align="left" alt="Muhammad Rizki Fauzaan | Gmail" src="https://img.shields.io/badge/-rizkifauzaan08@gmail.com-D14836?style=flat-square&logo=Gmail&logoColor=white"/></a>
</p>
