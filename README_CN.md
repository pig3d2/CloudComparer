# CloudComparer 使用说明

## 📝 如何修改云服务对比数据

### 文件位置
```
_data/cloudservices.yml
```

### 修改方法

直接用文本编辑器（VS Code、Sublime Text 等）打开上述文件，按照现有格式添加或修改数据。

### YAML 格式示例

```yaml
- category: Compute
  subcategory: Virtual Server
  service:
    - aws:
        - name: EC2
          ref: https://aws.amazon.com/ec2/
          icon: ec2.png
    - tencent:
        - name: CVM (Cloud Virtual Machine)
          ref: https://www.tencentcloud.com/products/cvm
          icon: cvm.png
```

## 🌐 查看效果

### 在线版本（推荐）
访问：https://ilyas-it83.github.io/CloudComparer/

修改后提交到 GitHub，几分钟后自动更新。

### 本地预览（需要环境配置）

由于本地环境配置复杂，建议使用以下方式之一：

1. **GitHub Codespaces**（推荐）
   - 在 GitHub 仓库页面点击 "Code" → "Codespaces"
   - 创建新的 Codespace
   - 自动配置好所有环境
   - 在浏览器中预览

2. **Docker**（如果已安装）
   ```bash
   docker run --rm -it \
     -p 4000:4000 \
     -v "$PWD:/srv/jekyll" \
     jekyll/jekyll:4.2.0 \
     jekyll serve --watch --force_polling --host 0.0.0.0
   ```

3. **Ruby 3.x + Jekyll**（需要配置环境）
   ```bash
   brew install ruby
   export PATH="/opt/homebrew/opt/ruby/bin:$PATH"
   gem install bundler jekyll
   bundle install
   bundle exec jekyll serve
   ```

## 💡 建议

**最简单的工作流程**：

1. 本地修改 `_data/cloudservices.yml`
2. 提交到 GitHub
3. 访问在线版本查看效果

**不需要本地预览！**

## 📞 需要帮助？

查看项目原始 README：`README.md`
