# Item Type
Item Types are a data structure that define a specific type of data. The creation of various Item Types are used as a means to effectively organize data the business creates. For example, I can have an item type that specifically holds data that related to electrical components and an item type that is specifically related to mechanical components. These two separate Item Types, electrical and mechanical, have different attributes defined to each other. A specific example could be that for an electrical component you need to have an attribute of 'voltage rating'. In contrast, the mechanical part would hold data that does not discern the concept of voltage, making that information irrelevant. 

## Item and Item Revisions
Whereas Item Types are how an Item is defined, the Item itself is defined by its data. An Item is the abstract entity that holds Item Revision(s), an Item Revision is the sub-structure that holds the data. Within an Item Revision you will have the ability to define attributes and add datasets. When needing to roll a revision, the Item Revision is what will be revised. This is sometimes confused with users who are used to rolling a revision on an individual file. All of the data in an Item Revision will be revised if a new revision is made. 

## Comparison: File Based Systems vs. Item Based Systems
I alluded to the difference of file and item based systems in my previous paragraph.

A file based system is one where the files are structured similarly to your File Explorer window on your computer. Authorized users are able to create folders and search on the established folder structure. Within these folders, authorized users can add their CAD files, PDFs, images, etc. 

An item based system is one where authorized users create an arbitrary container to hold their CAD files, PDFs, images, etc. This container is called, you guessed it, an Item. The data held in this container is what the user is able to search for when browsing for data.

## Personal Opinion Alert: Why Item Based Systems are Better
### Good Data Practice
To define a product, there is the 3D model which the designer is performing their work. In the current state of the world in engineering there are almost always additional datasets created that are representations of the 3D model file that the engineer creates. A typical engineers workflow could go something like so; (1) design a 3D model of a bolt, (2) make a drawing of the bolt using the 3D model, (3) create a PDF of the drawing, (4) save a .STEP file of the 3D model. In this scenario, we just created 4 different dataset formats that represent our bolt. Managing these 4 separate representaions of our bolt is an engineers nightmare. If we roll a revision on the model, how do we ensure that all our associated datasets are updated with the change? With an item based system, this task is much easier to automate when making revisions because the 4 separate datasets are defined in the item revision container. 

I would also add that engineers, by their nature, are creatures who are constantly attempting to maximize efficiency. The plight of the modern engineer is that the process of engineering requires far too many 'clicks'. Sending a single Item Revision through a workflow which holds the CAD file and its associated PDF reduces these clicks and keeps your data well managed. 

To play devils advocate, my opinion for holding these datasets in one revisionable unit falls apart if you are a business that is not concerned with keeping your CAD models up to date with the PDF or other associated dataset types you release to manufacturing. I will warn that this causes problems later when a revision needs to be made or a configuration is derived from your released PDF. This gets into the idea of your source-of-truth. It is possible that the released PDF will not match the CAD drawing which begs the question, is the PDF definition correct or the CAD file definition?
