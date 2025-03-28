# Linux的文件权限与目录配置

> 在Linux中，一切皆文件（Everything is a file）

## 重要目录说明

| 目录 | 说明 |
|:-----|:-----|
| `/bin` | 存放单人维护模式下可用的基本命令，所有用户（包括root和普通用户）都可以使用 |
| `/boot` | 存放系统启动相关文件，包括Linux内核文件、开机菜单和配置文件 |
| `/dev` | 设备文件目录，所有硬件设备都以文件形式存在于此，例如：`/dev/null`（空设备） |
| `/etc` | 系统配置文件目录，存放用户账号密码文件和各种服务的启动配置 |
| `/root` | 系统管理员（root）的主目录，位于根目录下，便于单人维护模式使用 |
| `/usr/local` | 系统管理员在本机自行安装的软件目录，建议将自行下载安装的软件放在此处 |
| `/usr/sbin` | 非系统正常运行所需的系统指令目录，通常包含网络服务器等服务的命令 |
| `/usr/bin` | 所有普通用户可用的命令目录 |
| `/media` | 可移动设备挂载点，例如：`/media/cdrom`、`/media/floppy` |
| `/lib` | 系统启动时需要的函数库，为`/bin`和`/sbin`下的命令提供支持 |
| `/opt` | 第三方软件安装目录，用于存放独立的软件包 |
| `/tmp` | 临时文件目录，所有用户都可以访问，用于存放程序运行时的临时文件 |
| `/home` | 用户主目录，新建用户时默认创建在此<br/>`~` 表示当前用户主目录<br/>`~用户名` 表示指定用户的主目录 |
| `/lib<qual>` | 特定格式的函数库目录，例如：`/lib64`用于64位系统 |

## 文件系统结构图
![Linux文件系统结构](https://github.com/LiMuma/Yungu-Highschool-G12-Cloud-Computing-Notebook-2025/blob/main/Image/DD6808A1-CB3B-4EF7-A28E-94855C52D75D.png?raw=true)
