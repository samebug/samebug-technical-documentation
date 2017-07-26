# Workspaces and permissions

A workspace usually corresponds to a team of developers working on a project. A Samebug user can access to multiple workspaces and a workspace can be associated with multiple users. Workspaces are useful to organize and control the visibility of content generated during the project development.

## Workspace visibility

Your activity on Samebug will always happen in the workspace you specified. When you create new content it will inherit the visibility of the workspace, so if you are working in a `Searchable` workspace and you send a crash to Samebug, your crash will be created under that workspace with `Searchable` visibility.

## Workspace permissions

You can grant access to other Samebug users for your workspace by adding different permissions. These permissions are:

| Permission name | Available actions |
|---|---|
| Admin  | can manage the workspace, grant or revoke permission of workspace users, change workspace settings |
| Read   | can see the stack trace details of content in the workspace (as if it was `Public` for him) |
| Search | can find content in the workspace by stack trace search (but not see the details, as if it was `Searchable` for him) |
| Write  | can create new content in the workspace, i.e. can send crash or create tip |

## Default workspace

As we mentioned, any activity you do on Samebug happens in a workspace. If you do not specify it otherwise, this is your Default Workspace, created along with your Samebug user. You have every permission on your Default Workspace, and it is on `Searchable` [visibility](/docs/privacy) by default.

## Managing workspaces

At the moment workspaces are an invisible feature. If you want to create new workspace, invite other users or change
the default visibility, please [contact us](mailto:hello@samebug.io)
