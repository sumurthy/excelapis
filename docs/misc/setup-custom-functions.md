# Setup

These instructions will let you set up your computer to preview custom functions in Excel. You'll need a Windows PC for now - the preview hasn't been released for Mac or other platforms yet.

## Office Insider Program
Join the [Office Insider program](https://products.office.com/en-us/office-insider?tab=Windows-Desktop) to install the version of Excel 2016 that's required for custom functions on your computer (must also be version 16.8711 or later). You must choose the "Insider" channel for the custom functions preview to work.

## Open starter tempalate

We've prepared a sample add-in with several custom functions. Download the [Excel-Custom-Functions](https://github.com/OfficeDev/Excel-Custom-Functions) code or clone the repo. 

Host the files on a web server. You can follow the steps below to host and edit them quickly via Azure Portal, or you can choose any alternate method like hosting on some other server or install IIS and host locally on your machine.
  1. Go to [https://portal.azure.com](https://portal.azure.com) and sign in with a Microsoft account.
  2. Create a resource > Web App
  3. Sign up for a subscription if you don't already have one (requires a credit card for verification but you won't be charged unless you explicitly convert to a paid service, which isn't required for this walkthrough).
  4. Choose a name for your web app. Other settings can be left on their defaults. Choose "pin to dashboard" and click Create
  5. Wait for your web app to deploy (around 30-90 seconds)
  6. In your Web App resource, scroll down and choose "App Service Editor (Preview)" under Development Tools
  7. In WWWROOT, choose "Upload Files" and upload the HTML and JS files in the sample. (Alternatively, if you prefer your own editor/client, you can deploy to the Azure Web App with git.)
  8. Copy 

