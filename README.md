# Microsoft DevDiv Growth and Analytics Teram

This repository contains data dumps from the Stack Overflow Developer Survey for 2019-2021. 

Each year contains a CSV file using the following schema:

UserID | QuestionRef | Answer

Additionally, there is a "QuestionKey" which lists unique QuestionRefs, and whether or not they are present in a given year. This is based on the raw data from Stack Overflow, and as such there may be unique columns that answer the same questions (For examplel, DatabaseUsed vs UsedDatabase)

The data is currently in a "long" format, where each row is a response to a question. Respondents have been assigned an ID which is consistent across a single year, but not across years (e.g., All ResponseIds of 23 are for the same respondent for 2021, but this is not the same "person" as ResponseId 23 in 2020).

The data does _not_ need to stay in "long" format, it can be pivoted to a "wide" format, separated out into different tables/files or whatever else makes it easier to answer the questions posed. 

The data has not been entirely sanitized. There may be odd characters from time to time. Demographic data has been purged as to add as much anonymity as possible.

# Licenses/Fair Use Information 

Legal:

The Public 2021 Stack Overflow Developer Survey Results - is made available under the Open Database License (ODbL): http://opendatacommons.org/licenses/odbl/1.0/. Any rights in individual contents of the database are licensed under the Database Contents License: http://opendatacommons.org/licenses/dbcl/1.0/

The Public 2020 Stack Overflow Developer Survey Results - is made available under the Open Database License (ODbL): http://opendatacommons.org/licenses/odbl/1.0/. Any rights in individual contents of the database are licensed under the Database Contents License: http://opendatacommons.org/licenses/dbcl/1.0/

The Public 2019 Stack Overflow Developer Survey Results - is made available under the Open Database License (ODbL): http://opendatacommons.org/licenses/odbl/1.0/. Any rights in individual contents of the database are licensed under the Database Contents License: http://opendatacommons.org/licenses/dbcl/1.0/


TLDR: You are free to share, adapt, and create derivative works from The Public 2021 Stack Overflow Developer Survey Results as long as you attribute Stack Overflow, keep the database open (if you redistribute it), and continue to share-alike any adapted database under the ODbl.

