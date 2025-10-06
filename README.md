# my-foc-eg2213-nce6050ka-nmos
my-foc-eg2213-nce6050ka-nmos


## 项目功能
物料成本仅需24.47元，包括主控stm32f104c8t6的foc无刷驱动板，MOS是60V 50A，但是由于DCDC（tps5405）不要超过30V,电流也不建议超过20A

## 项目参数

* 栅极驱动芯片是使用EG2133淘宝0.8元一颗,配合NCE6050 Nmos淘宝0.4元一颗；
* 主控使用的是最常见的stm32f103c8t6；
* 带有INA181A2+1mΩ的电流采样；
* 所有物料成本仅需24.47元（包括主控）
* 接口引出一路串口，两路iic（其中一路用来和as5600通信）
## 实物图
白嫖的沉金板子，浅浅摆放看一下效果
![IMG_20250511_102350.jpg](https://image.lceda.cn/oshwhub/pullImage/0a52716ac9f14c48aaa62ed7fa72e34a.jpg)
焊接好后的效果
![IMG_20250602_180225.jpg](https://image.lceda.cn/oshwhub/pullImage/2397c05e02b2402e93156faac63fbf0b.jpg)
![IMG_20250602_180216.jpg](https://image.lceda.cn/oshwhub/pullImage/f98af872f6c145c592e4b94379a0be17.jpg)


## 原理解析（硬件说明）

我们来看一下全桥mos的栅极波形
低侧mos的栅极波形
![低侧mos栅极波形.jpg](https://image.lceda.cn/oshwhub/pullImage/8030a555bf494f32ac50a9db56199ea2.jpg)
高侧mos的栅极波形

![高侧波形.jpg](https://image.lceda.cn/oshwhub/pullImage/b6205656a0534854bc71e2db2651feb3.jpg)
放大看，合理的布局和选型能很好的抑制振铃和米勒效应
![IMG_20250602_151649.jpg](https://image.lceda.cn/oshwhub/pullImage/9eaee81499774edfafbb2f2fd5660b93.jpg)



## 注意事项
请按照附件里面的BOM表进行下单即可获得24.47元的大功率带电流环的FOC驱动板。