# Managing Knowledge Bases

## Organizing content with folders and files

### Adding folders and files

1. Select a Knowledge Base from the list, click on its name.
![A screenshot of the Knowledge Bases list in the Profound Workspace Brand Hub, with an arrow pointing to the Company General Knowledge Base](./assets/KB3.jpg)

2. Click **Add Folder** to create a new folder.
3. Click **Add Files** to upload documents directly.
![A screenshot of the top of the File Overview table in the Company General Knowledge Base with arrows pointing to "Add Folder" and "Add Files" buttons](./assets/KB3-1.jpeg)

Supported file types include PDF, DOCX, TXT, and other common file formats.

### Managing files

#### File Overview table

In the File Overview table, you can see the following data:

- **Name**: Folder or file name
- **Last Sync**: When content was last updated
- **Details**: Number of files in folders or tags for individual files
- **Size**: Storage space used
- **Actions**: Download or manage individual items

![A screenshot of the File Overview table in the Company General Knowledge Base with sample files and folders](./assets/KB3-1.jpeg)

#### File tagging

Files can be assigned tags to help with categorization and search.

![A screenshot of the files in the File Overview table with arrows pointed at file tags](./assets/KB3-3.jpeg)

When you sync your Knowledge Base, some tags are added to your existing files automatically based on the file content. You can edit or add tags by clicking on the individual files and following the prompts.

When adding custom tags, make sure to use clear, descriptive tag names (e.g., "Onboarding", "Guide", "HR", etc.) for the best results.

Multiple tags can be added to the same file, and multiple files can have the same tags.

### Understanding storage limits

Based on your Profound plan, your workspace includes a certain amount of storage for Knowledge Bases. The default storage allocation on a Starter plan is 10GB. If you need more, you can talk to your sales representative or contact our sales team using [the contact form](https://www.tryprofound.com/contact-sales) to explore your options.

You can keep track of your storage usage in the **Brand Hub > Knowledge Bases** tab, where it is displayed (e.g., 3.7GB/10GB Used) just above the Knowledge Bases list:

![A screenshot of the Knowledge Bases list in the Profound Workspace Brand Hub, with the storage usage displayed and highlighted](./assets/KB2-1.jpg)

## Searching your Knowledge Base

The Knowledge Base Search Test feature lets you query your content before using it in Workflows, helping you verify that relevant information is indexed correctly.

![A screenshot of the File Overview table page in Company General Knowledge Base with arrows pointed at the Knowledge Base Search Test component](./assets/KB4.jpg)

### Running a search

1. Open any Knowledge Base.
2. In the **Knowledge Base Search Test** section, enter your query.
3. Click **Run Search** or press Enter.
4. Click **Advanced Settings** to refine your search parameters if needed.
5. Review results ranked by relevance.

### Understanding search results

Search results are organized by match quality.

![A screenshot of the sample Search Test search results](./assets/KB4-2.jpg)

**High Match** results directly answer your query, while **Medium Match** results are partially relevant, and **Low Match** results are only loosely related to your search terms.

Each result includes a source document name and folder, relevant text excerpt with the page number, as well as a "Show more" option to view extended context. To view the entire document that includes your search term, click on the document file name.

<img src="./assets/KB4-3.jpg" height="115px" alt="A screenshot of a search result with an arrow pointed at the clickable filename">

>[!TIP]
>Be specific in your search queries: "LinkedIn product description guidelines" returns better results than "social media". Try a few different phrasings to see which ones yield the best results.

### What are chunks?

When you upload files to a Knowledge Base, Profound automatically processes them into chunks.

<img src="./assets/KB3-4.jpeg" height="70px" alt="A screenshot of a Knowledge Base page with the amount of files and chunks displayed, the amount of chunks underlined">

**Chunks** are small segments of meaningful text within a file. For example, a 50-page product documentation PDF might be broken into 200 chunks, with each chunk containing a specific section like a feature description, pricing table, or integration guide.

Chunking is what allows the Knowledge Base search results to point to the exact relevant piece of text rather than an entire document, making it faster to find specific information.

## Using Knowledge Base content in Workflows

Knowledge Bases integrate seamlessly with Profound's Workflows, allowing you to automatically incorporate company information into AI-generated content.

Here's how to reference your Knowledge Base in a content creation Workflow:

1. **Create or edit a Workflow**. A detailed guide on how to do this can be found [in our Workflows documentation](https://profound-knowledge-base.help.usepylon.com/articles/2212787792-create-a-Workflow).
2. **Add a Use Knowledge Base step**:
   - In the Workflow Editor, add a **Use Knowledge Base** action before the actions that you need the information for
   - Select which Knowledge Base to use
   - Enter your query
   - Label the output with a descriptive variable name
3. **Reference the output** in the later Workflow steps by referencing its output variable name

>[!TIP]
> For a more detailed example of how to integrate your Knowledge Base into a Workflow, check out our [Integrating a Knowledge Base into a Workflow tutorial](../integration-tutorial.md)

## Next steps

- Learn [best practices for structuring your Knowledge Base](./best-practices.md)
- Follow the [integration tutorial](../integration-tutorial.md) to integrate a Knowledge Base into a Workflow
- Visit the [FAQ & Troubleshooting](../faq-troubleshooting.md) section
