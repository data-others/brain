![image](https://github.com/frankyeh/Brain-Data/assets/275569/06d71820-389b-4618-a48d-58b9e7e44bf4)

The Healthy Brain Network (HBN) is an ongoing initiative focused on building a biobank of data from 10,000 children and adolescents (ages 5-21) in the New York City area. This initiative adopts a community-referred recruitment model, where study advertisements target families concerned about one or more psychiatric symptoms in their child. The Healthy Brain Network Biobank contains a rich array of data, including psychiatric, behavioral, cognitive, and lifestyle (e.g., fitness, diet) information, as well as multimodal brain imaging, electroencephalography, digital voice and video recordings, genetics, and actigraphy. Beyond its primary aim of advancing transdiagnostic research, the Healthy Brain Network Biobank also holds promise for furthering biophysical modeling, voice and speech analysis, natural viewing fMRI and EEG, and methods optimization.

# License

HBN requests that any usage of HBN Biobank data is recognized through appropriate citation of the Data Descriptor, which is available on Nature Scientific Data:

Reference: [Alexander, Lindsay M., et al. "An open resource for transdiagnostic research in pediatric mental health and learning disorders." Scientific data 4.1 (2017): 1-26.](https://www.nature.com/articles/sdata2017181)

- [official website](https://fcon_1000.projects.nitrc.org/indi/cmi_healthy_brain_network/Publications.html)

# Participants and Experiments

Phase I: Implementation and testing (Participants 1–500; completed)
Established a prototype HBN Diagnostic Research Center in Staten Island, New York, and tested workflows for recruitment, evaluations, and assessments.

Phase II: Revision and hardening (Participants 501–1000; completed)
Balanced stable protocols with integrating new measures and optimizing protocols based on experiences and advances.

Phase III: Scale-up (Participants 1001–8500; in process)
Aims to enroll 7,500 participants, expanding capacity with more centers and MRI sites in NYC for a diverse sample.

Phase IV: Targeted recruitment (Participants 8501–10000)
Will use epidemiologic sampling to recruit an additional representative sample of 1,500 participants

# Download

| File Format | Modality/Content | Link | Details |
|-------------|---|---|---------|
| SRC | TOPUP-Eddy corrected DWI | [OneDrive](https://pitt-my.sharepoint.com/:f:/g/personal/yehfc_pitt_edu/EuQx-2egztZJpA0iIpzrTwgB_YR3HofgTpfhhH-thoQzCw?e=E8hGXP) | The SRC files contain raw dMRI signals for modeling. They can be reconstructed in DSI Studio to generate FIB files. The original NIFTI files can be downloaded from the HCP's connectome db website. |
| FIB | Fiber orientation maps in the native space| [OneDrive](https://pitt-my.sharepoint.com/:f:/g/personal/yehfc_pitt_edu/EhYy5-HBMx9OgA7uY_uQ6akBwx_3M4FInRd1VLUyxAlXAw?e=XFwDfE) | GQI reconstructed FIB file in the native space. The FIB files are track-ready files for DSI Studio to run fiber tracking. |
| NIFTI | T1W/T2W | [OneDrive](https://pitt-my.sharepoint.com/:f:/g/personal/yehfc_pitt_edu/EiM5CMupP4xKjoeeezAMTOIBO-u0-j7TOnX2_u47aJRJiQ?e=5aNM3f) |  |
| Text file | demographics | [OneDrive](https://pitt-my.sharepoint.com/:f:/g/personal/yehfc_pitt_edu/EqfsINe8hoJBhOGfuYeg56ABx1Lf3Grir8jMYWdt3ZEqnw?e=vkz2dK) | |

Download OneDrive data using [OneDrive Linux GUI](https://github.com/bpozdena/OneDriveGUI)

# Methods
> A multishell diffusion scheme was used, and the b-values were 1000 and 2000 s/mm². The number of diffusion sampling directions were 64 and 64, respectively. The in-plane resolution was 1.8 mm. The slice thickness was 1.8 mm. The susceptibility artifact was estimated using reversed phase-encoding b0 by TOPUP from the Tiny FSL package (http://github.com/frankyeh/TinyFSL), a re-compiled version of FSL TOPUP (FMRIB, Oxford) with multi-thread support. FSL eddy was used to correct for eddy current distortion. The correction was conducted through the integrated interface in DSI Studio ("Chen" release)(http://dsi-studio.labsolver.org). The diffusion MRI data were rotated to align with the AC-PC line at an isotropic resolution of 1.8. The restricted diffusion was quantified using restricted diffusion imaging (Yeh et al., MRM, 77:603–612 (2017)). The diffusion data were reconstructed using generalized q-sampling imaging (Yeh et al., IEEE TMI, ;29(9):1626-35, 2010) with a diffusion sampling length ratio of 1.25. The tensor metrics were calculated using DWI with b-values of 1000 s/mm².
## Release Link
https://github.com/data-others/brain/releases/tag/hbn
