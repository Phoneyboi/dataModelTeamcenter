# Item Type
Item Types are a data structure that define a specific type of data.

Lets distiguish the difference between an Item Type and an Item because it will help us understand what is specifically an Item Type. An Item Type is different than an Item in that an Item Type is how an Item is defined. For example, I can have an item type that specifically holds data that related to electrical components and an item type that is specifically related to mechanical components. These two separate Item Types, electrical and mechancical, have different attributes defined to each other. A specific example could be that for an electrical component you need to have an attribute of 'voltage rating'. In contrast, the mechanical part would hold data that does not discern the concept of voltage, making that information irrelevant. 

## Item and Item Revisions
Whereas an Item Type is how Items are defined, the Item itself is defined by its data. An Item is the umbrella structure that holds Item Revision(s), an Item Revision is the sub-umbrella structure that holds the data. Within an Item Revision you will have the ability to define attributes and add datasets. When needing to roll a revision, the Item Revision is what will be revised. This is sometimes confused with users who are used to rolling a revision on an individual file. Inside an Item Revision, the file (dataset) is a function of the Item Revision which requires a new Item Revision with the updated dataset. 

## Comparison: File Based Systems vs. Item Based Systems
I alluded to the difference of file and item based systems in my previous paragraph. I am sure this section will draw some controversy but I will do my best to explain my expereience with the two. 

A file based system is one where the files are structured similarly to your File Explorer window on your computer if you are running a WindowsOS. Authorized users are able to create folders and search on the established folder structure. Within these folders, authorized users can add their CAD files, PDFs, images, etc. 

An item based system is one where authorized users create a bucket to hold their CAD files, PDFs, images, etc. This bucket is called, you guessed it, an Item. It is this bucket that the user is able to search for when browsing for data.

## Personal Opinion Alert: Why Item Based Systems are Better
### Good Data Practice
For this specific opinion, I am assuming your business releases a PDF for manufacture. Revision controlling a PDF separate from the engineering drawing or the CAD model is a practice I would consider unsecure. I can hear you through my screen, "But Hutch, you can send the PDF and the CAD file in the same workflow". You are correct with this statement, but for file based systems the inherent relationship between the CAD file and the PDF of the CAD file is not defined as a single, revisionable unit which is the case in an Item based system.

I would also add that engineers, by their nature, are creatures who are constantly attempting to maximize efficiency. The plight of the modern engineer is that the process of engineering requires far too many 'clicks'. Sending a single Item Revision through a workflow which holds the CAD file and its associated PDF reduces these clicks and keeps your data well managed. 

To play devils advocate, my opinion for holding these datasets in one revisionable unit falls apart if you are a business that is not concerned with keeping your CAD models up to date with the PDF or other associated dataset types you release to manufacturing. I will warn that this causes problems later when a revision needs to be made or a configuration is derived from your released PDF. This gets into the idea of your source-of-truth. It is possible that the released PDF will not match the CAD drawing which begs the question, is the PDF definition correct or the CAD file definition?
