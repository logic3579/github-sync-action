[![GitHub To Gitee](https://img.shields.io/github/actions/workflow/status/yakir3/github-sync-action/sync2gitee.yml?label=GitHub%20To%20Gitee&logo=github&logoColor=white)](https://github.com/yakir3/github-sync-action/actions/workflows/sync2gitee.yml)

[![GitHub To GitLab](https://img.shields.io/github/actions/workflow/status/yakir3/github-sync-action/sync2gitlab.yml?label=GitHub%20To%20GitLab&logo=github&logoColor=white)](https://github.com/yakir3/github-sync-action/actions/workflows/sync2gitlab.yml)


```yaml
steps:
- name: Mirror the Github organization repos to Gitee.
  uses: yakir3/github-sync-gitee@main
  with:
    src: github/yakir3
    dst: gitee/yakir3
    dst_key: ${{ secrets.GITEE_PRIVATE_KEY }}
    dst_token: ${{ secrets.GITEE_TOKEN }}
    account_type: org
```

> Fork from: https://github.com/Yikun/hub-mirror-action
