# - 你就先ssh到云服务器, 再ssh -p 1222 localhost, http://blog.suexcxine.win/2018/09/13/nat_expose/, https://meaninglive.com/2021/05/14/%E4%BD%BF%E7%94%A8autossh%E5%AE%9E%E7%8E%B0%E5%8F%8D%E5%90%91ssh%E9%9A%A7%E9%81%93/
# 使用frp的一些心得记录
中转服务器可能会有两层防火墙，有的时候防火墙需要全部关闭，协议为kcp时，udp的相关防火墙也要关闭。端口转发就用tcp就行，本地的ip多试试127.0.0.1以及本地机器的内网ip，比如192啥的。不同的协议不能占用同一个端口，比如http与tcp，其实是不同的隧道。frp总的来说，非常好用，配置简洁可读，操作傻瓜式。速度快。
