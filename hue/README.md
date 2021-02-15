# hue ios shortcuts

Helper shortcuts to automatically disable my wake up light schedule, if the string "PTO" is found in any of the current day events. 
Runs daily at 1AM. Calender lookup logic is owned by an iOS automation, outside of these shortcuts.

This works by updating a hardcoded schedule (ID=1) status attribute to either "enabled" or "disabled".
Ref https://developers.meethue.com/develop/hue-api/3-schedules-api/#set-schedule-attr

Secrets that need to be manually updated within the Shortcuts app:
- $SECRET_HUE_USERNAME$ 

Future considerations: 
- Make the schedule ID lookup dynamic by accepting a string for the schedule name itself
- Add calendar lookup logic as a shortcut