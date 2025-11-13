
# Introduction

<img src="https://github.com/frankyeh/Brain-Data/assets/275569/b6783feb-2849-4d50-ad32-a983dd44065e" width=600/>

The SLIM (Structural, Longitudinal, and Integrated Multimodal) dataset is a valuable resource in neuroimaging, acquired through multimodal magnetic resonance imaging (mMRI). With a three-and-a-half-year longitudinal design, it addresses gaps in test-retest reliability and age-span limitations. Featuring diverse mMRI scans and behavioral assessments, SLIM provides a comprehensive view of the human brain. This dataset, acquired meticulously, is available for researchers globally, fostering collaboration and contributing to reproducible human brain sciences in partnership with CoRR. Explore the SLIM dataset for insights into the complexities of the human brain.

# License

License: Creative Commons License: Attribution - Non-Commercial

Reference: Liu W, Wei D, Chen Q, Yang W, Meng J, Wu G, Bi T, Zhang Q, Zuo XN, Qiu J. Longitudinal test-retest neuroimaging data from healthy young adults in southwest China. Scientific data. 2017 Feb 14;4(1):1-9. [link](https://www.nature.com/articles/sdata201717)

Official website: [link](https://fcon_1000.projects.nitrc.org/indi/retro/southwestuni_qiu_index.html)

# Download

| File Format | Modality/Content | Link | Details |
|-------------|---|---|---------|
| SRC | Eddy corrected DWI | [OneDrive](https://pitt-my.sharepoint.com/:f:/g/personal/yehfc_pitt_edu/EtWIdIDfcMhEu-3xFgEonroBEv4pd1pvF58jGCl_gUICvQ?e=4NGoEL) | The SRC files contain raw dMRI signals for modeling. They can be reconstructed in DSI Studio to generate FIB files. The original NIFTI files can be downloaded from the HCP's connectome db website. |
| FIB | Fiber orientation maps in the native space| [OneDrive](https://pitt-my.sharepoint.com/:f:/g/personal/yehfc_pitt_edu/EqCb30iFWu1NrxUuIA9B4BcBGV41jG1c8a17r8XV3Vckfg?e=ww9FlP) | GQI reconstructed FIB file in the native space. The FIB files are track-ready files for DSI Studio to run fiber tracking. |
| NIFTI | T1W | [OneDrive](https://pitt-my.sharepoint.com/:f:/g/personal/yehfc_pitt_edu/EnrYX8ziMQxNkiKdqFSzdUABDQ-14cjNIuHY_gL5ABoVVQ?e=2RDqCd) |  |
| Text file | demographics | [OneDrive](https://pitt-my.sharepoint.com/:f:/g/personal/yehfc_pitt_edu/ElrX6-IfV8ZEnBPD__vUM6sBpRECHjyZ7fBRhAs9q3o3yQ?e=QFAhyl) | |

# Methods
>  A DTI diffusion scheme was used, and a total of 90 diffusion sampling directions were acquired. The b-value was 1000 s/mm². The in-plane resolution was 2 mm. The slice thickness was 2 mm. FSL eddy was used to correct for eddy current distortion. The correction was conducted through the integrated interface in DSI Studio ("Chen" release)(http://dsi-studio.labsolver.org). The diffusion MRI data were rotated to align with the AC-PC line at an isotropic resolution of 2.000000. The restricted diffusion was quantified using restricted diffusion imaging (Yeh et al., MRM, 77:603–612 (2017)). The diffusion data were reconstructed using generalized q-sampling imaging (Yeh et al., IEEE TMI, ;29(9):1626-35, 2010) with a diffusion sampling length ratio of 1.25. The tensor metrics were calculated using DWI with b-value lower than 1750 s/mm². 
## Release Link
https://github.com/data-others/brain/releases/tag/swu-slim
