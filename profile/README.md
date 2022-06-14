## Hi 看看工作流程 👋

主分支是 `develop`，线上分支为 `main`.

## 如何开始工作
1. 先将 repo `fork` 到自己账号下
2. 然后开新分支进行开发
3. 开发完毕后 push 到自己的 repo
4. 到 GitHub 提交 `Pull Request`，打上对应的 `label`，然后 request 对应的同事 review

### Commit 格式
can
提交信息首行简要描述该提交涉及的改动，建议以动词开头。如需添加相关 `issue` ，须与首行之间保留一个空行，从第三行开始。可参考以下格式：
```log
第一行 [<type>:] 简要描述该提交涉及的改动，建议以开头动词 [(<scope>)]
第二行 空行
第三行 相关的链接（issue 或 jira 等）
第四行 更多必要信息
```
type（可选）:
```log
feat: 新功能
fix: 修复问题
docs: 添加或者修改文档
test: 添加或者测试用例
refactor: 重构（既不涉及新功能，也不是修复问题）
chore: 构建工具或者辅助工具的变动
style: 调整格式
```
scope（可选）:
 比如fix涉及的范围 组件名、文件名等等逗号分隔

例子：
```log
Integrate immutable.js (A,B,C)

https://trello.com/c/yIglLjvq
```

```shell
# add it to profile(如：~/.zshrc)
alias gclc='git commit -v --reset-author -c `git log --pretty=%H -n1`'
```
使用 [Commitizen](https://github.com/commitizen/cz-cli) 来帮你写 commit message
