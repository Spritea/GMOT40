# GMOT-40
This is the development project for paper: [GMOT-40: A Benchmark for Generic Multiple Object Tracking](https://arxiv.org/abs/2011.11858).

The official website, including sequences and labels, is provided [here](https://spritea.github.io/GMOT40).

<img src="sample.png" width="600">

## Abstract

Multiple Object Tracking (MOT) has witnessed remarkable advances in recent years. However, existing studies dominantly request prior knowledge of the tracking target (eg, pedestrians), and hence may not generalize well to unseen categories. In contrast, Generic Multiple Object Tracking (GMOT), which requires little prior information about the target, is largely under-explored. In this paper, we make contributions to boost the study of GMOT in three aspects. First, we construct the first publicly available dense GMOT dataset, dubbed GMOT-40, which contains 40 carefully annotated sequences evenly distributed among 10 object categories. In addition, two tracking protocols are adopted to evaluate different characteristics of tracking algorithms. Second, by noting the lack of devoted tracking algorithms, we have designed a series of baseline GMOT algorithms. Third, we perform a thorough evaluations on GMOT-40, involving popular MOT algorithms (with necessary modifications) and the proposed baselines.

## Baseline

| Methods | MOTA | MOTP  | IDF1 |
|-------|--------|--------| ----|
| MDP | 19.92%	$\pm$1.84% | 67.1 | 1097 | 
| DeepSORT | 68.7 | 66.3 | 3378 | 
| IOU tracker | 69.8 | 67.1 | 1097 | 
| FAMNet | 68.7 | 66.3 | 3378 | 

## Citation 

```
@article{bai2020gmot,
  title={GMOT-40: A Benchmark for Generic Multiple Object Tracking},
  author={Bai, Hexin and Cheng, Wensheng and Chu, Peng and Liu, Juehuan and Zhang, Kai and Ling, Haibin},
  journal={arXiv preprint arXiv:2011.11858},
  year={2020}
}
```

## Notes
Although we tried to make the annotation quality as high as possible, there is still room for improvement, due to personal bias, etc. We would continue to improve the annotation quality since the first release. 

If you find any inproper label/have better annotation ideas, please contact Wensheng Cheng: wenscheng@cs.stonybrook.edu.

Your effort would be greatly appreciated, and the person whose improvement is adopted would be added to a contribution list.
