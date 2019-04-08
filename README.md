BOOKMARK MANAGER

This is a project to create an application that people can use to manage their bookmarked websites.

USER STORIES

As a user,
Ao that I can quickly go to websites I regularly visit,
I would like to see a list of bookmarks.

Domain Model of the above User Story

   Client         Controller       Model   View

 -----------          ----------     all     ----------
|           |   GET  |          |---------->|          |
|           |------->|          |<----------| Bookmark |
| /bookmarks|        |    app   |[bookmarks]|          |
|           |        |          |            ----------
|           |<-------|          |
|           |response|          |
 -----------          ----------
