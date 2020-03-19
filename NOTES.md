# Issues
* Cannot install the theme dependencies due to an integrity error with js-yaml(?) in the existing 
package-lock.json. 
  * Solution: Removed the package-lock.json, cap the version of bootstrap at 4.3.1 in package.json and run
  the install again
  

# Timelog
##10/Mar
* 4h - Setup docker and build the project, build the frontend and install drupal.

## 11/Mar
* 4h - Setup the content types, work through the issues in the requirements with Peter Mason.

## 12/Mar
* 4.5h - Finish setting up all content types as per latest spec, started setting displays and frontend. 
  Got stuck on a bug that 2-col more general template is getting picked up instead of a more specific one.
  
## 13/March  


# 
* List of things I couldn't finish.
  * Dropdown selector navigation between Issues on the Header block.
    * Suggestion: Use closest Higher/Lower issue instead of +1/-1 issue on the next/previous logic.
  * Header navigation styling
  * Country taxonomy integration on the vocabulary
  * Sidebar on the hub taxonomy term page (Needs extra fields for blocks + Display configuration)
  * Issue highlight Listing styling
  * Make hub updates expandable only on Issue pages (js + css fix)
  
  
Changelog:
* New vocab: Innovation hub
* New Content types:
  * Innovation tracker issue
  * Innovation tracker story
  * Hub update
* New view: Innovation Tracker Issue
* Updated view: Taxonomy term (disabled page displays, converted them to Block displays, and these blocks 
  are placed under content block)
* New module: ipu_innovation_tracker
* New configuration form: /admin/config/system/ipu-innovation-tracker (Translatable through Configuration Translation)
* New blocks: Innovation Tracker Header, Innovation Tracker Contribute (used from Issues)
* Various frontend changes