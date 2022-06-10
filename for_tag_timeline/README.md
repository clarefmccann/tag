## README FOR THE TAG TIMELINE SCRIPT

# this script can be used to auto create a new tag timeline
# should be run once every 6 or so months to factor in actual dates for current waves

# DATE MOST RECENTLY RUN: 06/10/2022

* TO RUN:
  - Export the current waves "W# Session Dates" to /Volumes/psych-cog/dsnlab/TAG/behavior/Demographics/Age/timeline
  - Update the projected doc in the path above from the TAG Expected Scheduling Doc (you can just copy and paste all of the ID's and session dates, including the skipped folks - the script will organize into actual dates vs projected vs skipped)
    - name the columns - "subject_spit_id", "sa_date" and then create a "sb_date" column by using the EDATE(CELL, 1) function
    - change the format to be the YYYY-MM-DD date format in excel and save as CSV
    - change TAG_238 to tag_238 (that's the ID in redcap)
  - Update the skipped doc with IDs that have opted to "skip" the current wave but have not withdrawn
  - Update the withdrawals doc with IDs that have recently withdrawn

  * WHEN DONE:
    - Update the "TAG_age_session_dates.csv" in /Volume/psych-cog/dsnlab/TAG/behavior/Demographics/Age with the whole.csv
    - Update the TAG expected scheduling doc (carefully! don't lose the color coding)
