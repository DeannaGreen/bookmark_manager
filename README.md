BOOKMARK MANAGER

This is a project to create an application that people can use to manage their bookmarked websites.

USER STORIES

As a user,
Ao that I can quickly go to websites I regularly visit,
I would like to see a list of bookmarks.

Domain Model of the above User Story

   Client         Controller                   Model         View

 -----------          ----------     all     ----------
|           |   GET  |          |---------->|          |
|           |------->|          |<----------| Bookmark |
| /bookmarks|        |    app   |[bookmarks]|          |
|           |        |          |            ----------
|           |<-------|          |--------------------> -------------
|           |response|          |     [bookmarks]     |             |
 -----------          ---------- <--------------------|erb bookmarks|
                                          html        |             |
                                                       -------------

How to Set Up the Database

1. Connect to psql
2. Create the database using the psql command CREATE DATABASE bookmark_manager;
3. Connect to the database using the psql command \c bookmark_manager;
4. Run the query we have saved in the file 01_create_bookmarks_table.sql


Test Database

1. Connect to psql
2. Create the database using the psql command CREATE DATABASE bookmark_manager_test;
3. Connect to the database using the psql command \c bookmark_manager_test;
4. Run the query we have saved in the file 01_create_bookmarks_table.sql
