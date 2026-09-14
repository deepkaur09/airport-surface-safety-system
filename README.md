## Roadmap

### Phase 1: Planning
- [ ] Define scope and use cases (runway crossing, taxiway conflict, restricted zone entry, FOD path)

### Phase 2: Data
- [ ] Collect/prepare data (AVOSS, FAA surface data, simulated/self-recorded footage)
- [ ] Label data (LabelImg, CVAT, or Roboflow)

### Phase 3: Detection & Tracking
- [ ] Build/train object detection model (YOLOv8)
- [ ] Add multi-object tracking (DeepSORT / ByteTrack)

### Phase 4: Spatial Mapping
- [ ] Create airport map (runways, taxiways, hold-short lines, restricted zones)
- [ ] Calibrate camera-to-map coordinates (homography)

### Phase 5: Prediction & Risk Logic
- [ ] Compute motion features (position, velocity, heading, acceleration)
- [ ] Build trajectory prediction module (Kalman filter / LSTM)
- [ ] Build conflict detection logic (path intersection, time-to-conflict)
- [ ] Add rule-based safety layer (risk type + severity)

### Phase 6: Alerts & UI
- [ ] Design alert system (object, location, time-to-conflict, severity, action)
- [ ] Build dashboard/UI (OpenCV / Streamlit / Flask)

### Phase 7: Testing & Evaluation
- [ ] Test on simulated scenarios
- [ ] Evaluate performance (false alarm rate, accuracy, warning lead time)
- [ ] Refine and tune

### Phase 8: Wrap-up
- [ ] Document system (methodology, architecture, results, limitations)
- [ ] Prepare final demo
