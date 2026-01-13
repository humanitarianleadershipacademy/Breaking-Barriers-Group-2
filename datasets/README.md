# AWS Breaking Barriers Synthetic Datasets

The Kaya learning management system has over 800 public courses, one-million learner records and two-million completion records. The following synthetic datasets are provided for this challenge:

| File | Description |
| --- | --- |
| [/datasets/courses.csv](./courses.csv) | Public courses on the Kaya LMS |
| [/datasets/learners.csv](./learners.csv) | Synthetic learner records |
| [/datasets/completions.csv](./completions.csv) | Synthetic completion records |

## Course Fields
| Field | Type | Description |
| --- | --- | --- |
| id | UID | Unique identifer for each course |
| name | String | Name of the course |
| summary | Text | Short description of the course learning content |
| provider | String | Authors of the learning content, multiple providers seperated by comma |
| language | String | Two-digit course language code, multiple languages seperated by comma |
| url | URL | Full link to the course sign-up page |
| thumbnail | URL | Full link to the course thumbnail image (~500x330px) |
| tags | String Array | Comma seperated list of the course's tags, represented as URl-safe strings |

## Learner Fields
| Field | Type | Description |
| --- | --- | --- |
| id | UID | Unique identifer for each learner |
| country | String | Name of the country wher learner signed-up to the Kaya LMS |
| gender | String | Preset gender values: "Female", "Male", "Not specified" |
| age | String | Preset age ranges: "< 21", "21-31", "32-41", "42-51", "52-61", "62+", "Not specified" |

## Completion Fields
| Field | Type | Description |
| --- | --- | --- |
| learner | UID | Unique learner identifer for many-to-many join |
| course | UID | Unique course identifer for many-to-many join |

