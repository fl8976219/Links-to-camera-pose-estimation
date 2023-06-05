# Links-to-camera-pose-estimation
camera pose estimation

# Useful links
1. http://aag.ciirc.cvut.cz/minimal/ (计算机视觉中的最小问题清单，包括了很多的位姿估计的论文)


# some papers
1. A Direct Least-Squares Solution to the PnP Problem with Unknown Focal Length (<https://openaccess.thecvf.com/content_cvpr_2016/papers/Zheng_A_Direct_Least-Squares_CVPR_2016_paper.pdf>)
2. A fast minimal solver for absolute camera pose with unknown focal length and radial distortion from four planar points (<https://arxiv.org/pdf/1805.10705.pdf>)
## 线匹配
1. Camera Pose Estimation from Lines using Plücker Coordinates (<http://www.bmva.org/bmvc/2015/papers/paper045/index.html>)
2. Globally Optimal Camera Orientation Estimation from Line Correspondences by BnB algorithm (<https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9258393>)



# github
1. <https://github.com/hamburgerlady> (A fast minimal solver for absolute camera pose with unknown focal length and radial distortion from four planar points论文的作者，他的仓库中还包括了径向畸变的解决。)
2. https://github.com/GrumpyZhou/visloc-apr （PoseNet，深度学习的方式求位姿）
3. https://github.com/sebhaner/refractive_pose
4. https://github.com/Liumouliu/p2p_vertical_direction
5. https://github.com/Liu-Yinlong/Ro_PnL (绝对相机姿态估计,通过线匹配来做)
6. https://github.com/vlarsson/PoseLib (包含了求位姿（绝对位姿、相对位姿）的各种情况，如图所示，是绝对位姿的情况)
  | Solver        | Point-Point | Point-Line | Line-Point | Line-Line | Upright | Generalized | Approx. runtime | Max. solutions | Comment                                                      |
  | ------------- | ----------- | ---------- | ---------- | --------- | ------- | ----------- | --------------- | -------------- | ------------------------------------------------------------ |
  | `p3p`         | 3           | 0          | 0          | 0         |         |             | 250 ns          | 4              | Persson and Nordberg, LambdaTwist (ECCV18)                   |
  | `gp3p`        | 3           | 0          | 0          | 0         |         | ✔️           | 1.6 us          | 8              | Kukelova et al., E3Q3 (CVPR16)                               |
  | `gp4ps`       | 4           | 0          | 0          | 0         |         | ✔️           | 1.8 us          | 8              | Unknown scale.  Kukelova et al., E3Q3 (CVPR16) Camposeco et al.(ECCV16) |
  | `p4pf`        | 4           | 0          | 0          | 0         |         |             | 2.3 us          | 8              | Unknown focal length.  Kukelova et al., E3Q3 (CVPR16)        |
  | `p2p2pl`      | 2           | 2          | 0          | 0         |         |             | 30 us           | 16             | Josephson et al. (CVPR07)                                    |
  | `p6lp`        | 0           | 0          | 6          | 0         |         |             | 1.8 us          | 8              | Kukelova et al., E3Q3 (CVPR16)                               |
  | `p5lp_radial` | 0           | 0          | 5          | 0         |         |             | 1 us            | 4              | Kukelova et al., (ICCV13)                                    |
  | `p2p1ll`      | 2           | 0          | 0          | 1         |         |             | 1.6 us          | 8              | Kukelova et al., E3Q3 (CVPR16), Zhou et al. (ACCV18)         |
  | `p1p2ll`      | 1           | 0          | 0          | 2         |         |             | 1.7 us          | 8              | Kukelova et al., E3Q3 (CVPR16), Zhou et al. (ACCV18)         |
  | `p3ll`        | 0           | 0          | 0          | 3         |         |             | 1.8 us          | 8              | Kukelova et al., E3Q3 (CVPR16), Zhou et al. (ACCV18)         |
  | `up2p`        | 2           | 0          | 0          | 0         | ✔️       |             | 65 ns           | 2              | Kukelova et al. (ACCV10)                                     |
  | `ugp2p`       | 2           | 0          | 0          | 0         | ✔️       | ✔️           | 65 ns           | 2              | Adapted from Kukelova et al. (ACCV10)                        |
  | `ugp3ps`      | 3           | 0          | 0          | 0         | ✔️       | ✔️           | 390 ns          | 2              | Unknown scale. Adapted from Kukelova et al. (ACCV10)         |
  | `up1p2pl`     | 1           | 2          | 0          | 0         | ✔️       |             | 370 ns          | 4              |                                                              |
  | `up4pl`       | 0           | 4          | 0          | 0         | ✔️       |             | 1.4 us          | 8              | Sweeney et al. (3DV14)                                       |
  | `ugp4pl`      | 0           | 4          | 0          | 0         | ✔️       | ✔️           | 1.4 us          | 8              | Sweeney et al. (3DV14)                                       |

7. 


