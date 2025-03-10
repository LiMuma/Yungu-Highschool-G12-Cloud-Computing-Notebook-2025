# Linux 命令基础笔记

## 命令基本语法

命令的基本格式：
```bash
命令名 [command] [options] [arguments]
```

- **命令名**：存在于PATH环境变量中的可执行命令
- **command**：从属命令
- **options**：
  - 单字母选项使用单个`-`（例如：`-a`，`-l`）
  - 单词选项使用双`--`（例如：`--help`）
- **arguments**：命令的参数

## 常用命令

### ls (List)
列出目录内容
- `ls` - 列出当前目录的文件和文件夹
- `ls -a` - 显示所有文件（包括隐藏文件）
- `ls -l` - 显示详细信息
- `ls -al` - 组合使用，显示所有文件的详细信息

### 帮助命令
获取命令帮助：
- `-h` 或 `--help` - 显示命令的简要帮助
- `man [命令名]` - 显示命令的详细手册页
  - 例如：`man ls`

## 文件权限管理

### 权限体系
文件权限格式：`rwxrwx-----`
- 第一组`rwx`：所有者权限
- 第二组`rwx`：用户组权限
- 第三组`---`：其他用户权限

其中：
- `r`：读权限
- `w`：写权限
- `x`：执行权限

### 权限管理命令
1. `chmod` - 修改文件权限
   - 示例：`chmod 755 file.txt`

2. `chown` - 修改文件所有者和用户组
   - 示例：`chown user:group file.txt`

## 注意事项
- 命令选项可以组合使用
- 大多数命令都支持`--help`选项来获取帮助信息
- 权限管理需要相应的权限级别