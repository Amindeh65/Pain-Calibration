# Adaptive Pain and Tolerance Measurement

This method improves the accuracy of pain and tolerance measurement by adjusting the temperature based on participants' reported sensations. It enables the determination of individual pain and tolerance levels.

---

## Description of the Experiment

### Overview
Four runs (6 trials in each run, totaling 24 trials) of noxious heat were administered to six forearm sites using iterative adaptive logistic regression. Each stimulus lasted 13 seconds, with 1.5 seconds allocated for ramping. Sensation was rated on a circular scale ranging from "no sensation" to "strongest imaginable."

### Participant Reporting
Participants reported pain and tolerance using binary responses ("yes" or "no") to the following questions:
- **"Painful?"**
- **"Tolerate?"**

---

## Experiment Steps

### Step 1: Calibration Phase
1. The first run familiarized participants with a fixed temperature of **47°C** across all sites.
2. The second run included stimuli at **45°C**, **47°C**, and **48.9°C**, applied twice in a randomized order.

### Step 2: Adaptive Testing
1. **Runs 3 and 4**:
   - Included low and high temperatures based on the pain and tolerance responses from previous trials.
2. **Logistic Regression**:
   - A regression model was used to determine the low (pain) and high (tolerance) thresholds, updated after each trial.
   - The final trial identified the thresholds for pain and tolerance.

### Step 3: Selection for Stimulation
Two forearm sites with the least mean absolute error values in rate-temperature linear regression were selected for pain stimulation.

---

## Methodology Diagram
Here is an example diagram that visualizes the process:

![image](https://github.com/user-attachments/assets/1315c273-2167-4b79-9aa3-3e6673ac8487)

