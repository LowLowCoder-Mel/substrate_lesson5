# ink 笔记

- ink 也是用 Rust and Wasm 底层技术栈
- ink 合约架构 
    - #[ink(storage)]     存储
    - #[ink(constructor)] 合约实例化
    - #[ink(message)]     用户可调用的Method
    - #[ink(event)]       合约反馈的Event

- 整个合约包裹在 `#[ink::contract] mod` 里面

- 合约的 `message` 和 `constructor` 在 合约的 `impl` 里面实现 

- 合约的公共方法，一共有两种
  读, 写 (这里会有一些转账，或者修改)