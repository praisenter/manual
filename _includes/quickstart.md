# Quick start
> Welcome to the Quick Start Guide! Here, we'll walk through the steps to get you up and running quickly. For more detailed information, you'll find links to other sections of the manual.
{: .p-man-page-intro}

After following this guide, you should have Praisenter installed, displays configured, a Bible imported, and a slide presented. There's a lot more you can do with Praisenter, so feel free to explore additional features!

## 1. System configuration[#](#qs-configure-system)
{: #qs-configure-system}
Before you start Praisenter, make sure your displays are properly configured. Connect all your devices (monitors, projectors, TVs, etc.) to your computer and set your display mode to `Extend` so you can move windows between them. For more details, see the [Display setup]({{ page.relpath }}{{ page.displays_page }}#display-setup) section of the manual.

Once your displays are connected and you can drag applications between them, move on to the next step.

> **NOTE**: You don't _have_ to finish your system setup before starting.  Praisenter will detect when displays are added, removed, or changed. However, having everything configured ahead of time allows Praisenter to _auto-configure_ your displays, which speeds up the quick start process.

## 2. Install Praisenter[#](#install)
{: #qs-install}
There are two way to install Praisenter: Download from the store or install manually.  The recommended way is to download from the store.

> **NOTE**: Praisenter is released on the Microsoft and Snap Stores, but don't worry, it's free.

For **Windows**:

<a href="https://apps.microsoft.com/detail/Praisenter/9PHHWB94W800?launch=true&amp;mode=mini">
    <img src="{{ page.relpath }}assets/img/windows-download-icon.svg" height="82">
</a>

For **Ubuntu**:

<a href="https://snapcraft.io/praisenter">
    <img alt="Get it from the Snap Store" src="{{ page.relpath }}assets/img/ubuntu-download-icon.svg" height="82">
</a>

For **macOS**

<a href="https://apps.apple.com/us/app/praisenter/id6756894623?mt=12&itscg=30200&itsct=apps_box_badge&mttnsubad=6756894623" style="display: inline-block;">
    <img src="https://toolbox.marketingtools.apple.com/api/v2/badges/download-on-the-app-store/black/en-us?releaseDate=1769472000" alt="Download on the App Store" style="width: 246px; height: 82px; vertical-align: middle; object-fit: contain;" />
</a>

Praisenter is available on the Windows, Snap, and macOS App Stores.  Using the app store is the safest way to ensure you get an official version of Praisenter.  Praisenter can also be downloaded as an `MSI` or `DEB` from the [project site under the Releases section](https://github.com/praisenter/praisenter/releases), but these builds require more steps to install properly.  If you need help with manual install steps, see [this article](https://praisenter.org/install).

> **NOTE**: Praisenter is open source, so if none of the options above work for you, you can always try building Praisenter yourself by cloning the [GitHub repo](https://github.com/praisenter/praisenter).

Once installation is complete, launch Praisenter and continue to the next step.

## 3. Create a workspace[#](#qs-create-workspace)
{: #qs-create-workspace}
Every time you start Praisenter, you'll be prompted to [create a workspace]({{ page.relpath }}{{ page.workspaces_page }}#creating-workspaces).  A workspace is simply a folder on your computer that Praisenter uses to store its settings, Bibles, song lyrics, videos, and other content.  You can have multiple workspaces on one computer and [switch between them]({{ page.relpath }}{{ page.workspaces_page }}#switching-workspaces).

To continue, create a new folder, and select it as the workspace.  Then click `Launch`.

![workspace selection]({{ page.relpath }}assets/img/workspace-selection.png){: .rounded .img-fluid}

## 4. Setup displays[#](#qs-setup-displays)
{: #qs-setup-displays}
After selecting a workspace, the first screen you'll see is the [Present tab]({{ page.relpath }}{{ page.present_page }}#present) where you can control your configured displays.  Each display is assigned a [_display controller_]({{ page.relpath }}{{ page.displays_page }}#display-controllers), allowing you to control them independently.  In the example below, Praisenter detected 3 displays and automatically created a _display controller_ for display #2 (named `# ID=2 (-1920,0) 1920x1080`).  If you're not sure which display corresponds to which controller, use the [identify displays]({{ page.relpath }}{{ page.displays_page }}#identifying-a-display) feature.

By default, Praisenter will choose one display as the primary display, but you can [add more]({{ page.relpath }}{{ page.displays_page }}#adding-displays) or change the primary at any time.

Once you have at least one display controller ready, proceed to the next step.

![display controller example]({{ page.relpath }}assets/img/present-controller.png){: .rounded .img-fluid}

## 5. Import a Bible[#](#qs-download-bible)
{: #qs-import-bible}
Next, download a Bible from one of the [supported sources]({{ page.relpath }}{{ page.bibles_page }}#bibles) and [import]({{ page.relpath }}{{ page.library_page }}#importing-content) it into Praisenter.  You can download as many as you need and import them all at one time.  The easiest way is to download an [Unbound Bible](https://github.com/praisenter/unbound-bible-archive) by using the `Help` -> `Download Unbound Bibles` menu option.

![Bible download links]({{ page.relpath }}assets/img/misc-help.png){: .rounded .img-fluid}

Once your downloads are complete, [drag-and-drop]({{ page.relpath }}{{ page.library_page }}#importing-content) the files into the Praisenter window or use the `File` -> `Import` menu.  When the import finishes, continue to the next step.

> **NOTE**: You can skip this step if you don't plan to use Praisenter for displaying Bible verses.

> **NOTE**: If you can't find the version or translation you are looking for, you can use the [Bible editor]({{ page.relpath }}{{ page.bibles_page }}#books--chapters--verses) to create a new one.  Within the editor, use the [bulk edit]({{ page.relpath }}{{ page.bibles_page }}#bulk-edit) feature to quickly enter entire chapters or books.

## 6. Create slides[#](#qs-create-slides)
{: #qs-create-slides}
Now create a slide by going to the `File` menu and selecting `New Slide`.  From there, you can add [placeholders]({{ page.relpath }}{{ page.slidecomponents_page }}#placeholder-component), [media]({{ page.relpath }}{{ page.slidecomponents_page }}#media-component), and other content.  

Be sure to `Save` your slide, then continue to the next step.

> **NOTE**: If you're in a hurry, you can skip this step by using the sample slides provided.

## 7. Present slides[#](#qs-present-slides)
{: #qs-present-slides}
With your displays configured, Bible(s) imported, and slides created, you're ready to present.  Go back to the Present tab.  On the [Bible]({{ page.relpath }}{{ page.bibles_page }}#presenting-bible-verses) tab select a [slide template]({{ page.relpath }}{{ page.slides_page }}#slide-basics).

![presenting bibles select template]({{ page.relpath }}assets/img/present-bible-verses-template.png){: .rounded .img-fluid}

Then pick the Bible you imported earlier (or the sample Bible if you skipped the import).  Click the `Find` button to locate the verse and update the [Slide Preview]({{ page.relpath }}{{ page.present_page }}#slide-preview).

![presenting bibles select bibles]({{ page.relpath }}assets/img/present-bible-verses-bibles.png){: .rounded .img-fluid}

Click the `Show` button to show the slide on the display.  Finally, use the `Hide` button to clear the slide from the display.


