---
title: Response to Reviewers
geometry: margin=1in
---

Reviewer's original suggestions are in quote blocks and in **bold**  
Our response follows in normal font, and changes to the document are in quote blocks and normal font.  

# Editor Comments to Author

## Section Editor: 1

> **Comments to the Author:**  
> **This manuscript by Weber et al. is focused on oxygenation quantification in the SSS and CCV in 19 premature infants utilizing susceptibility mapping and paramagnetic separation, which is compared directly and thoroughly with the preceding literature using a variety of techniques. This is significant in that it may provide an additional, and hopefully more accurate, way to measure oxygenation in premature infants. Overall this is an impressive and well planned study.**

Thank you for your kind words and for taking the time to review our manuscript.

---

> **The main issue which needs to be addressed revolves around the conclusions, and that the presented data do not support that this has superior accuracy. It is important because some of the findings contradict previous studies. The language here needs to be softened**

We agree. It is important that our conclusions do not overstate the evidence provided. Based on the editor's recommendation, we have now softened our language in the abstract, impact statement, and conclusion:

Abstract:

> While paramagnetic component decomposition yielded SSS values closer to those found in the literature, it increased variability. No significant oxygenation differences were found between the SSS and CCV, contrasting with prior studies.

Impact Statement:

> This study evaluated the use of QSM and its paramagnetic components to measure cerebral oxygenation in neonates.

Conclusion:

> This study aimed to evaluate how the use of susceptibility separation on preterm neonatal QSM images could be used in determining the oxygenation of cerebral venous vessels

---

> **In the methods, there are 3 lines where "\*\*\*" appears, I am not sure what that is supposed to represent (lines 102, 104, 117).**

These asterisks' were included in order to abide by what we believed *Pediatric Research's* submission guidelines were, to anonymize the paper from reviewers. These will be replaced with the identifying information once accepted. Or, if we made a mistake, we are happy to de-anonymize them for the reviewers.

---

> **Requires additional clarification related to imaging analysis and how it leads to their conclusion**

We agree with the editor and with the reviewers below who made similar comments. Please see our responses below for a detailed summary of the changes we made.

# Reviewer(s)' Comments to Author

## Reviewer: 1

> **Comments to the Author**  
> **Summary:**  
> **This study aims to quantify oxygenation in the superior sagittal sinus and in central cerebral veins in a cohort of 19 preterm neonates using quantitative susceptibility mapping and the separation of its paramagnetic components.**  
> **The authors observed no significant differences between the oxygenation of the SSS and CCV, which contradicts previous results reported in the literature. They reported that the accuracy of the paramagnetic source separation was higher than QSM, but at the cost of an increased variability.**  
> **The methods of the manuscript are well detailed, and the results are appropriately compared to the literature. A few aspects require some clarification, see below.**

We thank the reviewer for taking the time to read our manuscript and for making suggestions to help improve the final result.

---

> **One limitation of this work is the lack of sufficient data to support the claim of increased accuracy with susceptibility sources separation compared to QSM. In the absence of a ground truth and with results that contradict literature, this work does not support the increased accuracy claimed. The conclusion of the work should be re-written to better reflect the actual results.**

We agree with the reviewer. Without a ground truth to compare to, it is difficult to say if our results reflect a more accurate measure. We have now included wording saying as much, and rewritten the conclusion as follows:

> This study aimed to evaluate how the use of susceptibility separation on preterm neonatal QSM images could be used in determining the oxygenation of cerebral venous vessels

The impact statement was also changed:

> This study evaluated the use of QSM and its paramagnetic components to measure cerebral oxygenation in neonates.

Along with the abstract:

> While paramagnetic component decomposition yielded SSS values closer to those found in the literature, it increased variability. No significant oxygenation differences were found between the SSS and CCV, contrasting with prior studies.

---

> **Specific Issues:**  
> **Abstract:**  
> **1. Please re-write the first sentence of the conclusion section of the abstract to better reflect the results presented in this work, which do not fully support the current claim of increased accuracy with susceptibility source separation.**

The first sentence of the conclusion of the abstract has been changed to better reflect our findings:

> While paramagnetic component decomposition yielded SSS values closer to those found in the literature, it increased variability. No significant oxygenation differences were found between the SSS and CCV, contrasting with prior studies.

---

> **Introduction:**  
> **2. It is mentioned that methods to assess whole brain oxygenation have been developed for adults and that they are starting to be explored in neonates. Please detail what are the challenges for transferring these methods to neonate population.**

We have adjusted this section to now read:

> For the preceding reasons, non-invasive MRI-based techniques are actively being explored to assess regional and whole-brain blood oxygenation. While MRI-based methods have been developed for adults (9-11), their application in neonates is only beginning to be explored (12-16). This delay is likely due to the unique challenges posed by neonates, including their smaller anatomies, distinct hemodynamic profiles, susceptibility to motion artifacts, and the difficulties associated with recruiting this population for research.

---

> **Method:**  
> **Image acquisition**  
>**3. Please state in the text the plane of acquisition for each sequence.**

We now include the plane of acquisition for each sequence in the text of the Image Acquisition section.

---

>**4. Table 1: The phase encoding row (2nd row) does not provide the phase encoding information. This row should be split in two, one for the acquisition plane information (axial, coronal, sagittal), and one for the actual phase encoding direction in plane (ex: right-left, antero-posterior, or head-foot).**

We thank the reviewer for catching this. We have now updated the table to reflect these changes by adding a row for Acquisition plane, and fixing the Phase-encoding direction

---

> **Image analysis:**  
> **5. Briefly explain why the fifth echo was selected to generate the preliminary brain mask.**

The last (fifth) echo was used to create the brain mask as the last echo will have the greatest signal decay from air-bone-tissue interfaces. This is important to use in order to properly avoid introducing aliasing in the inverse problem. We now include an explanation of this in our methods for readers:

> The last echo is used to generate the brain mask as it reliably removes artifacts from air-tissue and bone-tissue interfaces, e.g., sinuses, without the need for manual erosion. The reason for this is at longer echo times, tissues with rapid signal decay (such as bone, air, and sinuses) lose their MRI signal due to dephasing caused by greater magnetic field inhomogeneities.

---

> **6. Please clarify if all echoes were used for the preliminary QSM calculation.**

We apologise for the confusing way our methods section was written. The methods now describe that the fifth echo was used for mask creation; the STI suite used all five echoes to create five separate QSM images; the 3rd, 4th and 5th QSM maps were then averaged to create the final QSM image for which chi values are taken. The $\chi$-separation toolbox outputs a single map for diamagnetic, paramagnetic, and QSM. Please see the tracked changes in the methods section, and our response to #8 below.

---

> **7. Can the authors expand on the motivation for choosing the STI software? What does ‘cleanest images’ refer to exactly (accuracy, artifact free, etc.)? Please also add a reference to support this statement.**

The STI software appeared to give the best images, based on a visual check by the authors. As this was based on our opinion, we cannot provide a reference for this.  
We now include an explanation of this in the methods:

> STI Suite (v. 3.0), was used to process the final QSM images as it produced the images with the least amount of artifacts (based on a visual assessment by the authors) without eroding the SSS.

---

> **8. Can the authors explain why only the last three echoes were used for the STI QSM calculation?**

This was an error in reporting we have now fixed. Please see the response below.

---

> **9. The methods description mentions that the last three echoes only were used for the STI calculation, but then in the parameters listed in the text, it is mentioned that a TE1=5 ms was used, which is the first TE of the sequence. Can the authors clarify this?**

We apologise for this. The way it was written was not clear. We used all five echoes to produce a five echo QSM image, but then averaged the last three echoes to produce the final QSM image. The section now reads:

> The finalized brain mask along with the magnitude and phase images were used in STI Suite along with the following parameters: 0.9766 x 0.9766 x 1 mm3 voxel size, 5 ms TE1, 5.24 ms TE, and 77.4 ms sum TE, B0 strength = 3, and B0 direction = [0, 0, 1]. The 3D GRE data option was selected for the phase processing stage, and STAR-QSM was selected for the QSM stage. The last three echoes of the QSM were then averaged to create the final QSM image using fslmaths, as the accumulation of phase due to susceptibility is small in early echoes and artifacts dominate the phase.

---

> **10. In the paragraph describing the methods for the paramagnetic source separation, please list the TEs in ms unit instead of s for consistency with the rest of the manuscript. Also in the same paragraph, please use the acronym introduce earlier in the text for delta TE for consistency.**

We thank the reviewer for catching these. We originally stated the TEs in seconds in this section as that is what the paramagnetic source software uses when entering units. However, we believe that using consistent units throughout the manuscript would be best. We have made this correction in this section.

---

> **11. Can the authors include an illustration of the final SSS and CCV masks used to calculate mean susceptibility in these regions?**

Yes of course. We agree that this would be a good addition to the paper.

Please see the new figure now numbered Figure 2.

---

> **Results:**  
> **12. Figure 2: Please add a label to the colorbars (ex: chi (ppm)). Also, please clarify in the caption what the x/y/z label on each figure refers to.**

"$\chi$ (ppm)" has now been added to the two colorbars. In addition, we now include the following in the caption:

> The color bars in (b) and \(c\) indicates the range of susceptibility $\chi$ values in parts per million.

The caption also now includes a sentence at the end that reads:

> y, x and z values represent the slice number in each plane (coronal, sagittal, and axial, respectively).

---

> **13. Figure 3: In the text referring to fig 3, the graphs presented are referred to as boxplots, versus in the figure caption, they are referred to as violin plots. Please make sure to consistently use the same term.**

We apologise for missing this. The text has been changed to reflect the appropriate plot name: 'violin plots'.

> Violin plots of the comparisons are shown in Figure 3.

---

> **Discussion**  
> **14. The authors mention being the first to explore the susceptibility source separation technique in neonates, while it has been done in adult population. Please discuss the challenges of transferring this technique to a neonate population and how these were address in this work.**

Often times new techniques will first be used in adults before eventually being used in neonatal populations. Part of this is due to the relative difficulty in acquiring ethics and recruiting subjects for neonatal research. My lab has a focus on neonatal brain development and I happen to be interested in QSM. We believe we are the first to perform this type of analysis in a neonatal population simply due to a combination of luck, access to data, and timing. However, please see our response to #2 above where we now include some of the challenges in scanning neonates in the introduction.

---

> **15. Can the authors discuss why, based on their results, QSM underestimates the susceptibility compared to the paramagnetic component separation technique?**

Reading over the manuscript, we realise this is a very important concept that should have been included in the introduction. We now include the following sentence near the end of the introduction:

> Furthermore, QSM tends to underestimates parametric components due to the inclusion of diamagnetic tissue, and vice versa, as the opposing magnetic susceptibilities effectively subtract from one another.
