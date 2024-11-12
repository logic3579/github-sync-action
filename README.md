[![GitHub Actions](https://img.shields.io/github/actions/workflow/status/yakir3/github2gitee-action/sync2gitee.yml?label=GitHub%20Actions&logo=github&logoColor=white)](https://github.com/yakir3/github2gitee-action/actions)

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
