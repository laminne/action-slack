---
title: Next Action
metaTitle: Next Action | action-slack
metaDescription: This explains the next action-slack move.
---

# Selectable Field

Currently the field is fixed, but I want to make it selectable.  
It is assumed that the input is in csv format.

```yaml
steps:
  - uses: 8398a7/action-slack@v3
    with:
      status: ${{ job.status }}
      fields: repo,message,action,author
    env:
      GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }} # optional
      SLACK_WEBHOOK_URL: ${{ secrets.SLACK_WEBHOOK_URL }} # required
```
