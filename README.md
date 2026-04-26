Abstract
Multi-modal Magnetic Resonance Imaging
(MRI) is crucial for precise brain tumor segmentation. However, missing modalities are prevalent in clinical practice,
severely degrading the performance of deep networks designed for complete multi-modal data. Existing solutions
like synthesis or zero-filling often suffer from feature collapse or hallucinated artifacts, while most fusion strategies lack explicit awareness of the specific missing status. To address these challenges, we propose LFC-SATP,
a unified framework comprising Latent Feature Completion (LFC) and State-Aware Text Prompting (SATP). First,
the LFC strategy dynamically generates substitute vectors
in the latent space to fill missing dimensions, effectively
maintaining feature distribution integrity without the high
computational cost of voxel-level synthesis. Second, the
SATP mechanism automatically encodes modality availability into semantic text prompts. Utilizing a pre-trained text
encoder, it injects prior knowledge to guide the interaction
and calibration of visual features via cross-modal attention,
eliminating the need for manual input. Finally, a SemanticGuided Gating Module (SGG) is introduced to refine shallow
texture representations using deep semantic features for
noise suppression. Extensive experiments on BraTS 2018,
BraTS 2020, and BraTS 2021 datasets demonstrate that
our method achieves state-of-the-art performance under
various missing modality settings.
