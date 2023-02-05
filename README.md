# NovelGens Data Analysis

![Karystel](https://github.com/amymartika/novelgens-data-analysis/blob/main/karystel.png) ![Dounreleon](https://github.com/amymartika/novelgens-data-analysis/blob/main/dounreleon.png) ![Barrok](https://github.com/amymartika/novelgens-data-analysis/blob/main/barrok.png)

## Data source

The data consists of website data provided by Indent Labs' [NovelGens](https://www.novelgens.com/), which generates fictional creatures using AI.

## Business problem

Indent Labs used artificial intelligence to create 365 creatures in 2022 — one new, unique creature every day. Each creature was assigned a commonality, biome, tag, and paragraph of content. Users then had the ability to claim the creature, like the creature, create artwork of the creature, and/or write a story about the creature. 

The website collected anonymous feedback from users about each creature, asking: Is this creature memorable? Scary? Sad? Powerful? Unique? Comical? Comforting? Dangerous?

After producing creatures and collecting data for a year, Indent Labs seeks to better understand the trends between the qualitative data and the user-submitted feedback. They want to understand:

* **Which creatures claim superlatives** in each of the feedback categories? What factors contribute to this?
* **What trends exist** between creatures that share types, tags, and/or environments? What is the most common feedback associated with each of these data points?
* **What factors influence users to interact with each creature**, either by claiming it, liking it, or submitting new content about it? 

## Data cleaning

I received 20 .csv files from Indent Labs. I cleaned them using Google Sheets, eliminating unnecessary data, filling empty data, and reorganizing their structure before importing 16 tables to PostgreSQL.

1. **content_favorites**: The "likes" given to each creature, consisting of 5 columns and 408 rows.
2. **content_feedback**: User-submitted feedback about each creature, consisting of 18 columns and 4,652 rows.
3. **creature_environment_pairings**: The environments selected for each creature, consisting of 5 columns and 655 rows.
4. **creature_story_pairings**: The user-submitted stories and their respective creature(s), consisting of 5 columns and 20 rows.
5. **creature_tag_pairings**: The tags selected for each creature, consisting of 3 columns and 527 rows.
6. **creatures**: Published and drafted creatures, consisting of 8 columns and 369 rows.
7. **environment_story_pairings**: The environments selected for user-submitted stories, consisting of 5 columns and 2 rows.
8. **environment_submitted_image_pairings**: The environments selected for user-submitted images, consisting of 5 columns and 38 rows.
9. **environments**: All possible environments for creatures, consisting of 5 columns and 18 rows.
10. **ownership_contracts**: Creatures that have been claimed by users, consisting of 6 columns and 3,050 rows.
11. **profiles**: Profile pages for website users, consisting of 7 columns and 154 rows.
12. **submitted_content_kudos**: Kudos given by users to submitted stories and images by other users, consisting of 7 columns and 135 rows.
13. **submitted_images**: Images submitted by users about the creatures, consisting of 9 columns and 53 rows.
14. **submitted_stories**: Stories submitted by users about the creatures, consisting of 7 columns and 20 rows.
15. **tags**: All possible tags for creatures, consisting of 5 columns and 98 rows.
16. **users**: Encyrpted data on website users, consisting of 9 columns and 154 rows.

## Contact info

Please [reach out to me](https://www.linkedin.com/in/amymartikabrown/) if you have any questions or feedback.
