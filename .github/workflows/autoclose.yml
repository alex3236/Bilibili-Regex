name: Autocloser
on: [issues]
jobs:
  autoclose:
    runs-on: ubuntu-latest
    steps:
    - name: Autoclose issues that did not follow issue template
      uses: roots/issue-closer@v1.1
      with:
        repo-token: ${{ secrets.GITHUB_TOKEN }}
        issue-close-message: "@${issue.user.login} 似乎您没有阅读并确认表达式条件。此 Issue 自动关闭。"
        issue-pattern: ".*guidelines for Contributing.*"