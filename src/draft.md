
# open API vendor extensions

The vendor extensions for open-API are used for the vendor to interpret the data specific to their platform.

Example;

The x-ms-summary denotes how Microsoft should able to process this data to display the element labels in the Ui. 

Like these we have multiple extensions which may not be understandable by other platforms. When developing connectors for a platform, the vendors may not force to use these extensions. But its recommended to include these extension for a better user experience.

You can take this vendor extension even to next level for building complex ui on the vendor platform. Example, using the capability extension you can create a filepicker ui for the user to choose the folder and files.

3 webhook




# dynamic request input schema




# dynamic response output Schema




# dealing with large connector base

- use reusable properties
  - Definitions
  - Parameters
- don't think of the minimizing Json. That may not work. Because this will fail during the certification process.
- use dynamic Schema For request and response





