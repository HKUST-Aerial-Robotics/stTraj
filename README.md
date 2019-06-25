# stTraj
Spatial-temporal Trajectory Planning for UAV Teach-and-Repeat

## 1.Introduction
we propose a novel motion planning framework for quadrotor teach-and-repeat applications. Instead of controlling the drone to precisely follow the teaching path, our method converts an arbitrary jerky human-piloted trajectory to a topologically equivalent one, which is guaranteed to be safe, smooth, and kinodynamically feasible with an expected aggressiveness. Our proposed planning framework optimizes the trajectory in both spatial and temporal aspects. In the spatial layer, a flight corridor is found to represent the free space which is topologically equivalent with the teaching path. Then a minimum-jerk piecewise trajectory is generated within the flight corridor. In the temporal layer, the trajectory is reparameterized to obtain a minimum-time temporal trajectory under kinodynamic constraints. The spatial and temporal optimizations are both formulated as convex programs and are done iteratively. The proposed method is integrated into a complete quadrotor system and is validated to perform aggressive flights in challenging indoor and outdoor environments.For details we refer readers to our paper.

**Authors:**[Fei Gao](https://ustfei.com/) and [Shaojie Shen](http://www.ece.ust.hk/ece.php/profile/facultydetail/eeshaojie) from the [HUKST Aerial Robotics Group](uav.ust.hk).

**Disclaimer**

This is research code, any fitness for a particular purpose is disclaimed.

**Related Paper**
* **Optimal Trajectory Generation for Quadrotor Teach-and-Repeat**, Fei Gao, Luqi Wang, Kaixuan Wang, William Wu, Boyu Zhou, Luxin Han, and Shaojie Shen, **IEEE Robotics and Automation Letters (RA-L)**, 4(2), 1493-1500, 2019.

Video of this paper can be found at:

<a href="https://www.youtube.com/watch?v=ehoJi4K_QKE" 
target="_blank"><img src="https://img.youtube.com/vi/ehoJi4K_QKE/0.jpg" 
alt="video" width="752" height="480" border="10" /></a>

If you use this planning framework for your academic research, please cite our related paper.
```
@article{gao2019optimal,
  title={Optimal Trajectory Generation for Quadrotor Teach-and-Repeat},
  author={Gao, Fei and Wang, Luqi and Wang, Kaixuan and Wu, William and Zhou, Boyu and Han, Luxin and Shen, Shaojie},
  journal={IEEE Robotics and Automation Letters},
  volume={4},
  number={2},
  pages={1493--1500},
  year={2019},
  publisher={IEEE}
}
```
## 2. Updates

We have advanced our Teach-and-Repeat system as a complete and robust **Teach-Repeat-Replan** system which can deal with changing environments, moving obstacls and imperfect localization. We are cleanning our code and will release all components (global/local perception, global/local planning, global/local state estimation and onboard controller) soon at:
https://github.com/HKUST-Aerial-Robotics/uavTeachRepeatReplan

We promise to release our code by the end of June, 2019

The **Teach-Repeat-Replan** system contains all functionalities of this repo. Any further questions can be raised at that repo. Thanks.
