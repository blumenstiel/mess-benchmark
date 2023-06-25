---
title: "Leaderboard"
permalink: "/leaderboard/"
layout: page
---

Our evaluation focus on zero-shot transfer models as they are designed to generalize to unseen datasets. We evaluated eight model architectures with publicly available weights on the MESS benchmark.
We present the aggregated results in the following table and refer to the supplementary material of our paper for the dataset-wise results.

# Zero-shot semantic segmentation

| Model                                                                        |   General |   Earth Monitoring |   Medical Sciences | Engineering |   Agriculture and Biology |   Mean |
|:-----------------------------------------------------------------------------|----------:|-------------------:|-------------------:|------------:|--------------------------:|-------:|
| Random<sup>1</sup>                                                           |      1.17 |               7.11 |              29.51 |       11.71 |                      6.14 |  10.27 |
| Best supervised<sup>2</sup>                                                  |     49.15 |              79.12 |              89.49 |       67.66 |                     81.94 |  71.13 |
| [ZSSeg-B](https://github.com/MendelXu/zsseg.baseline)                        |     19.98 |              17.98 |              41.82 |        14.0 |                     22.32 |  22.73 |
| [ZegFormer-B](https://github.com/dingjiansw101/ZegFormer)                    |     13.57 |              17.25 |              17.47 |       17.92 |                     25.78 |  17.57 |
| [X-Decoder-T](https://github.com/microsoft/X-Decoder)                        |     21.99 |              18.92 |              23.25 |       15.31 |                     19.05 |  19.91 |
| [SAN-B](https://github.com/MendelXu/SAN)                                     |     29.35 |              30.64 |              29.85 |       23.58 |                     15.07 |  26.74 |
| [OpenSeeD-T](https://github.com/IDEA-Research/OpenSeeD)                      |     22.31 |              25.14 |              44.43 |       16.69 |                     10.53 |  24.35 |
| [CAT-Seg-B](https://github.com/KU-CVLAB/CAT-Seg)                             |     34.96 |              34.57 |              41.65 |       26.26 |                     29.32 |  33.74 |
| [Grounded-SAM-B](https://github.com/IDEA-Research/Grounded-Segment-Anything) |     29.51 |              25.97 |              37.38 |       29.51 |                     17.66 |  28.52 |
| [OVSeg-L](https://github.com/facebookresearch/ov-seg)                        |     29.54 |              29.04 |              31.9  |       14.16 |                     28.64 |  26.94 |
| [SAN-L](https://github.com/MendelXu/SAN)                                     |     36.18 |              38.83 |              30.27 |       16.95 |                     20.41 |  30.06 |
| [CAT-Seg-L](https://github.com/KU-CVLAB/CAT-Seg)                             |     39.93 |              39.85 |              48.49 |       26.04 |                     34.06 |  38.14 |
| [Grounded-SAM-L](https://github.com/IDEA-Research/Grounded-Segment-Anything) |     30.32 |              26.44 |              38.69 |       29.25 |                     17.73 |  29.05 |
| [CAT-Seg-H](https://github.com/KU-CVLAB/CAT-Seg)                             |     37.98 |              37.74 |              34.65 |       29.04 |                     37.76 |  35.66 |
| [Grounded-SAM-H](https://github.com/IDEA-Research/Grounded-Segment-Anything) |     30.27 |              26.44 |              38.45 |       28.16 |                     17.67 |  28.78 |

<small><sup>1</sup> Random is a lower bound. The values represent the expected mIoU from predictions with uniform class distribution.</small>

<small><sup>2</sup> Supervised are recent supervised models for each dataset individually. We refer to our paper for the details.</small>

# Zero-shot point-to-mask semantic segmentation

# Zero-shot box-to-mask semantic segmentation