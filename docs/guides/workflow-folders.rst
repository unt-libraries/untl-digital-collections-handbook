######################
Folder-based Workflows
######################

************
Introduction
************

One of the challenges in starting a digital project is how to organize the work. This is important for both born-digital projects as well as digitization projects. While many projects will follow the same workflow patterns, they will often deviate slightly depending on the specific project requirements. 

Designing a workflow system that works for small and large projects that doesn't also add too much overhead is something that many insitutions continue to struggle with in the digital libraries space.  There are commercial and open source projects that have been developed to solve these problems. We've found that a simple folder-based workflow works for many types of projects from small to large and helps workers and managers to quickly tell the status of a project, and what needs to be worked on. 

This guide will help to introduce the concept of the folder-based workflows used at the UNT Libraries and provide some examples of how they are being used in existing projects. 


The section is an example folder-based workflow ::

  Project-Workflow/
  ├── 0.toScan
  ├── 1.Scanning
  ├── 2.ToQualityCheck
  ├── 3.Issues
  ├── 4.ToOCR
  ├── 5.ToMetadata
  ├── 6.ToUpload
  ├── 7.Uploading
  └── 8.Uploaded

********************************
What are Folder-based Workflows?
********************************

The basic idea of a folder-based workflow is that each project has a folder created for it on a shared network drive. Each step in the workflow is used as a folder name. Objects within each folder are at that step within the workflow. This ensures that every step in the workflow is known and accounted for. This can be tailored to each project, and we use this workflow for submissions to UNT Scholarly Works.

For each project, the workflow will be contained within its own folder. Even if the project is relatively small, for example digitizing four maps, it will receive its own workflow folder. This folder may be named something like “scanned_from_ohs” for a project that had digital materials originating at another institution. All of the files that are important to this project are stored in this folder structure. The folder names are based on local naming conventions.

The workflow is essentially an ordered sequence of folders that define the steps in a workflow. For example, there is often the process of applying Optical Character Recognition (OCR) to a set of scanned items. This step usually happens after other steps have been completed, like scanning the documents and performing quality control checks on the images. After OCR has been completed, we then need to create descriptive metadata and can stage the content for uploading to the digital library system. In the rough workflow just outlined, there might be one or more people involved in moving digitized items through a workflow.

To facilitate this we have outlined a workflow that looks like this. ::

    scanned_from_ohs

    0.Staging/
    1.Scanning/
    2.ToQC/
    3.Issues/
    4.ToOCR/
    5.ToMetadata/
    6.ToUpload/
    7.Uploading/
    8.Uploaded/
    
While the steps are somewhat arbitrary and are aligned with workflows at the UNT Libraries, a description of the steps is helpful to understand how items move through the workflow. Before we do that, it is helpful for us to establish a few guiding principles of these workflows.

1. Only move content when you are ready for someone else to take it as part of the following step.
2. Keep folders as shallow as you can.
3. The location of an object in the folder structure should reflect the work that needs to be done to the object.
   Adjust the folder order and name to reflect the workflow.
4. With these guiding principles in place, we can talk about how content moves through a workflow.


First off, in the 0.Staging folder, we can begin to sort items that need to be digitized. In many cases, we can create directories that will act as containers for digital objects as they move through the process. We have found that representing a digital object as a folder and naming it with the unique identifier for the item is helpful. Then, all files related to that object are placed inside this object’s folder. Moving an object between steps in the workflow is now just moving a folder. By keeping the folder structure shallow with ideally just one level of hierarchy, the object folders can easily be moved around within the workflow folders making it easy to see how items are distributed throughout the workflow.

The next step in this workflow is called 1.Scanning. As an example, we will be digitizing a journal for a historical society. As a technician is digitizing the item, they can place working files into this workflow step’s folder. Once they have completed the initial quality control check, they will move the object folder to the next step’s folder in the workflow called 2.ToQC. In this step, another round of quality control is performed by another person in the unit. As this step is being completed, if there are any issues, such as missing pages or images that need to be rescanned, the person completing the quality control can move this object folder to the 3.Issues folder. If there are no problems, they can move the object folder to the 4.ToOCR folder in the workflow. At this step in the workflow, the person responsible for OCRing items will take items from this workflow folder and process them with an OCR engine. After that has completed, the object folder is moved to the 5.ToMetadata folder, where they will have descriptive metadata created for them. This step may involve full-record metadata creation or could involve the creation of basic metadata that will be updated and completed later when it is loaded into the system. After this metadata has been generated, the object folder is moved to the 6.ToUpload folder. The final three steps in this workflow outline the ingest activities of the UNT Digital Library where content is staged for upload and finally ingested into both the access repository, Aubrey, and the preservation repository, Coda. During this ingest period, the object folder is moved into the 7.Uploading folder to indicate that it is being uploaded to the system. Once verification of upload has taken place, the object folder is moved to the final folder, 8.Uploaded. At some point in the future when the project has completed, the files in the object folder are deleted to recover network space.

********
Examples
********

Newspaper Digitization Workflow
===============================

Born-Digital Workflow
=====================

Simple Vendor Digitized Workflow
================================

**********
Discussion
**********

Folder-Based Workflow Discussion
With the overview of the folder workflow complete, there are some things to discuss. This is a very simple way of organizing projects. At UNT this method allows us to have multiple people working on a single project at different times and it is clear what is happening along the workflow with a given digital object because of its location. It is important for all participants in the project to remember to only move items into a subsequent folder when they are ready for someone else to take that object and process it further. If an object hasn’t finished the step that its location in the workflow folder designates, it shouldn’t be moved. This important rule allows for different team members to work independently and confidently within the workflows.

Because we try to keep the folder structures as shallow as possible, ideally with only one level of folders representing objects in each of the workflow folders, it is easy to see how much content is waiting in what steps for a project. Simply browsing the folder structure gives an overview of where things are in the workflow. We have found that it is important to keep objects at a single level within the workflow folders. As folders become more deeply nested or contain multiple other folders, it becomes harder to understand the progress of the overall workflow or tell when objects are incomplete.

Because workflows can differ depending on the type of project, type of content, or because of unique requirements, it is important for the folder names to be descriptive about the step in the workflow that it represents. The number preceding the step is important to define the sequence of the steps, but the name of the step in the folder’s name should be clear to make the step understood by others involved in the project.

Finally, if we start a project and discover that the initial folder structure doesn’t meet the needs of the project, we change the structure to meet the needs. This is helpful because there are often many projects and a variety of types of projects being worked on at any given time. In order to keep track of what is happening within a specific project, it is important to make sure the folder structure matches the workflow.

While the folder-based workflow is not a particularly complicated management structure for projects, it has served its purpose well over the years.


***************
Further Reading
***************

Johnson-Freeman, W., Phillips, M. E., Phillips, K. K. (2021) *Managing an institutional repository workflow with GitLab and a folder-based deposit system* Code4Lib Journal <https://journal.code4lib.org/issues/issues/issue50>_ 
