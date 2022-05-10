# dmp-template
## UKCEH DSW DMP Templates
One template per branch.

Use the ``test`` branch to test stuff out.  
Please make sure the template runs without error before pushing to this repository.

### Working method
1. **Clone** this respository to a local repository on your computer (one-off).
2. **Checkout** the branch (template) you want to start working on.
3. **Pull** this branch to make sure your local copy has all the latest changes.
4. Let others know if you are working on a template and actively uploading to DSW (only one person should work on a template at a time, working on a different template from a different branch is fine).
5. Make changes as required, committing locally as required.
6. When all changes for this session have been made, and the template runs without error, commit and **push to GitHub** so your changes can be used by the next person who edits this template.

#### Creating a new template
1. Create a new branch from the commit you want to base the template on, and make sure this new branch is checked out.
2. **Rename** the template file (e.g. ``src/nerc-dmp-template.html.j2``) to a suitable name for the new template.
3. Edit the following fields in **template.json**:

    templateID  
    version  
    name  
    description

4. Edit the line referencing the template file in ``src/index.html.j2``, changing to the name of the new template file.

    e.g. ``{% include "src/nerc-dmp-template.html.j2" with context %}``
    
5. Make any changes to the template, **commit** and **push** to a new branch of the same name on GitHub.

**Note we can change any of this working method at any time, ensuring this readme file is kept up-to-date with any changes.**
