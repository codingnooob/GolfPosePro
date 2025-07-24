# GolfPosePro
GolfPosePro: Visual Golf Swing Analyzer with Pose and Phase Tracking


📝 Description:
Frame-by-frame golf swing analyzer that uses MediaPipe Pose to detect wrist motion, segment swing phases (Address → Impact → Follow-through), and generate synchronized debug visualizations with slow-motion playback. Ideal for coaching, comparison with pro players, and biomechanical feedback.


[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1-7KzGqmnw8213tHScEUuUiPEZWajxHzj#scrollTo=URjt8VkkIrJd)

GolfPosePro is an end-to-end pipeline for analyzing golf swings using pose estimation and wrist trajectory tracking. It segments swing phases, overlays visual diagnostics, compares student vs. pro frames, and generates slow-motion debug videos — all within a Colab Pro notebook.

---

## 🔍 What This Project Does

- 🎯 Detects golf swing phases from wrist motion (Address → Top → Impact → Follow-through)
- 📈 Plots wrist Y-trajectory with phase-colored overlays
- 📸 Compares student and pro swings frame-by-frame (with optional pose landmarks)
- 🐢 Adds slow-motion replay of the swing segment
- 🎬 Generates side-by-side annotated debug videos

---


---

## 🛠️ Dependencies

All dependencies are installed in Colab. Key libraries:

| Feature             | Library        | Why Use It?                              |
|---------------------|----------------|-------------------------------------------|
| Pose Estimation     | `mediapipe`     | Detect wrist landmarks frame-by-frame     |
| Video Editing       | `moviepy`, `cv2`, `ffmpeg` | Frame extraction, audio fix, slow-mo    |
| Visualization       | `matplotlib`    | Overlay swing phase plots                 |
| YouTube Downloading | `yt-dlp`        | Grab Pro swing clips from YouTube Shorts  |
| Data Smoothing      | `scipy.ndimage` | Clean wrist movement trajectory           |

---

## 🚀 How to Use

1. 🔁 Upload your swing clips (`IMG_*.MP4`)
2. 📥 Download Pro references (e.g., Max Homa, Ludvig Åberg) using `yt-dlp`
3. 🧠 Run wrist detection and swing segmentation
4. 🆚 Visually compare each swing phase (student vs pro)
5. 🎥 Generate annotated slow-motion debug video

---

## 📌 Example Swing Phases Detected

- **Address**: Wrist stability before motion begins  
- **Backswing**: Wrists rise and body coils  
- **Top**: Peak of backswing  
- **Downswing**: Motion toward ball  
- **Impact**: Contact with ball  
- **Follow-through**: Post-impact release


## 📘 Credits

- Built with ❤️ using [MediaPipe](https://developers.google.com/mediapipe), [OpenCV](https://opencv.org/), and [Matplotlib](https://matplotlib.org/)
- Pro swing clips courtesy of [YouTube Shorts](https://www.youtube.com/shorts)


## 📄 License

MIT License. See `LICENSE` for details.



