---
name: Retry a workflow
example: octokit.rest.actions.retryWorkflow({ owner, repo, run_id })
route: POST /repos/{owner}/{repo}/actions/runs/{run_id}/retry
scope: actions
type: API method
---

# Retry a workflow

Retry your workflow run using its `id`. You must authenticate using an access token with the `repo` scope to use this endpoint. GitHub Apps must have the `actions:write` permission to use this endpoint.

```js
octokit.rest.actions.retryWorkflow({
  owner,
  repo,
  run_id,
});
```

## Parameters

<table>
  <thead>
    <tr>
      <th>name</th>
      <th>required</th>
      <th>description</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>owner</td><td>yes</td><td>

</td></tr>
<tr><td>repo</td><td>yes</td><td>

</td></tr>
<tr><td>run_id</td><td>yes</td><td>

The id of the workflow run.

</td></tr>
  </tbody>
</table>

See also: [GitHub Developer Guide documentation](https://docs.github.com/rest/reference/actions#retry-a-workflow).