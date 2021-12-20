# go mod
## 描述

Go mod 提供对模块操作的访问。

请注意，对所有 go 命令都内置了对模块的支持，而不仅仅是“go mod”。
例如，依赖项的日常添加、删除、升级和降级应该使用“go get”完成。
有关模块功能的概述，请参阅“去帮助模块”。

## 选项
| Option | Effect                   |
|--------|--------------------------|
| `init` | 在当前目录中初始化新模块 |

## go help mod

```shell
Go mod provides access to operations on modules.

Note that support for modules is built into all the go commands,
not just 'go mod'. For example, day-to-day adding, removing, upgrading,
and downgrading of dependencies should be done using 'go get'.
See 'go help modules' for an overview of module functionality.

Usage:

	go mod <command> [arguments]

The commands are:

	download    download modules to local cache
	edit        edit go.mod from tools or scripts
	graph       print module requirement graph
	init        initialize new module in current directory
	tidy        add missing and remove unused modules
	vendor      make vendored copy of dependencies
	verify      verify dependencies have expected content
	why         explain why packages or modules are needed

Use "go help mod <command>" for more information about a command.
```

## output

ubuntu@VM-12-14-ubuntu:~/go/src/GoWebP$ go mod init
go: creating new go.mod: module GoWebP
go: to add module requirements and sums:
        go mod tidy
