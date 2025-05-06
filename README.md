# DetReIDX
# DetReIDX: A Stress-Test Dataset for Real-World UAV-Based Person Recognition

**DetReIDX** is a challenging dataset for evaluating pedestrian detection and person re-identification (ReID) across real-world aerial and ground conditions. Captured via drones and ground cameras, it simulates complex scenarios involving long-range tracking, variable pitch angles, occlusions, and domain shifts.

## 📌 Highlights

- **Real-World UAV Data**: Captured from drones at heights up to 40 meters, with varying pitch angles and distances.
- **Multiple Scenarios**:
  - **Aerial to Aerial**: Cross-session generalization from drone data.
  - **Aerial to Ground / Ground to Aerial**: Cross-view matching under domain shift.
  - **Long-Term and Long-Range Matching**: Identity persistence under severe visual degradation.
- **Annotations**:
  - Bounding boxes for pedestrian detection.
  - Identity labels for ReID.
  - File names encode camera height, pitch, and distance for contextual analysis.
- **Dataset Splits**:
  - Training, Query, and Gallery folders with structured tracklets.
  - Protocols for short-term and long-term evaluation.

## 📂 Folder Structure

