2020-3-6：
1，加入不同方法在VISoR-40测试数据集上的量化结果对比
2，加入不同方法输入PLNPR-NGPST enhanced VISoR-40 test images情况下的量化结果对比，文章中的table.1和table.2是展示这些结果的两种排版

2020-3-5：
1，对NGPST在原图上按照量化结果进行调参，加入量化结果和可视化结果。
2，对NGPST在enhanced后的图像上进行调参（ours），加入量化结果和可视化结果。
3，对比：当ours使用与NGPST原图相同的参数时，性能会下降，但是fscore仍然要比NGPST原图高一个点（0.739933792 vs 0.728837695），而ours在经过最优调参后，fscore为0.768235711。
3，MEIT和BigNeuron的excel中加入加权平均后的性能指标


2020-3-2：
1，UltraTracer_qualitatives中之前的thre=10，我检查了下，这里的thre=10其实是使用的UltraTracer的默认参数。之所以我之前写的10是因为UltraTracer的help说明里写的是默认参数下thre=10，从此处可以看出help文档写得可能不太准确，我感觉更像是自动调参模式，因为和手动将参数设置为10的结果并不相同，我在第5页有将这两者结果做了对比。
2，加入NGPST在原图上的调参结果，有个别case在作图的过程中感觉可以补充一下更大或更小参数下的结果，我会在下一个版本加入
3，加入UltraTracer和MEIT在不同参数下的量化结果