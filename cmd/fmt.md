# go fmt
## 描述

fmt 在导入路径命名的软件包上运行命令“gofmt -l -w”。它打印被修改的文件的名称。

有关 gofmt 的更多信息，请参阅“go doc cmd/gofmt”。
有关指定软件包的更多信息，请参阅“go help packages”。

-mod 标志的值设置要使用的模块下载模式：只读或供应商。
有关更多信息，请参阅“go help modules”。

要使用特定选项运行 gofmt，请运行 gofmt 本身。

## 选项

| Option | Effect                                 |
|--------|----------------------------------------|
| `-n`   | 打印要执行的命令                       |
| `-x`   | 在执行命令时打印命令                   |
| `-mod` | 设置要使用的模块下载模式：只读或供应商 |

## go help fmt

```shell
usage: go fmt [-n] [-x] [packages]

Fmt runs the command 'gofmt -l -w' on the packages named
by the import paths. It prints the names of the files that are modified.

For more about gofmt, see 'go doc cmd/gofmt'.
For more about specifying packages, see 'go help packages'.

The -n flag prints commands that would be executed.
The -x flag prints commands as they are executed.

The -mod flag's value sets which module download mode
to use: readonly or vendor. See 'go help modules' for more.

To run gofmt with specific options, run gofmt itself.

See also: go fix, go vet.
```
