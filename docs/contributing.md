# Contributing

Interested in contributing to the Cloud Engineering Documentation? Want to report a bug? Before
you do, please read the following guidelines.

## Submission context

### Got a question or problem?

For quick questions there's no need to open an issue as you can reach us on
[mattermost][1].

  [1]: https://mattermost.dunnhumby.com/default/channels/cloud-engineers

### Found a mistake in the documentation?

If you found a bug in the documentation, you can help us by submitting an issue
to the [issue tracker][2] in our GitLab Project. Even better, you can submit
a Merge Request with a fix. However, before doing so, please read the
[submission guidelines][3].

  [2]: https://jira.dunnhumby.co.uk
  [3]: #submission-guidelines

## Submission guidelines

### Submitting an issue

Before you submit an issue, please search the issue tracker, maybe an issue for
your problem already exists and the discussion might inform you of workarounds
readily available.

That said, the preffered method of fixing the documentation is to submit a merge request
with the corrected docmentation. If everyone gets into the habbit of just raising issues
and not addressing them, then the responsibility for maintaining the documentation will
fall to a small number of people, and ultimately become stale...

### Submitting a Merge Request (MR)

Search GitLab for an open or closed PR that relates to your submission. You
don't want to duplicate effort. If you do not find a related issue or PR,
go ahead.

1. **Development**: Fork the project. At this point you can either set up 
  the [development environment][4], or just edit the site in gitlab. The CI process 
  will automatically attempt to rebuild your site on commit (but not publish the changes).
  Please make your changes in a separate git branch and add descriptive messages to
  your commits. Use the naming convention `USER/descriptive-branch-name` for your branch.

2. **Build**: Before submitting a merge requests, build the site. This is a
  mandatory requirement for your MR to get accepted, as the site should successfully
  build, it should also pass the build in the CI pipeline.

3. **Merge Request**: After building the site successfully you can commit the source to GitLab. 
  Push your branch to GitLab and send a MR to `cloud-engineering/docs:master`. If we
  suggest changes, make the required updates, rebase your branch and push the
  changes to your GitLab repository, which will automatically update your MR.

After your MR is merged, you can safely delete your branch.

  [4]: http://localhost:8000/customization/#theme-development
