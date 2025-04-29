# Data and R code from: Fin whale song evolution in the North Atlantic&#x20;

---

These different datasets are in a CSV format to be used in the R script provided. Some datasets were used to create  figures in the associated paper, which numbers are in brackets.

## Description of the Data and file structure

Datasets contain measurements of three different fin whale parameters (internote interval and peak frequencies of the 20-Hz and higher frequency notes sorted by song (or day, since only one song was analysed per day). Measurements were made by the acoustic software Raven Pro 1.5 and then transferred to a database. The following datasets are included:

Perc_SE_songs: contains the percentages of each INI type from 1999 to 2005 at the southeast (SE) location of the Oceanic Northeast Atlantic (ONA) region (Figure 1B in paper). Column headers are the following: 

*   "Year"- referring to singing season (October through March) thus covering two years at a time
*   "perc"-percentage (%) of each song INI type in each year
*   "INI"- the type of INI

INI_ave_SE_99_05: contains all INIs averaged by song collected from 1999 to 2005 at the SE location of the ONA region (Figure 1C in paper). Column headers are the following:

*   "date"-  day of the analysed song
*   "Ave_INI"-averaged INIs by song and day
*   "SD_INI"- standard deviation for INIs by song and day
*   "Ave_PF"- averaged peak frequencies of  20-Hz notes by song and day
*   "SD_PF"-standard deviation of peak frequencies of 20-Hz notes by song and day
*   "Num_INI"-number of INIs measured.

Perc_ONA_songs: contains the percentages of each  INI during the 2002/2003 singing season at 6 locations of the ONA region (Figure 2 in paper). Column headers are the following: 

*   "perc": percentage (%) of each song INI type by location
*   "INI"- the type of INI
*   "Location" - location within the ONA region denoted by CE (central east), CW (central west), NE (north east), NW (north west), SE (south east) and SW (south west).

INI_ave_06_20: contains all INIs averaged by song collected from 2006 to 2020 and sorted by location, region and year (Figure 3A in paper). Column headers are the following: 

*   "Region"- regions as described in "Sampling locations" from the paper's methods section
*   "Location" - locations as described in "Sampling locations" from the paper's methods section
*   "date" - day of the analysed song
*   "Ave_INI"-averaged INIs by song and day
*   "SD_INI"- standard deviation for INIs by song and day
*   "Ave_PF"- averaged peak frequencies of  20-Hz notes by song and day
*   "SD_PF"-standard deviation of peak frequencies of 20-Hz notes by song and day
*   "Num_INI"-number of INIs measured
*   "Recorder"- Typer of recorder denoted by AR (Autonomous recorder) and OBS (Ocean bottom seismometer)
*    "year"- year of the analysed song.

20Hz_ave_EARs: contains INIs and peak frequencies of the 20-Hz note averaged by song (or day) and its standard deviations sorted by location, region and year recorded only with Ecologic Acoustic Recorders (EARs)  (Figure 3B in paper). Column headers are the following:

*   "Region"- regions as described in "Sampling locations" from the paper's methods section
*   "Location" - locations as described in "Sampling locations" from the paper's methods section
*   "date" - day of the analysed song
*   "year"- year of the analysed song
*   "Ave_INI"-averaged INIs by song and day
*   "SD_INI"- standard deviation for INIs by song and day
*   "Ave_PF"- averaged peak frequencies of  20-Hz notes by song and day
*   "SD_PF"-standard deviation of peak frequencies of 20-Hz notes by song and day
*   "Num_INI"-number of INIs measured.

HF_ave: contains peak frequencies of the high frequency (HF) note averaged by song (or day) and its standard deviations sorted location, region and year (Figure 3C in paper). Column headers are the following: 

*   "Region"- regions as described in "Sampling locations" from the paper's methods section
*   "Location" - locations as described in "Sampling locations" from the paper's methods section
*   "date" - day of the analysed song
*   "year"- year of the analysed song
*   "Ave_PF"- averaged peak frequencies of  HF notes by song and day
*   "SD_PF"-standard deviation of peak frequencies of HF notes by song and day
*   "Num_note"-number of notes measured.

INI_all: contains all INIs measured from 1999 to 2020 and sorted by location, region and year (Figure 4A). Column headers are the following:

*   "Region"- regions as described in "Sampling locations" from the paper's methods section
*   "Location" - locations as described in "Sampling locations" from the paper's methods section
*   "date" - day of the measured INI
*   "month" - month of the measured INI
*   "year"- year of the measured INI
*   "year2" -singing season
*   "time" - time of the first measured INI of each song
*   "INI" - measured INI
*   "PF_20Hz" - peak frequency of the 20-Hz note.

HF_all: contains all measurements of the higher frequency (HF) note peak frequencies sorted by location, region and year (Figure 4B). Column headers are the following:

*   "Region"- regions as described in "Sampling locations" from the paper's methods section
*   "Location" - locations as described in "Sampling locations" from the paper's methods section
*   "date" - day of the measured HF peak frequency
*   "month" - month of the measured HF note peak frequency
*   "year"- year of the measured HF note peak frequency
*   "year2" -singing season
*   "Peak-Freq" - peak frequency of the HF note.

test_ear_obs: contains measurements of INIs and peak frequencies of the 20-Hz note from the same song recorded by an EAR and and OBS to perform a Wilcox test pariwise comparisons. Column headers are the following: 

*   "INI_ear" - INIs measured from EAR recordings
*   "Peak_freq_ear" - peak frequencies of the 20-Hz note measured from EAR recordings
*   "INI_obs" - NIs measured from OBS recordings
*   "Peak_freq_obs" - peak frequencies of the 20-Hz note measured from OBS recordings

PF_ave_all: contains all 20-Hz note peak frequency measurements averaged per song (or day) and its standard deviations sorted location, region and year (*Figure 3 – figure supplement 2). Column headers are the following: 

*   "Region"- regions as described in "Sampling locations" from the paper's methods section
*   "Location" - locations as described in "Sampling locations" from the paper's methods section
*   "date" - day of the measured 20-Hz note peak frequency
*   "Ave_PF"- averaged peak frequencies of  20-Hz notes by song and day
*   "SD_PF"-standard deviation of peak frequencies of 20-Hz notes by song and day
*   "Num_note"-number of notes measured
*   "Recorder" - type of recorder (AR or OBS).

## Sharing/access Information

No other links exists for this data

Was data derived from another source?
No

#### **R Code**

The R code is organised following the same order as figures and tests in the associated paper with a reference to them as comments.
