# 请注意：
1. 如果你是新生且仅使用统一身份认证，并未设置教务系统密码，请修改脚本使用PHP SESSIONID。
2. 目前我们注意到如果在未修改默认账号密码的情况下使用默认账号密码登录，你的账号可能会被安全锁定。
3. 如果你的教务账号已经被锁定，你可以找你辅导员重设你的密码。

# fvti_enrollment
福州职业技术学院教务系统 公共选修课抢课辅助程序

开放源代码仅供学习和交流使用，禁止商用！

问题反馈：titusyu@acm.org

基于 Python3，依赖 requests 模块。

1. 环境依赖安装完成后，连接校园网。
2. 修改.py文件中的账号密码为要抢课的教务系统学号和密码
3. 运行并等待脚本请求验证码，程序会自动尝试打开二维码。
  （如果没打开的话手动打开一下哈）

4. 查看并输入验证码，回车后等待脚本向教务请求登入
5. 然后在脚本列出课程序号和课程列表后，输入要抢的课程的序列号即可开抢
6. 等待教务系统返回提交的结果，如果看到 code 的值为 1 则说明抢课提交成功
