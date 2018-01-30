

# Note

最近学习总是遇到很多阻碍，现实生活中的，自身的，想着用一些健康的方式来舒缓自己，就把自己学习过程中遇到的问题码出来吧，练一练编辑，也把问题归档好，给未来自己留点坑来瑱。

- [x] **极限**（2018.1.20）       

      $$ \lim\limits_{n \to +\infty} (1+\frac{1}{n^2})(1+\frac{2}{n^2}) \cdots (1+\frac{n}{n^2})$$ 

      (在一个群的入场问题中被卡下来了，日……丢人)

      ------

      **解：** 考虑

      $\frac{x-1}{x} \lt \ln x \lt x-1 \quad $ $x \in (0,+\infty)$ 

      $$\ln \prod\limits_{k=1}^{n}(1+\frac{k}{n^2})=\sum\limits_{k=1}^{n}\ln(1+\frac{k}{n^2}) $$

      $\ln(1+\frac{k}{n^2})\lt \frac{k}{n^2} \quad  $ 而且  $\ln(1+\frac{k}{n^2})\gt\frac{k}{n^2+k}\gt\frac{k}{n^2+n} $

      因而有 $\sum\limits_{k=1}^{n}\ln(1+\frac{k}{n^2}) \lt\frac{n(n+1)}{2n^2}=\frac{1}{2}+\frac{1}{2n}$   且 $\sum\limits_{k=1}^{n}\ln(1+\frac{k}{n^2}) \gt\frac{n(n+1)}{2(n^2+n)}=\frac{1}{2}$

      故 $\lim\limits_{n \to +\infty}\sum\limits_{k=1}^{n}\ln(1+\frac{k}{n^2}) =\frac{1}{2}$ 从而$\lim\limits_{n \to +\infty}\prod\limits_{k=1}^{n}(1+\frac{k}{n^2})=\sqrt{e}$ 

      ​

      PS: 想了一晚上，早上起来又想了一会，感觉好像有点hint 了，结果到桌子前写的时候又什么没有，只好又耻辱的进行了一波 library search ，还是stackexchange 好用，分分钟找到答案，感觉这个不等式自己是想不出来的，只有多见识多记了。（2018.1.21）

      ------

      ​


- [x] **极限**（2018.1.20）

      设$f(x)$ 在$[0,1]$上连续且恒为正，求证 $$\lim_{p \to 0^+}(\int_{0}^{1}f^p(x)\text dx)^{1/p}=e^{\int_{0}^{1}\ln f(x)\text dx}$$ 

      **解：** 变换形式有：

      $$(\int_{0}^{1}f^p(x)\text dx)^{1/p}=(1+\int_{0}^{1}f^p(x)\text dx-1)^{\frac{1}{\int_{0}^{1}f^p(x)\text dx-1}\cdot\frac{\int_{0}^{1}f^p(x)\text dx-1}{p}}$$

      因而就是要证

      $$\lim_{p\to0^+}\frac{\int_{0}^{1}f^p(x)\text dx-1}{p}=\int_{0}^{1}\ln f(x)\text dx$$ 

       $lim_{p\to0^+}\frac{\int_{0}^{1}f^p(x)\text dx-1}{p}\xlongequal{L'Hospital}lim_{p\to0^+}\int_{0}^{1}\ln f(x)\cdot f^{p}(x)\text dx= \int_{0}^{1}\ln f(x)\text dx$

      ​

      ​PS:又是在stackexchange上面填的坑，这次还提了问题，不过还好没有被举报（2018.1.22）

      ------

- [x] **极限**（2018.1.21）

      $\lim\limits_{n \to \infty}n[\int_{0}^{\frac{\pi}{4}}\tan^n(\frac{x}{n})\text dx]^{\frac{1}{n}} $

      (又他娘在一个群的入场问题上被卡了，日 ，不要面子的啊)

       （2018.1.21）

      居然可以确定这玩意有问题，或者直接就是无穷了。

      又是在stackexchange上找的答案，哎哎哎，感觉这个玩意给自己留坑心里总是很毛躁啊，迫切想知道答案。。。

      **解：** 只考虑$ I_n=\int_{0}^{\pi/4}tan^n(x) dx $ 

      有  $I_n=\int_{0}^{\pi/4}\tan^{n-2}(x)\sec^2(x)dx-\int_{0}^{\pi/4}\tan^{n-2}\text dx $

      $$I_n+I_{n-2}=\int_{0}^{1}t^{n-2}dt=\frac{1}{n-1} $$

      又$I_n$ 单调减有下界，从而收敛，所以 $I_n \to0$ .

      PS:填完坑心里的感觉是舒服的。（2018.1.21）

      ------

      ​