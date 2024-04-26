# TV Viewer Behaviour Dataset

## Overview

This dataset is derived from the _first-party data_ of **freeview linear television** in a European region, serving a population of over **5 million** individuals with a **high internet penetration rate** of over 85%. The dataset spans a **one-year** collection period (**52 weeks**) comprising **62,911,754 sessions** recorded from **352,987 unique devices** connected via _HbbTV_.

## Dataset Details

- **Data Source:** First-party data of freeview linear television
- **Population Served:** Over 5 million individuals
- **Internet Penetration Rate:** Over 85%
- **Collection Period:** One year (52 weeks)
- **Sessions Recorded:** 62,911,754
- **Unique Devices:** 352,987

## Data Processing and Classification

- Television programmes were classified based on a new content taxonomy devised in this research.
- Viewership levels were classified into four distinct categories:
  - **fan**
  - **regular**
  - **occasional**
  - **non-viewers**
- A session is defined from when a device tunes in to a channel until the viewer switches to another channel. Short **zapping** sessions (less than _300 seconds_) and **extreme** sessions (more than _10,800 seconds_) were filtered out for analysis.
- The dataset underwent processing to exclude non-compliant sessions, focusing on the first **19,386 devices** with the highest activity (only devices labelled as **'regular'** and **'fan'**).

## Features Included

The dataset includes additional columns providing insights into different aspects of viewership and engagement:

- **total_viewing_weeks**: weeks in which the device engaged in valid viewing sessions
- **total_viewing_duration**: cumulative duration of valid viewing sessions (seconds)
- **genre_number_weeks_viewed**: weeks during which a specific genre was watched
- **genre_number_weeks_broadcasted**: weeks during which a specific genre was broadcasted
- **genre_median**: median relevance score for a specific genre
- **genre_total_relevance**: cumulative relevance score for a particular genre (seconds)
- **genre_rae**: relative audience engagement metric for a specific genre
- **genre_wrae**: weighted RAE metric for a specific genre
- **genre_nwrae**: normalised WRAE metric for a specific genre
- **kids_content**: enthusiast, regular, occasional, no_commitment
- **Clusters from cluster analysis**: weekdays (morning, lunch, afternoon, evening, dinner) and weekend (morning, lunch, evening, dinner, afterdinner-night)

## Dataset Metrics

The dataset comprises 138 individual independent variables encompassing **19 distinct genres**. For device classification purposes, a **subset of 31 features** was utilised, capturing essential aspects of viewer engagement, genre relevance, and behavioural tendencies. Additionally, each device was classified based on a well-established approach in sociodemographic research, aligning their usage timing and preferred content genres with a **household taxonomy** based on _life cycle stages_, including:

- **Couple with young kids (0-8 years)**
- **Couple with teenagers (9-17 years)**
- **Couple with adult children (18+ years)**
- **Only young adults (18-35 years)**
- **Only middle-aged adults (36+ years)**
- **Seniors (elderly/retired adults)**

Specifically, the 31 features utilized for conducting the classification of households were:

- **viewership**
- **weekdays**
- **weekend**
- **genre_nwrae** (for each of the _19 genres_)
- **kids_presence**
