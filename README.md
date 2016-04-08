# NetWorkFromAsyncSocket

用法
通过宏定义：
#define SOCKET [NetWork sharedInstance]

连接网络
[SOCKET connectToHost:host Port:port withTimeout:timeout];

发送数据
[SOCKET sendOutData:string withTag:tag];

断开连接
[SOCKET cutOffSocket];

查看本地Ip和Port
NSDictionary *hostAndPort ＝ [SOCKET localHostAndPort];
NSString *host = [hostAndPort valueForKey:LocalHost];
NSString *port = [hostAndPort valueForKey:LocalPort];


