# About the Data - Rumble
## COMP2420 Semester 1, 2020
## Assignment 2

The following document is designed to give you an introduction to the data you
are working with.

## Data Table
The below table provides an outline of the data, broken down into the columns
the dataset features. Note that the column name may vary slightly between files.

| Column Name   | Description               |
| :------------ | :------------------------ |
| Draw          | The number of the entrant |
| Entrant       | The Entrant's name        |
| Brand         | Brand division, only exists in files for 2003-2011 and 2017 or later |
| Order         | The position of which the entrant was eliminated |
| Eliminated by | Name of the entrant who eliminated them<br>This may be multiple entrants, in which case it is semicolon-delimited (';')<br>If this is "Winner", then this indicates that the entrant won the event (never eliminated) |
| Time          | The amount of time (in minutes) the entrant was in the match<br>If this is '00:00', don't include them as a participant in the match; the reason will be given in `Eliminated by` |
| Eliminations  | The number of entrants they eliminated |
