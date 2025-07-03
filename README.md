#  Test Video Dataset Description

This repository contains a collection of **indoor and outdoor surveillance videos** used for evaluating our proposed scheme. The datasets are sourced from **UrbanTracker** and **Wisenet** projects.

---

## Outdoor Videos

### 1. Outdoor Video 1 (OV1) – *René Lévesque*
- **Source:** [UrbanTracker](https://www.jpjodoin.com/urbantracker/dataset.html)
- **Description:** Captures an office building and three nearby intersections. Each scene contains around **20 moving objects**.
- **Resolution:** 1280 × 720  
- **Frames:** 1000  
- **Codec:** H.264  
- **FPS:** 30  

### 2. Outdoor Video 2 (OV2) – *St Marc*
- **Source:** [UrbanTracker](https://www.jpjodoin.com/urbantracker/dataset.html)
- **Description:** Captures the Saint Marc and Maisonneuve intersection in Montréal, with **up to 14 moving objects**, including vehicles, bicycles, and pedestrians.
- **Resolution:** 1280 × 720  
- **Frames:** 1000  
- **Codec:** H.264  
- **FPS:** 30  

### 3. Outdoor Video 3 (OV3) – *Sherbrooke*
- **Source:** [UrbanTracker](https://www.jpjodoin.com/urbantracker/dataset.html)
- **Description:** Captures the Sherbrooke/Amherst intersection from a **low-angle CCTV camera**, showing **cars and pedestrians**, with ~7 objects per scene.
- **Resolution:** 800 × 600  
- **Frames:** 1001  
- **Codec:** H.264  
- **FPS:** 30  

---

## Indoor Videos

### 4. Indoor Video 1 (IV1) – *Wisenet - video2_1.avi*
- **Source:** [Wisenet Dataset (Kaggle)](https://www.kaggle.com/datasets/abdelrhmannile/wisenet?resource=download)
- **Description:** Captured by an indoor CCTV camera from `set_2/video2_1.avi`.
- **Resolution:** 1280 × 720  
- **Codec:** Xvid MPEG-4  
- **FPS:** 30  

### 5. Indoor Video 2 (IV2) – *Wisenet - video2_3.avi*
- **Source:** [Wisenet Dataset (Kaggle)](https://www.kaggle.com/datasets/abdelrhmannile/wisenet?resource=download)
- **Description:** Captured from `set_2/video2_3.avi`, depicting typical indoor movement scenarios.
- **Resolution:** 1280 × 720  
- **Codec:** Xvid MPEG-4  
- **FPS:** 30  

### 6. Indoor Video 3 (IV3) – *Atrium*
- **Source:** [UrbanTracker](https://www.jpjodoin.com/urbantracker/dataset.html)
- **Description:** Captures pedestrian movement inside École Polytechnique Montréal’s atrium.
- **Resolution:** 800 × 600  
- **Frames:** 4540  
- **Codec:** Xvid MPEG-4  
- **FPS:** 30  

---

##  Test Scenarios

This repository also includes multiple testing scenarios to evaluate performance under varying frame configurations and compression settings. These folders are named based on the number of frames used in the test:

- `10-10-testing`, `15-15-testing`, `15-20-testing`, `20-15-testing`, `20-20-testing`, `20-30-testing`, `30-20-testing`, `30-30-testing`  
  Represent combinations of different frame count tests (e.g., 10 frames from video1 with 10 frames from video2, and so on).

- `100-100-testing`, `300-300-testing`  
   Larger scale tests with 100 or 300 frames per video.

- `H.265`  
   Contains test outputs or encodings using the H.265 codec.

---

## Frame Directory Structure

- `video1_frames`, `video2_frames`  
   Original frames extracted from the videos.

- `video1_frames_png`, `video2_frames_png`  
   Same frames as above but converted to `.png` format.

- `Combined-frames-png`  
    Frame-by-frame merged outputs of video1 and video2.

- `reconstruct-video1-frames-png`, `reconstruct-video2-frames-png`  
   Reconstructed frames for individual video streams after processing or decompression.

- `raw-videos`  
    Contains the original `.avi` or `.mov` video files used for testing.

---

 All videos in this repository are used solely for research and testing purposes. 