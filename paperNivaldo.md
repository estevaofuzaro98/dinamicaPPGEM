# **Paper Nivaldo Lemos**
## **1. Moeda**

* **Lagrangiana:**
$$ \mathcal{L}=\frac{m}{2}\left(\dot{x}^{2}+\dot{y}^{2}\right)+\frac{m R^{2}}{4} \dot{\phi}^{2}+\frac{m R^{2}}{8} \dot{\theta}^{2}+m g y \text { sen } \alpha $$

* **Vínculos de rolamento:**

$$ \dot{x}-R \dot{\phi} \sin\theta=0,~~\dot{y}-R \dot{\phi} \cos \theta=0 $$


* **Variáveis de configuração:**

$$q_1 = \phi \\
q_2 = \theta \\
q_3 = x \\
q_4 = y$$

* **Parâmetros:**

$$\begin{align}n &= 4~\text{(fixo)} \rightarrow \text{var. de configuração} \\
m &= 2~(\text{fixo}) \rightarrow \text{velocidades independentes}\\
k &= n - m = 2~(\text{fixo})\\
l &= (1~\text{até}~k) = (1,2)\\
j &= (1~\text{até}~m)= (1,2)\\
\nu &= (1~\text{até}~k) = (1,2)\end{align}$$

* **Obtenção dos termos de vínculo $a_{lj}$:**

$$\dot{q}_{m+l} - \sum_{j=1}^{m} a_{lj} \dot{q}_j = 0,~l=1,\cdots,k$$

$$\dot{q}_{3} - (a_{11}\dot{q}_1 + a_{12}\dot{q}_2) = 0 \Rightarrow \dot{x} - (a_{11}\dot{\phi} + a_{12}\dot{\theta}) = 0\\ 
\dot{q}_{4} - (a_{21}\dot{q}_1 + a_{22}\dot{q}_2) = 0 \Rightarrow \dot{y} - (a_{21}\dot{\phi} + a_{22}\dot{\theta}) = 0$$

$$\dot{x} - (a_{11}\dot{\phi} + a_{12}\dot{\theta}) = \dot{x}-R \dot{\phi} \sin\theta~~\therefore~{\boxed{a_{11} = R\sin{\theta}~~\text{e}~~a_{12} = 0}} \\
\dot{y} - (a_{21}\dot{\phi} + a_{22}\dot{\theta}) = \dot{y}-R \dot{\phi} \cos \theta~~\therefore~{\boxed{a_{21} = R\cos{\theta}~~\text{e}~~a_{22} = 0}}$$

* **Lagrangiana reduzida:**

$$ \bar{L}=\frac{3 m R^{2}}{4} \dot{\phi}^{2}+\frac{m R^{2}}{8} \dot{\theta}^{2}+m g y \text { sen } \alpha $$

* **Equações de Voronec:**
$$
\frac{d}{d t}\left(\frac{\partial \bar{L}}{\partial \dot{q}_{i}}\right)-\frac{\partial \bar{L}}{\partial q_{i}}=\sum_{\nu=1}^{k} \frac{\partial \bar{L}}{\partial q_{m+\nu}} a_{\nu i}+\sum_{\nu=1}^{k} \sum_{j=1}^{m} \frac{\partial L}{\partial \dot{q}_{m+\nu}} b_{i j}^{\nu} \dot{q}_{j}, i=1, \ldots, m
$$

$$
b_{i j}^{\nu}=\frac{\partial a_{\nu i}}{\partial q_{j}}-\frac{\partial a_{\nu j}}{\partial q_{i}}+\sum_{\mu=1}^{k}\left(\frac{\partial a_{\nu i}}{\partial q_{m+\mu}} a_{\mu j}-\frac{\partial a_{\nu j}}{\partial q_{m+\mu}} a_{\mu i}\right)
$$

* **Encontrando os coeficientes $b_{ij}^{\nu}$:**

$$
b^1_{12} = - b^1_{21} = R\cos(\theta) \\
b^2_{12} = - b^2_{21} = - R\sin(\theta)
$$


---
---
## **2. Pêndulo simples via $x$ e $y$**

* **Cinética:**
$$ T(\dot{x},\dot{y}) = \frac{1}{2}m \dot x ^2+ \frac{1}{2}m \dot y^2 $$

* **Potencial:**
$$ V(y) = -mgy $$

* **Lagrangiana:**
$$
\mathcal{L}=\frac{1}{2}m\left(\dot{x}^{2}+\dot{y}^{2}\right) + mgy
$$

* **Vínculação holônoma:**

$$ f(x,y) = x^2 + y^2 - L^2 = 0 $$


* **Variáveis de configuração:**

$$q_1 = x \\
q_2 = y$$

* **Parâmetros:**

$$\begin{align}n &= 2~\text{(fixo)} \rightarrow \text{var. de configuração} \\
m &= 1~(\text{fixo}) \rightarrow \text{velocidades independentes}\\
k &= n - m = 1~(\text{fixo})\\
l &= (1~\text{até}~k) = (1,1)\\
j &= (1~\text{até}~m)= (1,1)\\
\nu &= (1~\text{até}~k) = (1,1)\end{align}$$

* **Obtenção dos termos de vínculo $a_{lj}$:**

$$\dot{q}_{m+l} - \sum_{j=1}^{m} a_{lj} \dot{q}_j = 0,~l=1,\cdots,k$$

$$\dot{q}_{2} - a_{11}\dot{q}_1 = 0 \Rightarrow \dot{y} - a_{11}\dot{x} = 0 ~~\therefore~{\boxed{a_{11} = \frac{\dot{y}}{\dot{x}} }}$$

ou

$$a_{11} = \frac{\partial f(q_1,\cdots,q_m)}{\partial q_1} = \frac{\partial f}{\partial x} = 2x ???$$

* **Lagrangiana reduzida:**

$$ \mathcal{L}=\frac{1}{2}m\left(\dot{x}^{2}+\dot{y}^{2}\right) + mgy $$

$$ f(x,y) = x^2 + y^2 - L^2 = 0 \Rightarrow y = (L^2 - x^2)^{\frac{1}{2}} \\
\frac{d}{dt}f(x,y) = \frac{d}{dt}(x^2 + y^2 - L^2) = 0 \\
\frac{d}{dt}f(x,y) = 2x\dot{x} + 2y\dot{y} = 0 \\
\dot{y} = -\left(\frac{x}{y}\right)\dot{x}$$

$$ \bar{\mathcal L} = \frac{1}{2}m\left\{\dot{x}^{2}+\left[-\left(\frac{x}{y}\right)\dot{x}\right]^{2}\right\} + mgy$$

* **Equações de Voronec:**
$$
\frac{d}{d t}\left(\frac{\partial \bar{\mathcal L}}{\partial \dot{q}_{i}}\right)-\frac{\partial \bar{\mathcal L}}{\partial q_{i}}=\sum_{\nu=1}^{k} \frac{\partial \bar{\mathcal L}}{\partial q_{m+\nu}} a_{\nu i}+ \cancel{\sum_{\nu=1}^{k} \sum_{j=1}^{m} \frac{\partial \mathcal{L}}{\partial \dot{q}_{m+\nu}} b_{i j}^{\nu} \dot{q}_{j}}^{~~0\text{ (holônomo)}}, i=1, \ldots, m
$$

$$
\cancel{b_{ij}^{\nu}=\frac{\partial a_{\nu i}}{\partial q_{j}}-\frac{\partial a_{\nu j}}{\partial q_{i}}+\sum_{\mu=1}^{k}\left(\frac{\partial a_{\nu i}}{\partial q_{m+\mu}} a_{\mu j}-\frac{\partial a_{\nu j}}{\partial q_{m+\mu}} a_{\mu i}\right)}^{~~0\text{ (holônomo)}}
$$

$$
\frac{d}{d t}\left(\frac{\partial \bar{\mathcal L}}{\partial \dot{q}_{1}}\right)-\frac{\partial \bar{\mathcal L}}{\partial q_{1}}=\frac{\partial \bar{\mathcal L}}{\partial q_{2}} a_{11}
$$

$$
\boxed{\frac{d}{d t}\left(\frac{\partial \bar{\mathcal L}}{\partial \dot{x}}\right)-\frac{\partial \bar{\mathcal L}}{\partial x}=\frac{\partial \bar{\mathcal L}}{\partial y} a_{11}}
$$

---

$$ \text{♫ Cedo ou tarde a gente vai se encontrar}\\ \text{Tenho certeza, numa bem melhor}\\ \text{Sei que quando canto você pode me escutar ♪} $$

<center>✨ 13/07/2023 ✝️ 14/07/2023</center>

---

