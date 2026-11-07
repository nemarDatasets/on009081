# EEG during Balinese dance movements and balance tasks in expert dancers and non-dancers

Raw 16-channel EEG from 38 women (23 expert Balinese dancers, 15 non-dancers; age 15 years and older), recorded
during two paradigms in one session: three Balinese dance movements and a Romberg-type standing task. Standing Stork
(single-leg stance) times are included in `participants.tsv`.

- **task-rest**: separate resting recording made before the task session (about 1 min, standing, eyes open; participants closed their eyes only in the final part of the Romberg-type task).
- **task-dance**: one continuous task recording. It contains three Balinese dance movements (ngeed, agem to the
  right, agem to the left; 4 repetitions each, in two blocks separated by a 3-min standing rest), followed by a
  Romberg-type standing protocol (feet together; 30 s eyes open while fixating a black dot on the wall, 15 s relaxed standing with eyes open, 30 s eyes
  closed). In several recordings the EEG stopped before the end of the eyes-closed period (see `beyond_recording_end`).

Recording: KT88-1016 digital EEG system (Contec Medical Systems), 16 dry scalp electrodes (10-20 system without midline sites), each referenced to the ipsilateral earlobe
(A1 for left, A2 for right sites); 100 Hz sampling; effective bandwidth about 0.5-35 Hz (amplifier filtering). The
channels Add_lead1 and Add_lead2 carry no signal. The amplifier intermittently produced flat segments (signal resets,
about 0 uV); they are left in the data and should be masked before analysis. Occipital alpha power did not increase
consistently with eye closure in these recordings; see the data article.

Events (task-dance): movement phases (descent, hold, ascent) annotated manually from video; Romberg periods from the
annotated eye-closure time; and the instruction display timeline. Repetitions in which the movement was not
performed are not listed. Two annotated repetitions lack one phase boundary (start of hold or return to upright), so
the events files contain 437 descent events for 438 annotated repetitions.

Participants: `participants.tsv` gives group, age group, sex, categorised dance experience and practice frequency,
and the Standing Stork times (seconds; one trial per leg and eye condition with the hands at the sides, timed with a
Takei balance tester before the EEG session; 240 s = test ceiling). Exact ages, dates, names and video recordings are not shared.

Timing: EEG and video were started manually on a shared count; event times are given on the EEG clock with an
EEG-video offset of 0 s. Two estimates of the residual offset disagree by about 1 s (onset of movement artefacts:
median about 0 s; cross-correlation of video motion with the EEG muscle-artefact envelope: about +0.9 s, unreliable in
part of the sample). Users analysing short phases such as the hold may repeat their analyses with an alternative
offset.

Ethics: Research Ethics Committee of the Faculty of Medicine, Universitas Udayana/Sanglah General Hospital (Komisi Etik Penelitian FK Unud/RSUP Sanglah), No. 3259/UN14.2.2.VII.14/LT/2026, 31 August 2026. All participants gave written informed consent, including consent to share de-identified data; for
participants younger than 18 years a parent gave written consent and the participant gave assent.

Code for the conversion and analyses: https://doi.org/10.5281/zenodo.24026706

Contact: I Putu Adiartha Griadhi, Department of Physiology, Faculty of Medicine, Universitas Udayana, Denpasar, Bali,
Indonesia (adiartha.griadhi@unud.ac.id).
