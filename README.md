# Blazor Rich Text Editor — File Manager

A Blazor Server sample showing how to integrate a File Manager with the Rich Text Editor to browse server files and insert images into editor content.

## Project Overview

This sample demonstrates adding a custom File Manager toolbar button to the `SfRichTextEditor`. Clicking the button opens a modal `SfFileManager` dialog, lets the user browse or upload images, and inserts the selected image into the editor using `ExecuteCommandAsync`.

## Key Points

- Adds a custom toolbar item that opens a modal File Manager dialog
- Uses `SfFileManager` for browsing, upload, and selection
- Inserts selected images into the editor by restoring the editor selection and executing the `InsertImage` command

## Prerequisites

- .NET 8.0 SDK
- Visual Studio 2022+ or VS Code
- Syncfusion Blazor packages and license (if required)

## Setup & Running Steps

Installation

```bash
git clone https://github.com/SyncfusionExamples/blazor-richtexteditor-filemanager.git
cd blazor-richtexteditor-filemanager
```

Restore NuGet packages

```bash
dotnet restore
```

Run the application

```bash
dotnet run
```

## Usage

1. Open the sample in the browser and focus the Rich Text Editor.
2. Click the custom File Manager button in the toolbar to open the dialog.
3. Browse or upload images; select an image (PNG/JPG/JPEG) and click Insert. The sample restores the saved editor selection and inserts the image using a server image URL.

## Troubleshooting

- Ensure the FileManager Ajax endpoints (`FileOperations`, `Upload`, `Download`, `GetImage`) are reachable and configured for your environment.
- Verify CORS, authentication, and file permissions if uploads or image retrieval fail.

## Support

This sample is provided for demonstration purposes. For issues, open an issue in the repository.

## See also

- [Online examples](https://blazor.syncfusion.com/demos/rich-text-editor/overview?theme=fluent2)
- [Documentation](https://blazor.syncfusion.com/documentation/rich-text-editor/getting-started-webapp)

>Looking for the full Blazor Rich Text Editor component overview, features, pricing, and documentation? Visit the [Blazor Rich Text Editor](https://www.syncfusion.com/blazor-components/blazor-rich-text-editor) page.
