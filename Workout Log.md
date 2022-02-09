# Custom Workout Log for Prague

This is a Dataview code I made to help out [Prague](https://thebuccaneersbounty.wordpress.com/2022/01/05/how-i-use-the-daily-notes-plugin-a-comprehensive-guide/#comment-34) with his custom workout log.

## Workout Logs
---

```dataview
TABLE WITHOUT ID link(file.link, " ") + "<strong> 🏋️‍♀️" + Progression-Week  + " | " + Progression-Day + "</strong>" + "<br>" 

+ Exercise1 + " [" + Exercise1MuscleGroup + "] = " + Exercise1Sets + "x" + Exercise1Reps  + " (" + Exercise1Weight + ")"  + "<br>" 
+ Exercise2 + " [" + Exercise1MuscleGroup + "] = " + Exercise2Sets + "x" + Exercise2Reps  + " (" + Exercise2Weight + ")"  + "<br>" 
+ Exercise3 + " [" + Exercise1MuscleGroup + "] = " + Exercise3Sets + "x" + Exercise3Reps  + " (" + Exercise3Weight + ")"  + "<br>" 
+ Exercise4 + " [" + Exercise1MuscleGroup + "] = " + Exercise4Sets + "x" + Exercise4Reps  + " (" + Exercise4Weight + ")"  + "<br>" 


+ file.link as Entries

from "Daily Notes"
SORT file.name desc
```