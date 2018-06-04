# Simple commit style guide
This is a hyper-simple Git commit style guide created with the goal of simplifying but unifying commit messages in small-scale
projects.

## Branches
Branch names must not exceed 35 characters and must be formatted in a descriptive and readable manner in lowercase text, words should
be linked by dashes:
<br>``git checkout -b spanish-translation-header``✔
<br>``git checkout -b Span-head`` is incorrect.

## Commits
Commits must have simple descriptive lowercase summary starting with one of the below tags leading the text, 
All commits should contain only a single technical change group. Technical change groups can be as simple as adjusting the text and
color of a header or as complex as changing a core algorithm. 
<br><br>
Try to keep your commits as small and individual as possible for readability and reversion purposes.
<br>
``Summary: [new feature]Added a chat box to the core engine.``✔
### Tags
|[Tag]           |  Description | 
|----------------|-----|
|[bugfix]        |  Any bug fix or repair done in the form of actual code changes. |
|[new feature]   |  Addition of any new feature.|
|[cleanup]       |  Movement, reordering and reformatting of code. |
|[clerical]      |  Adjustments, fixes and changes in non-code text content. |
|[continuation]  |  Continuation of a new feature or bugfix. See proper syntax below. |
|[change]        |  Generic changes. |
#### Continuation syntax
``Summary: [continuation][bugfix]finalized #1327 fix.``✔

Tags do not count towards the total summary character count.
<br><br>
Tags must be entirely in lowercase.
<br><br>
Generic changes using the ``[change]`` tag may only be used in cases where another tag does not fit any other standard tags, and must include an extra in-depth description for review.

## Descriptions
Descriptions must be in-depth and cover all changes completed with a length of up to 720 characters total. Text may contain 
any ascii or unicode character or symbol so long as it does not distract from the descriptiveness.

## Pull requests
Pull requests must be titled with the general gist of all the changes with a description that covers any notes or additions
that are relevant.
