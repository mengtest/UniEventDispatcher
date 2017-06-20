# UniEventDispatcher
一个基于委托实现的Unity事件分发器，可以代替SendMessage使用.
委托是什么？
我们不需要从代码层次上去理解，现实生活中，我们有一些事情在某些情况下不想或者无法自己亲力亲为，那么我们可以委托某些人为我们代办，比如付费委托快递帮我们寄送一个包裹，对我们而言，代办（寄快递）的过程就是黑盒子，我们甚至可以认为是“自动化”的，我们不需要去了解过程。同理，在程序中，委托就是这样的角色，不过它托管的是一段代码，比如是一个封装好的函数（function，我们也可以理解为包裹），我们指定一个地址给它（string addr），然后它就会送到那个地址。当然，在一开始，我们已经和收货人约定了一个确定的地址，那么收货人就会开始关注这个地址有没有送包裹过来（注册事件），在包裹到达后（开始分发事件），收货人就会收到通知，至于包裹的内容则需要收货人自己去拆开（比如说通过一段程序）。
有什么用？
目标当然是弱化组件之间的关联，进一步解耦。正如寄快递这个事情，如果我们全程自己做，是不是很累？
