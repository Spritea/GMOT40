# GMOT-40 Benchmark
[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This is the official development project for paper: [GMOT-40: A Benchmark for Generic Multiple Object Tracking](https://arxiv.org/abs/2011.11858).

To get the dataset, including sequences and labels, please go to the [official website](https://spritea.github.io/GMOT40).

<img src="sample.png">

## Abstract
Multiple Object Tracking (MOT) has witnessed remarkable advances in recent years. However, existing studies dominantly request prior knowledge of the tracking target (eg, pedestrians), and hence may not generalize well to unseen categories. In contrast, Generic Multiple Object Tracking (GMOT), which requires little prior information about the target, is largely under-explored. In this paper, we make contributions to boost the study of GMOT in three aspects. First, we construct the first publicly available dense GMOT dataset, dubbed GMOT-40, which contains 40 carefully annotated sequences evenly distributed among 10 object categories. In addition, two tracking protocols are adopted to evaluate different characteristics of tracking algorithms. Second, by noting the lack of devoted tracking algorithms, we have designed a series of baseline GMOT algorithms. Third, we perform a thorough evaluations on GMOT-40, involving popular MOT algorithms (with necessary modifications) and the proposed baselines.

## Baseline
Below are the results of baseline methods with one-shot GMOT protocol. We randomly
sample the one target in the 1st frame for the protocol and repeat this procedure for 5 times. Then we report the mean and standard deviation of the results over these 5 experiments.

| Methods | MOTA | MOTP  | IDF1 |
|-------|-------|-------| -------|
| [MDP](https://www.cv-foundation.org/openaccess/content_iccv_2015/papers/Xiang_Learning_to_Track_ICCV_2015_paper.pdf) | 19.92%	&plusmn; 1.84%  | 24.16% &plusmn; 0.27%  | 31.84%	&plusmn; 2.23%  | 
| [DeepSORT](https://arxiv.org/pdf/1703.07402.pdf) | 14.98%	&plusmn; 1.47%  | 23.66% &plusmn; 0.53%  | 25.38%	&plusmn; 2.32%  | 
| [IOU Tracker](http://elvera.nue.tu-berlin.de/typo3/files/1517Bochinski2017.pdf) | 12.36%	&plusmn; 1.60%  | 25.34% &plusmn; 0.36%  | 20.90%	&plusmn; 2.73%  | 
| [FAMNet](https://openaccess.thecvf.com/content_ICCV_2019/papers/Chu_FAMNet_Joint_Learning_of_Feature_Affinity_and_Multi-Dimensional_Assignment_for_ICCV_2019_paper.pdf) | 17.60%	&plusmn; 0.85%  | 22.56% &plusmn; 0.23%  | 27.76%	&plusmn; 1.16%  | 

## Citation 
The proceeding version is shown below. You may check the [arXiv version](https://arxiv.org/abs/2011.11858) for updates.

```
@inproceedings{bai2021gmot,
  title={GMOT-40: A Benchmark for Generic Multiple Object Tracking},
  author={Bai, Hexin and Cheng, Wensheng and Chu, Peng and Liu, Juehuan and Zhang, Kai and Ling, Haibin},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  pages={6719--6728},
  year={2021}
}
```

## Notes
Although we tried to make the annotation quality as high as possible, there is still room for improvement, due to personal bias, etc. We would continue to improve the annotation quality since the first release. 

If you find any inproper label/have better annotation ideas, please contact Wensheng Cheng by Email: wenscheng at cs.stonybrook.edu.

Your effort would be greatly appreciated, and the person whose improvement is adopted would be added to a contribution list!

## License
<!-- Shield: [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa] -->

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

<!-- [![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa] -->

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
<!-- [cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png -->
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg