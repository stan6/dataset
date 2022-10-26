# uirepair-dataset

## Format for the name of the folder for each (old, new) pair:
website name: YouTube

Old version: 1.0

New version: 2.0

Each folder has the name:
``<Website name>-<Old version>-<New version>``
 
 For this example, the folder name should be ``YouTube-1.0-2.0''


## Format for Labeled Text Matching (all labeled texts are stored at labeled-text.csv)

Example:

website name: YouTube

Old version: 1.0

New version: 2.0

Columns in labeled-text.csv:

Website name,Old version,New version, Text in Old version,The correct text in New version
YouTube, 1.0, 2.0,text1,text2

So, the table will look like:

| Website name | Old version | New version| Text in Old version |The correct text in New version |
| --- | --- | --- | --- | --- |
| YouTube | 1.0 | 2.0 |text1 | text2 |





## Labeled Image matching (starts with image-* prefix):

Example (Each image in each version should have an image id starting from 1, a deleted image has image id 0):

website name: YouTube

Old version: 1.0

New version: 2.0

Image Id in Old version: 1

The correct Image Id in New version: 2

- Each image in the old version then has the name:
``image-<Website name>-<Old version>-<New version>-old<Image Id in Old version>-new<The correct Image Id in New version>``

- Each image in the new version then has the name:
``image-<Website name>-<Old version>-<New version>-new<Image Id in New version>``

For this example, the old image name should be ``image-YouTube-1.0-2.0-old1-new2`` (we specify the correct matching new image in the id for old image to make it easier to search for matching). The correct new image name should be ``image-YouTube-1.0-2.0-new2``.
