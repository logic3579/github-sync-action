Fork from: https://github.com/Yikun/hub-mirror-action

```yaml
steps:
- name: Mirror the Github organization repos to Gitee.
  #uses: yakir3/github-sync-gitee@master
  uses: Yikun/hub-mirror-action@master
  with:
    src: github/yakir3
    dst: gitee/yakir3
    dst_key: ${{ secrets.GITEE_PRIVATE_KEY }}
    dst_token: ${{ secrets.GITEE_TOKEN }}
    account_type: org
```
