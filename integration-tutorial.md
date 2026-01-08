### Integrating a Knowledge Base into a Workflow

Let's say you have a workflow that generates an article that mentions your in-development product, and you need a writeup of the product, approved for public media use.

Here's the example of how to use a Knowledge Base for that:

1. **Create or edit a workflow**. A detailed guide on how to do it can be found [in our Workflows documentation](https://profound-knowledge-base.help.usepylon.com/articles/2212787792-create-a-workflow).
2. **Add a Use Knowledge Base step**
   - In the workflow builder, add a "Use Knowledge Base" action directly before the "Generate Article" action (or any other action that you need information for)
   - Select which Knowledge Base to use
   - Enter your query: *"approved public description for public media"*
   - Label the output with a descriptive variable name: *Public Product writeup"*
3. **Reference the output**:
   - Later workflow steps can access your Knowledge Base step output by referencing the *Public Product writeup* variable
   - Use this information in your "Generate Article" step
   - Learn more about [using variables in Workflow steps](https://profound-knowledge-base.help.usepylon.com/articles/2212787792-create-a-workflow#use-variables-in-steps)