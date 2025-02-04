[DEPRECATED] The Office JS Snippet Explorer is no longer supported. To get the latest snippets for Office-JS, we recommend developers to try the [Script Lab](https://store.office.com/en-001/app.aspx?assetid=WA104380862&ui=en-US&rs=en-001&ad=US&appredirect=false) add-in.

# OfficeJS Snippet Explorer

This Office Add-in sample uses Angular. It lets you explore and modify code snippets for ExcelJS and WordJS. You can browse the code snippets at these two locations:

- [Word](https://officesnippetexplorer.azurewebsites.net/#/snippets/word)
- [Excel](https://officesnippetexplorer.azurewebsites.net/#/snippets/excel)

IntelliSense is enabled so that you can see which properties and methods are available on each object. We highly suggest that you run this sample in Excel and Word after you browse the available snippets. The next two sections will show you how you can make this add-in available in Excel and Word.

## Run OfficeJS Snippet Explorer in Excel 2016

Do the following steps to run this sample in Excel 2016:

1. Create a folder on a network share called `manifests`.
2. Save the snippet-explorer-excelJS.xml file in the network share.
3. Open Excel 2016 with a new workbook.
4. Select **File** > **Options** > **Trust Center** > **Trust Center Settings** > **Trusted Add-in Catalogs**.
5. In the **Catalog Url** field, add the url to the `manifests` folder you created on the network share. Select the **Add catalog** button.
6. Check the **Show in menu** button and then select **OK**.
7. Select **Insert** > **My Add-ins** > **Shared Folder**.
8. Select the add-in named excel-js-snippet-explorer and select **Insert**. The add-in will load.
9. You can now run the code samples. We suggest that you play with the snippets in the code editor to see what you can do with ExcelJS.

## Run OfficeJS Snippet Explorer in Word 2016

Do the following steps to run this sample in Word 2016:

1. Once you have cloned or downloaded the repo, create a folder on a network share called `manifests`.
2. Save the snippet-explorer-wordJS.xml file in the network share.
3. Open Word 2016 with a new document.
4. Select **File** > **Options** > **Trust Center** > **Trust Center Settings** > **Trusted Add-in Catalogs**.
5. In the **Catalog Url** field, add the url to the `manifests` folder you created on the network share. Select the **Add catalog** button.
6. Check the **Show in menu** button and then select **OK**.
7. Select **Insert** > **My Add-ins** > **Shared Folder**.
8. Select the add-in named word-js-snippet-explorer and select **Insert**. The add-in will load.
9. You can now run the code samples. We suggest that you play with the snippets in the code editor to see what you can do with WordJS.

> **Note**: You might need to close and reopen Word in order for the add-in to show.

## Contributing

You will need to sign a [Contributor License Agreement](https://cla.microsoft.com) before submitting your pull request. To complete the Contributor License Agreement (CLA), you will need to submit a request via the form and then electronically sign the Contributor License Agreement when you receive the email containing the link to the document.

This sample is open for pull requests to add snippets to this repository. You can add to the snippets in either the excel-snippets or word-snippets directories. Here's what you do to add a snippet:

1. Create a fork of this repository.
2. Create a JS file in the excel-snippets or word-snippets directory with a descriptive name. Take a look at the existing file names for ideas on how you should name the file.
3. Add your snippet to the file.
4. Open samples.json.
5. Add an entry to the `values` array. Your entry will look like:

   `{ "done": true, "filename": "YOURFILENAME", "name": "DISPLAYNAME", "group": "GROUPNAMEFROMGROUPS", "description": "ASIMPLEDESCRIPTION"}`

6. Replace the value for the filename, name, group, and description fields with information that describes your snippet. The filename should take the form of {object}{method}{description}.js. The object name is required -- this makes the list of snippets easy to peruse. For example: paragraphClear.js or rangeInsertText.js.
7. Save all of your changes, test it, push it, and open your pull request.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information, see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Additional resources

Learn more about these APIs by [reading the documentation](https://github.com/OfficeDev/office-js-docs).

Visit [http://dev.office.com](http://dev.office.com) for all your Office 365 Development needs

- Get started with Office 365 development at [http://dev.office.com/getting-started](http://dev.office.com/getting-started)
- Browse our full collection of Code Samples at [http://dev.office.com/code-samples](http://dev.office.com/code-samples)
- Watch on-demand video training at [http://dev.office.com/training](http://dev.office.com/training)
- Subscribe to the weekly podcast at [http://dev.office.com/podcasts](http://dev.office.com/podcasts)
- Try our APIs at [https://apisandbox.msdn.microsoft.com/](https://apisandbox.msdn.microsoft.com/)
- Follow us on [@officeDev](http://twitter.com/OfficeDev) and [Facebook](http://www.facebook.com/OfficeDev)
- Give us your feedback
- Submit Issues directly against this repo
- Submit feedback on [UserVoice](http://officespdev.uservoice.com/)
