---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Workspaces
date: 2025-11-03 09:48:58 -0500
relpath: ../
---

# Workspaces
> A _workspace_ is simply a folder on your computer where Praisenter will store all content that you import, create, and use.
{: .p-man-page-intro}

Workspaces represent an isolated collection of content.  For example, you can create two workspaces, one for your main service and a different one for youth services.  Having these two workspaces mean that the content (things like pictures, videos, bibles, etc.) are separated.

You must select a workspace before launching Praisenter.

## Creating workspaces[#](#creating-workspaces)
You are prompted to create a workspace on your first run of Praisenter.  Praisenter will setup a few things to initialize your workspace, but these steps happen automatically.  Every time Praisenter is started, you are prompted to select the workspace to open.

![Alt text]({{ page.relpath }}assets/img/workspace-selection.png){: .rounded .img-fluid}

- You can use the text box to select a previously selected workspace
- You can use the text box to type in a path to a folder
- You can use the folder icon to select folder

You will receive an error if you choose a folder that's not empty unless Praisenter detects it's an existing workspace. Once you have selected the workspace, click the Launch button to continue.

## Switching workspaces[#](#switching-workspaces)
Because Praisenter can have many workspaces, you can switch between those workspaces.  You can choose the workspace when you launch Praisenter as shown in the [Creating a workspace](#creating-a-workspace) section or you can switch workspaces after Praisenter has been launched by using the `File` -> `Switch Workspace` menu.

Switching a workspace closes the current workspace first. This means that any unsaved documents will need to be saved or discarded and that any content you are presenting will be cleared.

You can also create a new workspace from the `File` -> `Switch Workspace` menu. Just like switching, you want to make sure any unsaved documents are saved or discarded and that any content you are presenting is cleared.

## Removing workspaces[#](#removing-workspaces)
As of version 3.1.7, there isn't a way to remove a workspace from the application.  

If you want to clean up your workspaces you can delete the `workspaces.json` file stored in `C:\Users\your_user_name\.Praisenter3` on [Windows](https://apps.microsoft.com/detail/9phhwb94w800) or `/home/your_user_name/snap/praisenter/common/.Praisenter3` on Ubuntu using the [Snap](https://snapcraft.io/praisenter) or `/home/your_user_name/.Praisenter3` on Ubuntu when manually installing the `.deb`.  This will clear the list of previously selected workspaces.  Just select the folder again to open an existing workspace.

If you are savvy enough, you can alternatively _edit_ the `workspaces.json` file. You'll want to edit the `workspaces` and the `lastSelectedWorkspace` properties.  You can freely delete those file locations as well.

## Workspace upgrade[#](#workspace-upgrade)
When selecing a workspace, Praisenter attempts to detect if it's an empty folder or an existing workspace.  If it's an existing workspace, it should be fine to open that workspace, but be aware that the workspace will be updated to the latest version.  Updating the workspace version is usually a minor activity, but there could be version updates in the future that could take a significant amount of time to upgrade or prevent upgrading entirely.