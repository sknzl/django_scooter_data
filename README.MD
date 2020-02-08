# Django Scooter Data
Project related to the article in my [blog](https://sknzl.github.io/tracking-electric-scooters-in-lisbon/)

# How to use
The foldername indicates the time frame in which the data was recorded. The first data-set was recorded from 19th August 2019 to 8th December 2019.
The zip file in the folder contains 2 csv files:

## scooters.csv
A list of all scooters that were recorded.
- `id` is the unique id attributed to each scooter.
- `scooter_id` is the unique id used by Circ to identify the scooter.
- `last_lng` and `last_lat` are the last known coordinates of the scooter.
- `distance_travelled` is the total distance in meters the scooter was moving.
- `created` is the timestamp the scooter was first seen.
- `updated` is the timestamp the scooter was last seen.

## scooter_activities.csv
A list of all recorded scooter positions.
- `scooter_id` identifies for which unique scooter id the position was logged (refers to `id` in scooters.csv).
- `lat` and `lng` are the coordinates.
- `created` is the timestamp the position was logged.


# License
[![CC BY 4.0][cc-by-shield]][cc-by]

This work is licensed under a [Creative Commons Attribution 4.0 International
License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg