## Pytorch加载模型时出现的错误   
[加载模型](http://www.baidu.com/link?url=mDgMhyI9JHIL16kmjbGqlZux1Kzkne-1TSbL5fFwragMSPNyll9Nb2sextrcHe-_oGa5X_iKh02lJYb0GvSflT93d9xqTprgs21bearMP6O&wd=&eqid=d8db9f2300000fe8000000035c185d9d)
## Pytorch出现显存超出的情况   
[OUT OF MEMORY](https://zhuanlan.zhihu.com/p/36307662)中关于item()的介绍： 
由于统一返回值，tensor 返回都为 tensor , 为了获得 python number 现在需要通过.item()来实现，考虑到之前的 loss 累加为 total_loss +=loss.data[0], 由于现在 loss 为0维张量, 0维检索是没有意义的，所以应该使用 total_loss+=loss.item()，通过.item() 从张量中获得 python number.需要注意的是， 如果你的 loss 不转为 python number 再累加，你可能会发现你的内存消耗一直在增加。这是因为0维张量会增加梯度的计算历史。 
如果是先计算，后加，应该就可以不用item()
