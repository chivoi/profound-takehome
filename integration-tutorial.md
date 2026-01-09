# Integrating a Knowledge Base into a Workflow

This is an Integration tutorial on how to integrate an information from a Knowledge Base to a Workflow

## Scenario: Creating a blog post mentioning your new feature

Let's say you are a member of a fintech startup marketing team, and you want to create a "Top 10 Expense Management Features" blog post listicle that includes your newly launched automated receipt scanning feature. The feature is scheduled to launch soon, but you are not sure how much information has been publicly announced about it, and using the non-approved (let alone AI-hallucinated) information can harm the release.

## Solution

This is a perfect use case for the "Use Knowledge Base" workflow step that can retrieve the approved product writeup from your official company Knowledge Base, and incorporate it into your blog post.

Here is how to use it:

### I.Create/edit a content generation workflow

A detailed guide on Workflow creation, including configuring inputs, adding steps, using variables, etc. can be found in our [Workflows documentation](https://profound-knowledge-base.help.usepylon.com/articles/2212787792-create-a-workflow).

Some suggested Workflow steps for a content generation workflow will be:

- **Use Brand Kit** to get the information about your brand's competitors, customers profile, as well as the tone of voice and writing style for later steps;
- **Prompt LLM / Perplexity Search** to research the most popular expense management products from competitors, your potential customers pain points, etc.;
- **Article Title Suggestion** to generate an AEO-optimized article title
- **Generate Article** to generate your article content using the information gathered in the previous steps

>[!TIP]
>Many of the above steps will require you to write prompts. Check out our guide on [How to Write Great Prompts](https://profound-knowledge-base.help.usepylon.com/articles/5556357652-how-to-write-great-prompts) for Workflows.

### II. Add a Use Knowledge Base step

1. In the workflow builder, click "+" directly before the "Generate Article" action, search for a "Use Knowledge Base" action, click on it to add it to the flow

2. Select the Knowledge Base you would like to reference from the list of your available Knowledge Bases (e.g., "Marketing Content Library")

3. Enter your query, for example *"public announcement automated receipt scanning feature"*

4. Label the output with a descriptive variable name, like *"Receipt Scanning Public Info"*

### III. Reference the output

After you save the Use Knowledge Base step, the result of your query will be available to all subsequent Workflow steps.

Use the *"Receipt Scanning Public Info"* variable to access it in the input fields of the "Generate Article" step by selecting a field and clicking an **“(x) Add variable”** icon.

>[!TIP]
>Learn more about [using variables in Workflow steps](https://profound-knowledge-base.help.usepylon.com/articles/2212787792-create-a-workflow#use-variables-in-steps)

## Result

After incorporating the approved Receipt Scanning feature writeup into your blog post, you have a comprehensive quality listicle that includes only relevant and correct information about the feature!

## Tips for effective integration

- **Query strategically**: "Short product description for LinkedIn" returns more relevant results than "product info"
- **Combine sources**: Use multiple Knowledge Bases in the same workflow (e.g., product docs + brand guidelines)
- **Review the content**: Always review AI-generated content that references your Knowledge Base to ensure it's appropriate
- **Test your queries**: Use the Knowledge Base Search Test feature to refine queries before adding them to workflows

## Next steps

Now that you understand how to integrate Knowledge Bases into workflows, one thing left to do is to try it out!

- Head to the Worflows section in the left side menu of your Profound dashboard and have a go at putting together a simple flow with the Use Knowledge Base step.
- Overwhelmed with options? Use the templates in the **Popular Templates** section to get you started
- Still not quite comfortable with Workflows? Head to the [Workflow documentation](https://profound-knowledge-base.help.usepylon.com/collections/1956844252-workflows) section to learn more.
