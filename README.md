# AlgorithmXcframework

算法二进制存储仓库

# 操作

1. 首先到源码仓库去把 Rust 算法打包

```sh
cargo build --target aarch64-apple-ios --release
cargo build --target aarch64-apple-ios-sim --release
cargo build --features spm --release
```

2. 把打包好后的 xframework 压缩成 zip 文件

3. 把 xframework.zip 文件传到当前仓库的 release

4. 把 Swift SPM 包的版本及引用二进制地址改成当前仓库的 release 二进制地址
