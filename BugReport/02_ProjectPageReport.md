
## Summary (Summarize the bug encountered concisely)
    Typo within the "Create blank project" element on the project creation page. 
    Reads "Create black project" instead of "Create blank project"
    "black" is the typo.


## Steps to reproduce     
    Ensure you've logged into GitLab
    Ensure you are on the Main Page
    Click on "New Project"
    Once on the "Create new Project" -screen, pay attention to top-left element creation element.
   

## What is the current bug behavior?
    The top-left element's title is "Create black element"
     

## What is the expected correct behavior?
    The top-left element's title should be "Create blank element"

     
## Relevant logs and/or screenshots

    Relevant line of HTML. Typo highlighted with !!!! [typo] !!!!

    ```
        <div class="new-namespace-panel-wrapper gl-float-left gl-mb-5 gl-inline-block gl-px-3">
            <a href="#blank_project" data-testid="panel-link" data-qa-panel-name="blank_project" class="new-namespace-panel gl-flex gl-w-full gl-shrink-0 gl-flex-col gl-items-center gl-rounded-base gl-border-1 gl-border-solid gl-border-gray-100 gl-px-3 gl-py-6 hover:!gl-no-underline lg:gl-flex-row"><div class="new-namespace-panel-illustration gl-flex gl-shrink-0 gl-justify-center"><img aria-hidden="" src="/assets/webpack/project-create-new-sm.d02514e7.svg"></div> <div class="gl-pl-4">
            <h3 class="gl-text-size-h2 gl-text-inherit">
                 Create !!!! black !!!! project
            </h3>  
            <p class="gl-text-default">
            Create a blank project to store your files, plan your work, and collaborate on code, among other things.
            </p>
            </div>
            </a>
        </div>
    ```
      

## Possible fixes
    Change "Create black project" back to "Create blank project"

    ```
        <h3 class="gl-text-size-h2 gl-text-inherit">
             Create !!!! black !!!! project 
        </h3>
    ```  
## Whom do you report/ Assign To/ Tags
      /label ~bug ~reproduced ~needs-investigation 
      /cc @project-manager 
      /assign @developer


## Priority
    Minor

    

      
