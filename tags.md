# Tag Usage

Tags can be *lightweight* or *annotated*. The default on the command line
is a lightweight tag. However, these are not recommended as they are local
to a developer, not pushed to the GitHub or other server repository. The
SourceTree GUI, for example, creates *annotated* tags. You have to ask for
a lightweight tag, and the GUI marks that choice as *not recommended*.

## Tags and GitHub

GitHub creates *releases* for any tags you create. You can also create release notes
on the GitHub server for any releases. A tag of the form "v*version*" allows download
of a ZIP or tar-ball where the "v" is removed. For example, a project called *gorp*
might have a tag called *v1.0*. The ZIP download for the corresponding release will
be called *gorp-1.0.zip*, which will have a top-level directory called *gorp-1.0*.

Release notes are not defined by Git, nor are they part of the Git repository
maintained by GitHub.

## Tags and SourceTree

Tags are not automatically fetched from remote repositories. You can check the box
when fetching to retrieve tags from remotes as well as changes.
