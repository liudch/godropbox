http://www.oschina.net/news/53407/dropbox-opensource-go-lib
Dropbox的成功大部分归功于Python，这个语言可以使我们快速迭代开发。然而，为了支持日益增长的用户量，我们的基础设施日渐成熟，这时 我们开始寻找一种更为高效的方式来改变系统规模。大约在一年前，我们作出决定，把对于性能要求很苛刻的后台部分从Python迁移到了Go语言，以提供更 好的并发支持和更快的运行速度。一个规模很小的工程师团队做出了大量的努力，这背后大约是200,000（二十万）行Go语言代码。此时，我们成功地把架 构的大部分迁移到了Go语言。

缺少构建大型系统的健壮的程序库，已经成为了反复出现阻碍我们开发进度的问题。这并不奇怪，因为Go语言还是一门十分年轻的语言。为了处理这个问 题，我们的团队开始构建各种各样的库，已提供更好的封装抽象，例如连接管理和MenCache客户端。我们非常兴奋的宣布我们开源了这些库，帮助更广大的 社区开发大型的产品系统。

作为这项努力的开端，我们包含了许多库。下面列举几个：

caching ：提供建立caching层的通用抽象。
errors ：强化了标准错误接口并且揭示出栈跟踪的信息
database/sqlbuilder : 允许开发者用可编程的方式生成sql语句。
memcache ： 实现了一个全特性的memcache客户端库，支持连接池和灵活的 shading 。
net2 : 连接管理中加入了函数性功能。
（还有我个人最喜欢的，hash2，它包含了一个空间效率高，基于排列的连续哈希算法）
# godropbox [![GoDoc](https://godoc.org/github.com/dropbox/godropbox?status.png)](https://godoc.org/github.com/dropbox/godropbox)

Common libraries for writing go services/applications.

### Installation
``go get github.com/dropbox/godropbox``

### Documentation

See https://godoc.org/github.com/dropbox/godropbox for modules documentation.

#### Contributors
- Adam Faulkner
- Antoine Grondin
- Christian Ohler
- Cuong Do
- Harish Mallipeddi
- Jack Ferris
- Jamie Turner
- Pascal Borreli
- Patrick Lee
- Samir Goel
- Sujay Jayakar
- Todd Eisenberger
- Xinyao Hu
- Zviad Metreveli
