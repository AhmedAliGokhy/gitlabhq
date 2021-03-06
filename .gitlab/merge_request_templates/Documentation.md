<!--See the general Documentation guidelines https://docs.gitlab.com/ee/development/documentation/index.html -->

## What does this MR do?

<!-- Briefly describe what this MR is about -->

## Related issues

<!-- Mention the issue(s) this MR closes or is related to -->

Closes 

## Moving docs to a new location?

Read the guidelines:
https://docs.gitlab.com/ee/development/documentation/#changing-document-location

- [ ] Make sure the old link is not removed and has its contents replaced with
      a link to the new location.
- [ ] Make sure internal links pointing to the document in question are not broken.
- [ ] Search and replace any links referring to the old docs in the GitLab Rails app,
      specifically under the `app/views/` and `ee/app/views` (for GitLab EE) directories.
- [ ] Make sure to add [`redirect_from`](https://docs.gitlab.com/ee/development/documentation/index.html#redirections-for-pages-with-disqus-comments)
      to the new document if there are any Disqus comments on the old document thread.
- [ ] If working on CE and the `ee-compat-check` jobs fails, [submit an MR to EE
      with the changes](https://docs.gitlab.com/ee/development/documentation/index.html#cherry-picking-from-ce-to-ee) as well.
- [ ] Ping one of the technical writers for review.

/label ~Documentation
