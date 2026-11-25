# app- covariance

<!-- brainlife-app:begin (generated from the App manifest; edit the manifest, not this block) -->

> **Computes a noise covariance matrix from the first 60 seconds of a raw MEG FIF recording with MNE-Python compute_raw_covariance and saves it with an HTML report.**

Reads the raw FIF file, crops it to 60 s, computes the covariance with mne.compute_raw_covariance and writes cov.fif and an MNE report. Use it for a noise covariance for source estimation, ideally on empty-room or baseline data. The registered branch master does not exist on GitHub; this description is based on the main branch.

| | |
|---|---|
| 📥 **Inputs** | `neuro/meg/fif` |
| 📤 **Outputs** | `neuro/meeg/mne/covariance` · `report/html` |
| 🐳 **Container** | `brainlife/mne:1.0.2` |
| ⚙️ **Resources** | 8 CPUs |
| 🔗 **Run it** | [doi.org/10.25663/brainlife.app.625](https://doi.org/10.25663/brainlife.app.625) |

#### 📥 Inputs

| Input | Datatype | Required | Description |
|---|---|---|---|
| `fif` | `neuro/meg/fif` | yes | Raw MEG recording (FIF). |

#### 📤 Outputs

| Output | Datatype | Description |
|---|---|---|
| `out_dir` | `neuro/meeg/mne/covariance` | Noise covariance matrix (cov.fif). |
| `out_dir_report` | `report/html` | HTML report showing the covariance. |

<!-- brainlife-app:end -->

