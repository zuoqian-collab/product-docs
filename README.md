# Product Docs

团队产品需求文档（PRD）仓库

## 目录结构

```
product-docs/
├── prds/           # 产品需求文档
├── templates/      # PRD 模板
└── README.md       # 本文件
```

## 使用方式

### 作为 Git Submodule 链接到代码仓库

在代码仓库中执行：

```bash
git submodule add <product-docs-repo-url> docs/product-docs
```

### 编写 PRD

1. 复制 `templates/prd-template.md` 到 `prds/` 目录
2. 按照日期或功能命名，例如：`prds/2026-01-user-login.md`
3. 填写文档内容
4. 提交到 git

### 查看产品变更历史

```bash
# 查看文档变更记录
git log --oneline prds/

# 查看某个文档的演进历史
git log -p prds/2026-01-user-login.md
```

