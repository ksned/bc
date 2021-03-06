# AEM Breadcrumb sample component

This is an AEM 6.2 implementation for a breadcrumb component.

## How to build

Install the package **breadcrumb-kirk.zip** using the AEM package manager.

## How to use
After install, use Design mode to choose this component from the "KIRK" category.

In Edit mode, drop the component on to a nested page.

Open the dialog. There are two configuration options:
  - Level from top: allows the author to start breadcrumbs from any number of levels down from the root (/content, 0)
  - Hide current page: allows the author to hide the current page from the breadcrumb list (extra functionality)

Pages that have the "Hide In Navigation" option checked in the Page Properties will not show in the list.

## Implementation
  - This component uses a JS use class for its backend and clientlibs for minimal styling.

## Make it Better
  - Don't use JS use class (I am not a Java dev, and I didn't want to use the OOB breadcrumb backend)
  - 6.3 finally handles dialog checbkboxes properly. For 6.2, I used a hidden field in the dialog to force the Boolean. Refactor for 6.3.
  - Dynamic link checker will fail on non-page resources.
  - I added an HTML extension manually in HTL - it should go to the backend
  - Maybe add an option for the author to start *on the current page* and go up from there?




