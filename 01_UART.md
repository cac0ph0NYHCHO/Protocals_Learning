# UART（Universal Asynchronous Receiver/Transmitter）通用异步收发器
- 口头上叫“串口”
- 串行
- 异步
- 全双工
## UART数据帧格式
<img width="1094" height="424" alt="image" src="https://github.com/user-attachments/assets/2bf71a4d-54b7-4eba-a6c8-bf67ae50b98a" />

- 空闲位：空闲状态维持高电平
- 起始位：由空闲位的1变为0
- 数据位：先发低位再发高位
- 校验位：常用奇偶校验
- 停止位：表示通信结束
- 通过波特率判断发送了1个0还是2个0
- 一次只能发一个字节去消除累计误差（发送方和接收方时钟不同步的问题）
## UART硬件连接
<img width="781" height="424" alt="image" src="https://github.com/user-attachments/assets/b1adbd71-8a5a-427f-929a-961a90b4412d" />

- TXD（Transmit Data）数据输出引脚
- RXD（Receive Data） 数据输入引脚
