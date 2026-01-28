# Hafner-2026-IL-BMP
Public repo for sharing data associated with IL-BMP-2023-2024 paper

# Link to paper
Excepted soon (by end of January 2026)

# Maintainer
Sasha Hafner.
Contact information here: <https://au.dk/sasha.hafner@bce.au.dk>.

# Contents
The `data` directory contains five files, summarized below.

* `biogas.csv`: Cumulative volume of methane and total biogas over time for each test bottle. Total of around 66,000 rows.
* `BMP_rep.csv`: Reported (submitted) biochemical methane potential (BMP). One mean value per lab x test x substrate. Around 200 rows.
* `BMP_calc.csv`: BMP values by bottle calculated from submitted detailed measurement data. More than 600 rows.
* `inoc_prop.csv`: Inoculum properties.
* `setup.csv`: BMP test setup data, i.e., what and how much went into each bottle, along with volatile solids (VS) concentration of inoculum and substrate. 
* `SMP.csv`: Specific methane production (SMP) curve data by bottle, calculated based on submitted detailed measurement data.
* `SMP_eval.csv`: Screening results of specific methane production (SMP) curves.

# Column names
Several column names are shared among files--the meaning is always the same.

* `bmp_calc`: Biochemical methane potential (BMP) calculated from original measurements (mL methane per g substrate VS added). By bottle. 
* `bmp_rep`: Mean (n = 3) biochemical methane potential (BMP) reported (submitted) by participating laboratories (mL methane per g substrate VS added). 
* `bmp_sd`: Standard deviation in BMP.
* `bottle_id`: Unique bottle key as integer. Can be used for merging data from different files.
* `cvBg`: Cumulative volume of biogas by bottle (mL)
* `cvCH4`: Cumulative volume of methane by bottle (mL)
* `c_vs_inoc`: Concentration of VS in inoculum (g/g)
* `c_vs_sub_f`: Reference (`f` is for "fixed") concentration of VS in substrate (g/g)
* `c_vs_sub_m`: Measured (by submitting laboratory) concentration of VS in substrate (g/g)
* `file_id`: Unique integer key for each submitted data file
* `fv_inoc`: Fraction of total methane produced estimated as coming from inoculum (inoculum contribution) (mL/mL)
* `ISR`: Inoculum-to-substrate ratio on a VS basis
* `lab_id`: Unique key for each laboratory. 
* `mass_inoc`: Fresh mass of inoculum added to bottle.
* `mass_sub`: Fresh mass of substrate added to bottle.
* `n`: Number of replicate bottles.
* `set`: Submission set, used for organizing corrections to submitted data.
* `smp`: Specific methane production (mL methane per g substrate VS added)
* `smp_prob`: Binary result of visual screening of SMP curves. 1 = problem observed.
* `substrate`: Substrate name
* `test`: Test key (1 or 2)
* `time_d`: Time of BMP test measurement in days
* `xCH4`: Volume (or mole) fraction of methane in biogas measured or assumed by participating laboratories

