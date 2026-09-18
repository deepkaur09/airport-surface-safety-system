## Roadmap

### Phase 1: Planning
- [x] Define scope and use cases (runway crossing, taxiway conflict, restricted zone entry, FOD path)

### Phase 2: Data
- [x] Collect/prepare data (real tarmac footage + simulated coordinates)
- [ ] Label data (LabelImg, CVAT, or Roboflow) — not needed yet, using pretrained YOLOv8 classes

### Phase 3: Detection & Tracking
- [x] Build/train object detection model (YOLOv8, pretrained)
- [x] Add multi-object tracking (YOLOv8 built-in tracker)

### Phase 4: Spatial Mapping
- [x] Create airport map (runways, taxiways, hold-short lines, restricted zones)
- [ ] Calibrate camera-to-map coordinates (homography) — attempted, not reliably aligned with real video; see Known Limitations

### Phase 5: Prediction & Risk Logic
- [ ] Compute motion features (position, velocity, heading, acceleration)
- [ ] Build trajectory prediction module (Kalman filter / LSTM)
- [x] Build conflict detection logic (zone entry + hold-short proximity, tested on simulated paths)
- [x] Add rule-based safety layer (risk type + severity)

### Phase 6: Alerts & UI
- [x] Design alert system (object, location, alert type, severity → CSV)
- [ ] Build dashboard/UI (OpenCV / Streamlit / Flask)

### Phase 7: Testing & Evaluation
- [x] Test on simulated scenarios (restricted zone entry, hold-short crossing)
- [ ] Evaluate performance (false alarm rate, accuracy, warning lead time)
- [ ] Refine and tune

### Phase 8: Wrap-up
- [ ] Document system (methodology, architecture, results, limitations)
- [ ] Prepare final demo
