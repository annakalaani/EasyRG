# EasyRG
an all-in-one tool for automatic bulk analysis of ffERG waveforms in preclinical studies - ERG made easy!

### Licensing
The EasyRG program is published under a GNU General Public 3.0 License. Please consult "LICENSE" for more information on the licensing of the code.
If you wish to re-use this code under a different licens, please contact IXA: info@IXA.nl

## Quickstart guide
### Set-up
<img width="1111" height="472" alt="Screenshot 2026-07-06 at 10 59 53" src="https://github.com/user-attachments/assets/ae261b92-4a56-4006-a76e-91fdfa949893" />

The program starts with a chunk of modifiable code. This is the only part that has to be modified by the user.

First, fill in the pathnames to:
1) A folder containing all your raw CSV files (or your file with pre-processed data). This folder should not contain other files.
2) A file containing the metadata, formatted according to the metadata_template
3) An output folder to export the excel file to. This folder can contain other files.

Second, fill in the time_label and the grouping_var to specify the set-up of your experiment (e.g. "weeks since treatment" x "treatment", or "days of age" x "genotype". Please note that the grouping_var is case sensitive and must match the label in the metadata.

### Running the code
<img width="1137" height="477" alt="Screenshot 2026-07-06 at 11 06 17" src="https://github.com/user-attachments/assets/c2f6645d-61c2-43ea-aebe-874a25e16b42" />
<img width="1130" height="456" alt="Screenshot 2026-07-06 at 11 06 31" src="https://github.com/user-attachments/assets/207a770a-3420-4af5-8934-cae27b1b90da" />

Run the code by knitting to html (recommended option), word, or pdf. You can also run the code within Rstudio by running all chunks.

### Output
<img width="1170" height="833" alt="Screenshot 2026-07-06 at 11 08 00" src="https://github.com/user-attachments/assets/0a0a270e-12cd-4ea4-aff6-494ab788ad8c" />

When knitting to html, a pop-up will appear containing all the main data. Here you can see the first overview plot of the testing data.

<img width="982" height="615" alt="Screenshot 2026-07-06 at 11 10 15" src="https://github.com/user-attachments/assets/3d4ef423-5887-4d96-8bcc-68a760df6777" />
<img width="982" height="777" alt="Screenshot 2026-07-06 at 11 10 28" src="https://github.com/user-attachments/assets/d9c2edc8-21ab-45e6-8732-926eac34571b" />

The html file will contain the plotted waveforms, as well as plots showing the average a- and b-wave amplitudes and the average flicker amplitude per group and timepoint. Statistics and normality tests are shown for these outcomes, but only the significant results are described in the tables to make it easier to read.

<img width="1467" height="851" alt="Screenshot 2026-07-06 at 11 14 05" src="https://github.com/user-attachments/assets/020b414b-0c3f-44ef-90c7-d57478dd9b46" />

The excel output file that is created, on the other hand, contains all calculated outcomes (for flash waveforms: amplitudes, implicit times, and area under the curve; for flicker waveforms: average amplitude and peak 2 amplitude). It also contains *all* results of the statistical tests, so not only the significant ones.

### For more detailed instructions on how to run the code, please consult the handbook.

PLEASE NOTE!

This program was created in Rstudio as a .rmd file and was optimized for ffERG data from Brown Norway rats, retrieved from a Roland ERG machine (RETImap full flash Ganzfeld).

Modifications may be necessary to run properly on data from other animal models.

It is possible to upload pre-processed data from other ERG machines. We encourage researchers to create and share their own pre-processing modules for different machines.

### Bugs or questions?
Please contact us through the "Issues" page on this repository.
For bugs, mention the error you received and the lines on which you received the error.

