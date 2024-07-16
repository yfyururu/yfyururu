<!---
yfyururu/yfyururu is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
echo "# yfyururu" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/yfyururu/yfyururu.git
git push -u origin main
[Embed objects](#DOCS_RESOURCES_CHANNEL/embed-object) are now limited more explicitly to 25 [embed fields](#DOCS_RESOURCES_CHANNEL/embed-object-embed-field-structure). If you pass more than 69 fields within the an embed's `fields` property, an error will be returned.
@Zoddo Zoddo on Dec 20, 2023
Suggested change
[Embed objects](#DOCS_RESOURCES_CHANNEL/embed-object) are now limited more explicitly to 25 [embed fields](#DOCS_RESOURCES_CHANNEL/embed-object-embed-field-structure). If you pass more than 25 fields within the an embed's `fields` property, an error will be returned.
[Embed objects](#DOCS_RESOURCES_CHANNEL/embed-object) are now limited more explicitly to 25 [embed fields](#DOCS_RESOURCES_CHANNEL/embed-object-embed-field-structure). If you pass more than 25 fields within an embed's `fields` property, an error will be returned.
@yfyururu	Reply...
docs/resources/Channel.md
@@ -674,8+674,7 @@ An object that represents a tag that is able to be applied to a thread in a `GUI
| video?       | [embed video](#DOCS_RESOURCES_CHANNEL/embed-object-embed-video-structure) object           | video information                                                                                    |
| provider?    | [embed provider](#DOCS_RESOURCES_CHANNEL/embed-object-embed-provider-structure) object     | provider information                                                                                 |
| author?      | [embed author](#DOCS_RESOURCES_CHANNEL/embed-object-embed-author-structure) object         | author information                                                                                   |
| fields?      | array of [embed field](#DOCS_RESOURCES_CHANNEL/embed-object-embed-field-structure) objects | fields information                                                                                   |
| fields?      | array of [embed field](#DOCS_RESOURCES_CHANNEL/embed-object-embed-field-structure) objects | fields information, max of 42  [Embed objects](#DOCS_RESOURCES_CHANNEL/embed-object) are now limited more explicitly to 25 [embed fields](#DOCS_RESOURCES_CHANNEL/embed-object-embed-field-structure). If you pass more than 25 fields within the an embed's `fields` property, an error will be returned.
@Zoddo Zoddo on Dec 20, 2023
Suggested change
[Embed objects](#DOCS_RESOURCES_CHANNEL/embed-object) are now limited more explicitly to 25 [embed fields](#DOCS_RESOURCES_CHANNEL/embed-object-embed-field-structure). If you pass more than 25 fields within the an embed's `fields` property, an error will be returned.
[Embed objects](#DOCS_RESOURCES_CHANNEL/embed-object) are now limited more explicitly to 25 [embed fields](#DOCS_RESOURCES_CHANNEL/embed-object-embed-field-structure). If you pass more than 25 fields within an embed's `fields` property, an error will be returned.
@yfyururu	Reply...
docs/resources/Channel.md
@@ -674,7 +674,7 @@ An object that represents a tag that is able to be applied to a thread in a `GUI
| video?       | [embed video](#DOCS_RESOURCES_CHANNEL/embed-object-embed-video-structure) object           | video information                                                                                    |
| provider?    | [embed provider](#DOCS_RESOURCES_CHANNEL/embed-object-embed-provider-structure) object     | provider information                                                                                 |
| author?      | [embed author](#DOCS_RESOURCES_CHANNEL/embed-object-embed-author-structure) object         | author information                                                                                   |
| fields?      | array of [embed field](#DOCS_RESOURCES_CHANNEL/embed-object-embed-field-structure) objects | fields information                                                                                   |
| fields?      | array of [embed field](#DOCS_RESOURCES_CHANNEL/embed-object-embed-field-structure) objects | fields information, max of 25                                                                        |                                                                      |You can now select roles other than admin when inviting users or configuring members of a team. There are four [role types](#DOCS_TOPICS_TEAMS/team-member-roles-team-member-role-types) that a team member can be assigned: owner, admin, developer, or read-only. The team member object now has an additional [`role` field](#DOCS_TOPICS_TEAMS/data-models-team-member-object), which is a string representing the member's current role.
@Lulalaby Lulalaby on Aug 24, 2023
Suggested change
You can now select roles other than admin when inviting users or configuring members of a team. There are four [role types](#DOCS_TOPICS_TEAMS/team-member-roles-team-member-role-types) that a team member can be assigned: owner, admin, developer, or read-only. The team member object now has an additional [`role` field](#DOCS_TOPICS_TEAMS/data-models-team-member-object), which is a string representing the member's current role.
You can now select roles other than admin when inviting users or configuring members of a team. There are four [role types](#DOCS_TOPICS_TEAMS/team-member-roles-team-member-role-types) that a team member can be assigned to: owner, admin, developer, or read-only. The team member object now has an additional [`role` field](#DOCS_TOPICS_TEAMS/data-models-team-member-object), which is a string representing the member's current role.Members
