### Under original measure $N_t=1, W_{t+1}\sim N(0,1)$

- From numerical differenciation, we obtained the value for $-f_{2,x^+}$, $f_{2,x}$, $f_{2,w}$, and $f_q$ 

$$
-\underbrace{f_{2,x^{+}}}_{2\times2}\underbrace{X_{2,t+1}^1}_{2\times1}=\underbrace{f_{2,x}}_{2\times2}\underbrace{X_{2,t}^1}_{2\times1}+\underbrace{f_{2,w}}_{2\times4} {\underbrace{W_{t+1}}_{4\times1}}+f_q
$$

- Rearange the terms we have
  $$
  X_{2,t+1}^1=-(f_{2,x^{+}})^{-1}f_{2,x}X_{2,t}^1-(f_{2,x^{+}})^{-1}f_{2,w}W_{t+1}-(f_{2,x^{+}})^{-1}f_q
  $$

- We guess the law of motion for the state evolution equations have the following form
  $$
  \begin{aligned}
  X_{2,t+1}^1&=\psi_{x} X_{2,t}^1+\psi_{w} W_{t+1}+\psi_{q}
  \end{aligned}
  $$

  - Compare coefficients we have
    $$
    \begin{aligned}
    \psi_{x}&=-(f_{2,x^{+}})^{-1}f_{2,x}\\
    \psi_{w}&=-(f_{2,x^{+}})^{-1}f_{2,w}\\
    \psi_{q}&=-(f_{2,x^{+}})^{-1}f_q
    \end{aligned}
    $$



- From numerical differenciation, we obtained the value for $-f_{2,x^+}$, $f_{2,x}$, $f_{2,xx}$, $f_{2,xx^+}$,$f_{2,xw}$, $f_{2,xq}$, $f_{2,x^+x^+}$, $f_{2,x^+w}$, $f_{2,x^+q}$, $f_{2,ww}$, $f_{2,wq}$ and $f_{2,qq}$ 
  $$
  \begin{aligned}
  -f_{2,x^+}X_{2,t+1}^2&=f_{2,x}X_{2,t}^2\\
  &+f_{2,xx}(X_{2,t}^1\otimes X_{2,t}^1)+2f_{2,xx^+}(X_{2,t}^1\otimes X_{t+1}^1)+2f_{2,xw}(X_{2,t}^1\otimes W_{t+1})+2f_{2,xq}X_{2,t}^1\\&+f_{2,x^+x^+}(X_{2,t+1}^1\otimes X_{2,t+1}^1)+2f_{2,x^+w}(X_{2,t+1}^1\otimes W_{t+1})+f_{2,x^+q}X_{2,t+1}^1\\&+f_{2,ww}(W_{t+1}\otimes W_{t+1})+f_{2,wq}W_{t+1}+f_{2,qq}
  \end{aligned}
  $$

- Since we know the law of motion of $X_{2,t+1}^1$, replace $X_{2,t+1}^1$ with $X_{2,t}^1$, $W_{t+1}$, and constant terms, we have
  $$
  \begin{aligned}
  -f_{2,x^+}X_{2,t+1}^2&=f_{2,x}X_{2,t}^2+D^2_{2,xx}(X_{2,t}^1\otimes X_{2,t}^1)+D^2_{2,xw}(X_{2,t}^1\otimes W_{t+1})+D^2_{2,xq}X_{2,t}^1\\&+D^2_{2,ww}(W_{t+1}\otimes W_{t+1})+D^2_{2,wq}W_{t+1}+D^2_{2,qq}
  \end{aligned}
  $$

- We guess the law of motion for the state evolution equations have the following form
  $$
  \begin{aligned}
  X_{2,t+1}^2&=\psi_{x} X_{2,t}^2+\psi_{xq} X_{2,t}^1+\psi_{wq} W_{t+1}+\psi_{qq}\\
  &+\psi_{xx}(X_{t}^1\otimes X_{t}^1)+\psi_{xw}(X_t^1\otimes W_{t+1})+\psi_{ww}(W_{t+1}\otimes W_{t+1})
  \end{aligned}
  $$

  - Compare the coefficients we have
    $$
    \begin{aligned}
    \psi_x&=-(f_{2,x^{+}})^{-1}f_{2,x}\\
    \psi_{xq}&=-(f_{2,x^{+}})^{-1}D_{2,xq}^2\\
    \psi_{wq}&=-(f_{2,x^{+}})^{-1}D_{2,wq}^2\\
    \psi_{qq}&=-(f_{2,x^{+}})^{-1}D_{2,qq}^2\\
    \psi_{xx}&=-(f_{2,x^{+}})^{-1}D_{2,xx}^2\\
    \psi_{xw}&=-(f_{2,x^{+}})^{-1}D_{2,xw}^2\\
    \psi_{ww}&=-(f_{2,x^{+}})^{-1}D_{2,ww}^2\\
    \end{aligned}
    $$
    



### Under new measure $\tilde{N}_{t+1},W_{t+1}=\tilde{\mu}_t+\widetilde{\Gamma} \widetilde{W}_{t+1}$, where $\tilde{W}_{t+1}\sim N(0,1)$

- From numerical differenciation, we obtained the value for $-f_{2,x^+}$, $f_{2,x}$, $f_{2,w}$, and $f_q$ 
  $$
  -\underbrace{f_{2,x^{+}}}_{2\times2}\underbrace{X_{2,t+1}^1}_{2\times1}=\underbrace{f_{2,x}}_{2\times2}\underbrace{X_{2,t}^1}_{2\times1}+\underbrace{f_{2,w}}_{2\times4}({\underbrace{\tilde{\mu}_t}_{4\times1}+\underbrace{\widetilde{\Gamma}}_{4\times 4} \underbrace{\widetilde{W}_{t+1}}_{4\times1}})+f_q
  $$

- Since $\tilde{\mu}_t=\tilde{H}_0+\tilde{H}_1X_{2,t}^1$, we have
  $$
  -{f_{2,x^{+}}}{X_{2,t+1}^1}={f_{2,x}}{X_{2,t}^1}+{f_{2,w}}({{\tilde{H}_0}+\tilde{H}_{1}X_{2,t}^1+{\widetilde{\Gamma}}{\widetilde{W}_{t+1}}})+f_q
  $$

- Rearange the terms we have
  $$
  X_{2,t+1}^1=-(f_{2,x^{+}})^{-1}(f_{2,x}+f_{2,w}\tilde{H}_1)X_{2,t}^1-(f_{2,x^{+}})^{-1}f_{2,w}\tilde{\Gamma}\widetilde{W}_{t+1}-(f_{2,x^{+}})^{-1}f_q-(f_{2,x^{+}})^{-1}f_{2,w}\tilde{H}_0
  $$

- We guess the law of motion for the state evolution equations have the following form
  $$
  X_{2,t+1}^1=\tilde{\psi}_{x} X_{2,t}^1+\tilde{\psi}_{w} \tilde{W}_{t+1}+\tilde{\psi}_q
  $$

  - Compare the coefficients we have
    $$
    \begin{aligned}
    \tilde{\psi}_{x}&=-(f_{2,x^{+}})^{-1}(f_{2,x}+f_{2,w}\tilde{H}_1)\\
    \tilde{\psi}_{w}&=-(f_{2,x^{+}})^{-1}f_{2,w}\tilde{\Gamma}\\
    \tilde{\psi}_{q}&=-(f_{2,x^{+}})^{-1}f_q-(f_{2,x^{+}})^{-1}f_{2,w}\tilde{H}_0
    \end{aligned}
    $$

- Besides, we can directly replace $W_{t+1}$ in the original measure as $\tilde{\mu}_t+\widetilde{\Gamma} \widetilde{W}_{t+1}$, then we have
  $$
  X_{2,t+1}^1={\psi}_{x} X_{2,t}^1+{\psi}_w(\tilde{H}_0+\tilde{H}_1X_{2,t}^1)+{\psi}_w\tilde{{\Gamma}}\tilde{W}_{t+1}+\psi_q
  $$

  - Rearange the terms, we have
    $$
    X_{2,t+1}^1=({\psi}_{x}+{\psi}_w\tilde{H}_1)X_{2,t}^1+{\psi}_w\tilde{{\Gamma}}\tilde{W}_{t+1}+\psi_q+\psi_w\tilde{H}_0
    $$

  - Compare the coefficients we have
    $$
    \begin{aligned}
    \tilde{\psi}_{x}&=({\psi}_{x}+{\psi}_w\tilde{H}_1)&=-(f_{2,x^{+}})^{-1}(f_{2,x}+f_{2,w}\tilde{H}_1)\\
    \tilde{\psi}_{w}&={\psi}_w\tilde{{\Gamma}}&=-(f_{2,x^{+}})^{-1}f_{2,w}\tilde{\Gamma}\\
    \tilde{\psi}_{q}&=\psi_q+\psi_w\tilde{H}_0&=-(f_{2,x^{+}})^{-1}(f_q+f_{2,w}\tilde{H}_0)
    \end{aligned}
    $$
    

- From numerical differenciation, we obtained the value for $-f_{2,x^+}$, $f_{2,x}$, $f_{2,xx}$, $f_{2,xx^+}$,$f_{2,xw}$, $f_{2,xq}$, $f_{2,x^+x^+}$, $f_{2,x^+w}$, $f_{2,x^+q}$, $f_{2,ww}$, $f_{2,wq}$ and $f_{2,qq}$ 
  $$
  \begin{aligned}
  -f_{2,x^+}X_{2,t+1}^2&=f_{2,x}X_{2,t}^2\\
  &+f_{2,xx}(X_{2,t}^1\otimes X_{2,t}^1)+2f_{2,xx^+}(X_{2,t}^1\otimes X_{t+1}^1)+2f_{2,xw}(X_{2,t}^1\otimes W_{t+1})+2f_{2,xq}X_{2,t}^1\\&+f_{2,x^+x^+}(X_{2,t+1}^1\otimes X_{2,t+1}^1)+2f_{2,x^+w}(X_{2,t+1}^1\otimes W_{t+1})+f_{2,x^+q}X_{2,t+1}^1\\&+f_{2,ww}(W_{t+1}\otimes W_{t+1})+f_{2,wq}W_{t+1}+f_{2,qq}
  \end{aligned}
  $$

- Since we know the law of motion of $X_{t+1}^1$, replace $X_{t+1}^1$ with $X_{t}^1$, $W_{t+1}$, and constant terms, we have
  $$
  \begin{aligned}
  -f_{2,x^+}X_{2,t+1}^2&=f_{2,x}X_{2,t}^2+D^2_{2,xx}(X_{2,t}^1\otimes X_{2,t}^1)+D^2_{2,xw}(X_{2,t}^1\otimes ({{\tilde{\mu}_t}+{\widetilde{\Gamma}} {\widetilde{W}_{t+1}}}))+D^2_{2,xq}X_{2,t}^1\\&+D^2_{2,ww}(({{\tilde{\mu}_t}+{\widetilde{\Gamma}} {\widetilde{W}_{t+1}}})\otimes ({{\tilde{\mu}_t}+{\widetilde{\Gamma}} {\widetilde{W}_{t+1}}}))+D^2_{2,wq}({{\tilde{\mu}_t}+{\widetilde{\Gamma}} {\widetilde{W}_{t+1}}})+D^2_{2,qq}\\
  &=f_{2,x}X_{2,t}^2+D^2_{2,xx}(X_{2,t}^1\otimes X_{2,t}^1)+D^2_{2,xw}(X_{2,t}^1\otimes {{\tilde{\mu}_t}+X_{2,t}^1\otimes{\widetilde{\Gamma}} {\widetilde{W}_{t+1}}})+D^2_{2,xq}X_{2,t}^1\\&+D^2_{2,ww}({{\tilde{\mu}_t}\otimes{\tilde{\mu}_t} +{\widetilde{\Gamma}}{\widetilde{W}_{t+1}}\otimes{\tilde{\mu}_t}+ {\widetilde{\Gamma}}{\widetilde{W}_{t+1}}\otimes{\widetilde{\Gamma}}{\widetilde{W}_{t+1}}+{\tilde{\mu}_t}\otimes{\widetilde{\Gamma}}{\widetilde{W}_{t+1}}})+D^2_{2,wq}({{\tilde{\mu}_t}+{\widetilde{\Gamma}} {\widetilde{W}_{t+1}}})+D^2_{2,qq}\\
  \end{aligned}
  $$

- Since $\tilde{\mu}_t=\tilde{H}_0+\tilde{H}_1X_{2,t}^1$, we have
  $$
  \begin{aligned}
  -f_{2,x^+}X_{2,t+1}^2
  &=f_{2,x}X_{2,t}^2+D^2_{2,xx}(X_{2,t}^1\otimes X_{2,t}^1)+D^2_{2,xw}(X_{2,t}^1\otimes {(\tilde{H}_0+\tilde{H}_1X_{2,t}^1)+X_{2,t}^1\otimes{\widetilde{\Gamma}} {\widetilde{W}_{t+1}}})+D^2_{2,xq}X_{2,t}^1\\
  &+D^2_{2,ww}((\tilde{H}_0+\tilde{H}_1X_{2,t}^1)\otimes(\tilde{H}_0+\tilde{H}_1X_{2,t}^1)+{\widetilde{\Gamma}}{\widetilde{W}_{t+1}}\otimes(\tilde{H}_0+\tilde{H}_1X_{2,t}^1)+{\widetilde{\Gamma}}{\widetilde{W}_{t+1}}\otimes{\widetilde{\Gamma}}{\widetilde{W}_{t+1}}+(\tilde{H}_0+\tilde{H}_1X_{2,t}^1)\otimes{\widetilde{\Gamma}}{\widetilde{W}_{t+1}})\\
  &+D^2_{2,wq}({\tilde{H}_0+\tilde{H}_1X_{2,t}^1+{\widetilde{\Gamma}} {\widetilde{W}_{t+1}}})+D^2_{2,qq}\\
  &=f_{2,x}X_{2,t}^2+D^2_{2,xx}(X_{2,t}^1\otimes X_{2,t}^1)+D^2_{2,xw}(I_x\otimes \tilde{H}_0)X_{2,t}^1+D^2_{2,xw}(I_x\otimes\tilde{H}_1)(X_{2,t}^1\otimes X_{2,t}^1)+D^2_{2,xw}(I_x\otimes\tilde{\Gamma})(X_{2,t}^1\otimes\widetilde{W}_{t+1})+D^2_{2,xq}X_{2,t}^1\\
  &+D^2_{2,ww}(\tilde{H}_0\otimes\tilde{H}_0)+
  D^2_{2,ww}(\tilde{H}_1\otimes\tilde{H}_0)X_{2,t}^1+D^2_{2,ww}(\tilde{H}_1\otimes\tilde{H}_1)(X_{2,t}^1\otimes X_{2,t}^1)+D^2_{2,ww}(\tilde{H}_0\otimes \tilde{H}_1)X_{2,t}^1\\
  &+D^2_{2,ww}(\widetilde{\Gamma}\otimes\tilde{H}_0){\widetilde{W}_{t+1}}+D^2_{2,ww}(\widetilde{\Gamma}\otimes\tilde{H}_1)(\widetilde{W}_{t+1}\otimes X_{2,t}^1)+D^2_{2,ww}(\widetilde{\Gamma}\otimes\widetilde{\Gamma})(\widetilde{W}_{t+1}\otimes \widetilde{W}_{t+1})\\
  &+D^2_{2,ww}(\tilde{H}_0\otimes\widetilde{\Gamma})\widetilde{W}_{t+1}+D^2_{2,ww}(\tilde{H}_1\otimes\widetilde{\Gamma})(X_{2,t}^1\otimes\widetilde{W}_{t+1})+D^2_{2,wq}{\tilde{H}_0+D^2_{2,wq}\tilde{H}_1X_{2,t}^1+D^2_{2,wq}{\widetilde{\Gamma}} {\widetilde{W}_{t+1}}}+D^2_{2,qq}
  \end{aligned}
  $$

- Rearrange the coefficients, we can get
  $$
  \begin{aligned}
  -f_{2,x^+}X_{2,t+1}^2
  &=f_{2,x}X_{2,t}^2+(D^2_{2,xx}+D^2_{2,xw}(I_x\otimes\tilde{H}_1)+D^2_{2,ww}(\tilde{H}_1\otimes\tilde{H}_1))(X_{2,t}^1\otimes X_{2,t}^1)\\
  &+(D^2_{2,xw}(I\otimes \tilde{H}_0)+D^2_{2,xq}+D^2_{2,ww}(\tilde{H}_1\otimes\tilde{H}_0)+D^2_{2,ww}(\tilde{H}_0\otimes \tilde{H}_1)+D^2_{2,wq}\tilde{H}_1)X_{2,t}^1\\
  &+(D^2_{2,xw}(I\otimes\tilde{\Gamma})+D^2_{2,ww}(\tilde{H}_1\otimes\widetilde{\Gamma})+D^2_{2,ww}\text{KronComm}(\widetilde{\Gamma}\otimes\tilde{H}_1))(X_{2,t}^1\otimes\widetilde{W}_{t+1})\\
  &+(D^2_{2,ww}(\widetilde{\Gamma}\otimes\tilde{H}_0)+D^2_{2,ww}(\tilde{H}_0\otimes\widetilde{\Gamma})+D^2_{2,wq}{\widetilde{\Gamma}}){\widetilde{W}_{t+1}}\\
  &+D^2_{2,ww}(\widetilde{\Gamma}\otimes\widetilde{\Gamma})(\widetilde{W}_{t+1}\otimes \widetilde{W}_{t+1})\\
  &+D^2_{2,ww}(\tilde{H}_0\otimes\tilde{H}_0)+D^2_{2,wq}{\tilde{H}_0}+D^2_{2,qq}
  \end{aligned}
  $$
  
- We guess the law of motion for the state evolution equations have the following form
  $$
  \begin{aligned}
  X_{2,t+1}^2&=\psi_{x} X_{2,t}^2+\psi_{xq} X_{2,t}^1+\psi_{wq} W_{t+1}+\psi_{qq}\\
  &+\psi_{xx}(X_{2,t}^1\otimes X_{2,t}^1)+\psi_{xw}(X_{2,t}^1\otimes W_{t+1})+\psi_{ww}(W_{t+1}\otimes W_{t+1})
  \end{aligned}
  $$

  - Compare the coefficients we have
    $$
    \begin{aligned}
    \psi_x&=-(f_{2,x^{+}})^{-1}f_{2,x}\\
    \psi_{xq}&=-(f_{2,x^{+}})^{-1}(D^2_{2,xq}+D^2_{2,xw}(I\otimes \tilde{H}_0)+D^2_{2,ww}(\tilde{H}_1\otimes\tilde{H}_0)+D^2_{2,ww}(\tilde{H}_0\otimes \tilde{H}_1)+D^2_{2,wq}\tilde{H}_1)\\
    \psi_{wq}&=-(f_{2,x^{+}})^{-1}(D^2_{2,wq}{\widetilde{\Gamma}}+D^2_{2,ww}(\widetilde{\Gamma}\otimes\tilde{H}_0)+D^2_{2,ww}(\tilde{H}_0\otimes\widetilde{\Gamma}))\\
    \psi_{qq}&=-(f_{2,x^{+}})^{-1}(D^2_{2,qq}+D^2_{2,ww}(\tilde{H}_0\otimes\tilde{H}_0)+D^2_{2,wq}{\tilde{H}_0})\\
    \psi_{xx}&=-(f_{2,x^{+}})^{-1}(D^2_{2,xx}+D^2_{2,xw}(I\otimes\tilde{H}_1)+D^2_{2,ww}(\tilde{H}_1\otimes\tilde{H}_1))\\
    \psi_{xw}&=-(f_{2,x^{+}})^{-1}(D^2_{2,xw}(I\otimes\tilde{\Gamma})+D^2_{2,ww}(\tilde{H}_1\otimes\widetilde{\Gamma})+D^2_{2,ww}\text{KronComm}(\widetilde{\Gamma}\otimes\tilde{H}_1))\\
    \psi_{ww}&=-(f_{2,x^{+}})^{-1}(D^2_{2,ww}(\widetilde{\Gamma}\otimes\widetilde{\Gamma}))\\
    
    \end{aligned}
    $$
    


$$
\begin{aligned}
\psi_x&=-(f_{2,x^{+}})^{-1}f_{2,x}\\
\psi_{xq}&=-(f_{2,x^{+}})^{-1}D_{2,xq}^2\\
\psi_{wq}&=-(f_{2,x^{+}})^{-1}D_{2,wq}^2\\
\psi_{qq}&=-(f_{2,x^{+}})^{-1}D_{2,qq}^2\\
\psi_{xx}&=-(f_{2,x^{+}})^{-1}D_{2,xx}^2\\
\psi_{xw}&=-(f_{2,x^{+}})^{-1}D_{2,xw}^2\\
\psi_{ww}&=-(f_{2,x^{+}})^{-1}D_{2,ww}^2\\
\end{aligned}
$$


### Jump Variables

- Now take the equilibrium conditions for both jump variables and state variables

$$
-f_{x^{+}} \tilde{\mathbb{E}}\left[X_{t+1}^1 \mid \mathcal{F}_t\right]=f_x X_t^1+f_w {\tilde{\mathbb{E}}\left[W_{t+1} \mid \mathcal{F}_t\right]}
$$

- Since under the change of measure $\tilde{N}_{t+1}$, we have $\tilde{\mathbb{E}}[W_{t+1}]=\tilde{H}_0+\tilde{H}_1X_{2,t}^1$
  $$
  -f_{x^{+}} \tilde{{\mathbb{E}}}\left[X_{t+1}^1 \mid \mathcal{F}_t\right]=f_x X_t^1+\underbrace{f_w}_{5\times4} (\underbrace{\tilde{H}_0}_{4\times1}+\underbrace{\tilde{H}_1}_{4\times2}\underbrace{X_{2,t}^1}_{2\times1})
  $$

- Augment $X_{2,t}^1$ to $X_t^1$ and $\tilde{H}_1$ to $\tilde{H}_2$, $\tilde{H}_2 = \begin{bmatrix}\underbrace{0}_{4\times3}&\underbrace{\tilde{H}_1}_{4\times2}\end{bmatrix}$
  $$
  -f_{x^{+}} \tilde{{\mathbb{E}}}\left[X_{t+1}^1 \mid \mathcal{F}_t\right]=f_x X_t^1+\underbrace{f_w}_{5\times4} (\underbrace{\tilde{H}_0}_{4\times1}+\underbrace{\tilde{H}_2}_{4\times5}\underbrace{X_{t}^1}_{5\times1})
  $$

- Rearrange the terms, collect coefficients on $X_t^1$ and constant terms
  $$
  -f_{x^{+}}\tilde{{\mathbb{E}}}\left[X_{t+1}^1 \mid \mathcal{F}_t\right]=(f_x+{f_w}{\tilde{H}_2} )X_t^1+{f_w} {\tilde{H}_0}
  $$

- Apply the generalized Schur decomposition to $-f_{x^+}$ and coefficients on $X_t^1$, transform the first-order system to be lower triangular:
  $$
  -\mathbb{Q}^* f_{x^+}\mathbb{Z}\mathbb{Z}^* \tilde{{\mathbb{E}}}\left[X_{t+1}^1 \mid \mathcal{F}_t\right]=\mathbb{Q}^* (f_x+{f_w}{\tilde{H}_2} )\mathbb{Z}\mathbb{Z}^* X_t^1+\mathbb{Q}^*{f_w} {\tilde{H}_0}
  $$

  $$
  \left[\begin{array}{cc}
  \Lambda_{11}^{+} & \Lambda_{12}^{+} \\
  0 & \Lambda_{22}^{+}
  \end{array}\right] \mathbb{Z}^* \tilde{{\mathbb{E}}}\left[X_{t+1}^1 \mid \mathcal{F}_t\right]=\left[\begin{array}{cc}
  \Lambda_{11}^0 & \Lambda_{12}^0 \\
  0 & \Lambda_{22}^0
  \end{array}\right] \mathbb{Z}^* X_t^1+\mathbb{Q}^*{f_w} {\tilde{H}_0}
  $$

- Write the second block of this equation as:
  $$
  \Lambda_{22}^{+}\left[\begin{array}{ll}
  0 & \mathbb{I}
  \end{array}\right] \mathbb{Z}^* \tilde{{\mathbb{E}}}\left[X_{t+1}^1 \mid \mathcal{F}_t\right]=\Lambda_{22}^0\left[\begin{array}{ll}
  0 & \mathbb{I}
  \end{array}\right] \mathbb{Z}^* X_t^1+\mathbb{Q}^*{f_{2,w}}{\tilde{H}_0}
  $$

- We partition $\mathbb{Z}^*$ as $\mathbb{Z}^*=\left[\begin{array}{c|c}
  Z_{11} & Z_{12} \\
  \hline Z_{21} & Z_{22}
  \end{array}\right]$,
  $$
  \Lambda_{22}^{+}(Z_{21} {\tilde{{\mathbb{E}}}}[X_{1, t+1}^1]+Z_{22}{\tilde{{\mathbb{E}}}}[X_{2, t+1}^1])=\Lambda_{22}^0(Z_{21} X_{1, t}^1+Z_{22} X_{2, t}^1)+\mathbb{Q}^*{f_{2,w}} {\tilde{H}_0}
  $$

- Replace $X_{1, t}^1=\mathbb{N} X_{2, t}^1+C$,
  $$
  \Lambda_{22}^{+}(Z_{21} {\tilde{{\mathbb{E}}}}[\mathbb{N}X_{2, t+1}^1+C]+Z_{22}{\tilde{{\mathbb{E}}}}[X_{2, t+1}^1])=\Lambda_{22}^0(Z_{21} \mathbb{N}X_{2, t}^1+Z_{21} C+Z_{22} X_{2, t}^1)+\mathbb{Q}^*{f_{2,w}} {\tilde{H}_0}
  $$

- Rearrange the terms, we have
  $$
  \Lambda_{22}^{+}((Z_{21} \mathbb{N}+Z_{22}){\tilde{{\mathbb{E}}}}[X_{2, t+1}^1]+Z_{21}C)=\Lambda_{22}^0(Z_{21} \mathbb{N}+Z_{22})X_{2, t}^1 +\Lambda_{22}^0Z_{21} C+\mathbb{Q}^*{f_{2,w}} {\tilde{H}_0}
  $$

- Replace $X_{2,t+1}^1=\tilde{\psi}_{x} X_{2,t}^1+\tilde{\psi}_{w} \tilde{W}_{t+1}+\tilde{\psi}_q$
  $$
  \Lambda_{22}^{+}((Z_{21} \mathbb{N}+Z_{22})(\tilde{\psi}_{x} X_{2,t}^1+\tilde{\psi}_q)+Z_{21}C)=\Lambda_{22}^0(Z_{21} \mathbb{N}+Z_{22})X_{2, t}^1 +\Lambda_{22}^0Z_{21} C+\mathbb{Q}^*{f_{2,w}} {\tilde{H}_0}
  $$

- Rearrange the terms, we have
  $$
  \begin{aligned}
  \Lambda_{22}^{+}(Z_{21} \mathbb{N}+Z_{22})\tilde{\psi}_{x} X_{2,t}^1&=\Lambda_{22}^0(Z_{21} \mathbb{N}+Z_{22})X_{2, t}^1\\
  \Lambda_{22}^{+}((Z_{21} \mathbb{N}+Z_{22})\tilde{\psi}_q+Z_{21}C)&=\Lambda_{22}^0Z_{21} C+\mathbb{Q}^*{f_{2,w}} {\tilde{H}_0}
  \end{aligned}
  $$

  - To solve for $\mathbb{N}$, we have
    $$
    \Lambda_{22}^{+}Z_{21} \mathbb{N}\tilde{\psi}_{x}-\Lambda_{22}^0Z_{21} \mathbb{N}=\Lambda_{22}^0Z_{22}-\Lambda_{22}^{+}Z_{22}\tilde{\psi}_{x}
    $$

  - Multiply both LHS and RHS by $(\Lambda_{22}^0Z_{21})^{-1}$
    $$
    (\Lambda_{22}^0Z_{21})^{-1}\Lambda_{22}^{+}Z_{21} \mathbb{N}\tilde{\psi}_{x}- \mathbb{N}=(\Lambda_{22}^0Z_{21})^{-1}\Lambda_{22}^0Z_{22}X_{2, t}^1-(\Lambda_{22}^0Z_{21})^{-1}\Lambda_{22}^{+}Z_{22}\tilde{\psi}_{x}
    $$

  - To solve for $C$, we have
    $$
    \Lambda_{22}^{+}Z_{21}C={f_{2,w}} \mathbb{Q}^*{\tilde{H}_0}-\Lambda_{22}^{+}(Z_{21} \mathbb{N}+Z_{22})\tilde{\psi}_q
    $$




$$
\begin{aligned}
&X_{1, t+1}^1-D_1=\mathbb{N}\left(X_{2, t+1}^1-D_2\right) \\
&X_{2, t+1}^1-D_2=\tilde{\psi}_x\left(X_{2, t}^1-D_2\right)+\tilde{\psi}_w W_{t+1}
\end{aligned}
$$

$$
\tilde{\psi}_q=D_2-\tilde{\psi}_x D_2=(I-\tilde{\psi}_x)D_2
$$

$$
D_2 =(I-\tilde{\psi}_x)^{-1}\tilde{\psi}_q
$$


$$
\begin{aligned}
X_{1, t+1}^1-D_1&=\mathbb{N}\left(\tilde{\psi}_x\left(X_{2, t}^1-D_2\right)+\tilde{\psi}_w W_{t+1}\right) \\
&=\mathbb{N}\tilde{\psi}_xX_{2, t}^1+\mathbb{N}\tilde{\psi}_w W_{t+1}-\mathbb{N}\tilde{\psi}_xD_2
\end{aligned}
$$









- From numerical differentiation, we have

$$
\begin{aligned}
-f_{x^+}\tilde{\mathbb{E}}[X_{t+1}^2]&=f_{x}X_{t}^2\\
&+\tilde{\mathbb{E}}[f_{xx}(X_{t}^1\otimes X_{t}^1)+2f_{xx^+}(X_{t}^1\otimes X_{t+1}^1)+2f_{xw}(X_{t}^1\otimes W_{t+1})+2f_{xq}X_{t}^1\\&+f_{x^+x^+}(X_{t+1}^1\otimes X_{t+1}^1)+2f_{x^+w}(X_{t+1}^1\otimes W_{t+1})+f_{x^+q}X_{t+1}^1\\&+f_{ww}(W_{t+1}\otimes W_{t+1})+f_{wq}W_{t+1}+f_{qq}]
\end{aligned}
$$


- Replace $W_{t+1}=\tilde{H}_0+\tilde{H}_2X_{t}^1+\tilde{\Gamma}\tilde{W}_{t+1}$
  $$
  \begin{aligned}
  -f_{x^+}\tilde{\mathbb{E}}[X_{t+1}^2]&=f_{x}X_{t}^2\\
  &+\tilde{\mathbb{E}}[f_{xx}(X_{t}^1\otimes X_{t}^1)+2f_{xx^+}(X_{t}^1\otimes X_{t+1}^1)+2f_{xw}(X_{t}^1\otimes (\tilde{H}_0+\tilde{H}_2X_{t}^1+\tilde{\Gamma}\tilde{W}_{t+1}))+2f_{xq}X_{t}^1\\&+f_{x^+x^+}(X_{t+1}^1\otimes X_{t+1}^1)+2f_{x^+w}(X_{t+1}^1\otimes (\tilde{H}_0+\tilde{H}_2X_{t}^1+\tilde{\Gamma}\tilde{W}_{t+1}))+f_{x^+q}X_{t+1}^1\\&+f_{ww}((\tilde{H}_0+\tilde{H}_2X_{t}^1+\tilde{\Gamma}\tilde{W}_{t+1})\otimes(\tilde{H}_0+\tilde{H}_2X_{t}^1+\tilde{\Gamma}\tilde{W}_{t+1}))+f_{wq}(\tilde{H}_0+\tilde{H}_2X_{t}^1+\tilde{\Gamma}\tilde{W}_{t+1})+f_{qq}]
  \end{aligned}
  $$






$$
\begin{align*}
0&=\frac{P_t}{D_t}-\tilde{\mathbb{E}}[\beta\left(\frac{V_{t+1}}{R_t}\right)^{1-\gamma}\left(\frac{V_{t+1}}{R_t}\right)^{\rho-1}\left(\frac{C_{t+1}}{C_t}\right)^{-\rho}\frac{D_{t+1}}{D_t}(\frac{P_{t+1}}{D_{t+1}}+1)]
\end{align*}
$$



$$
\frac{d^2f}{d\text{vmc}_t^2},\frac{d^2f}{d\text{vmc}_t d\text{rmc}_t},\frac{d^2f}{d\text{vmc}_t d\text{pd}_t},\frac{d^2f}{d\text{vmc}_t d\text{x}_t},\frac{d^2f}{d\text{vmc}_t d\sigma_t},\frac{d^2f}{d\text{vmc}_t d\text{gd}_t},\frac{d^2f}{d\text{vmc}_t d\text{gc}_t}
$$

$$
\frac{d^2f}{d\text{rmc}_td\text{vmc}_t},\frac{d^2f}{d\text{rmc}_t^2},\frac{d^2f}{d\text{rmc}_t d\text{pd}_t},\frac{d^2f}{d\text{rmc}_t d\text{x}_t},\frac{d^2f}{d\text{rmc}_t d\sigma_t},\frac{d^2f}{d\text{rmc}_t d\text{gd}_t},\frac{d^2f}{d\text{rmc}_t d\text{gc}_t}
$$

$$
\frac{d^2f}{d\text{pd}_td\text{vmc}_t},\frac{d^2f}{ d\text{pd}_td\text{rmc}_t},\frac{d^2f}{d\text{pd}_t^2},\frac{d^2f}{ d\text{pd}_td\text{x}_t},\frac{d^2f}{d\text{pd}_t d\sigma_t},\frac{d^2f}{d\text{pd}_t d\text{gd}_t},\frac{d^2f}{d\text{pd}_t d\text{gc}_t}
$$






- Second order expansion 

$$
-f_{x^{+}} \mathbb{E}\left[\tilde{N}_{t+1} X_{t+1}^2 \mid \mathcal{F}_t\right]=f_x X_t^2+D_t
$$

- $D_t$ includes all of the first-order contributions after taking expectation, the $D_{t+1}^2$ includes the first-order contributions from second-order expansion before taking expectation. this is known from first order expansion and numerical differentiation

$$
D_t=\mathbb{E}\left[\tilde{N}_{t+1} D_{t+1}^2 \mid \mathcal{F}_t\right]
$$

- Applied the generalized Schur decomposition to $f_{x^+}$ and $f_x$,

$$
-\mathbb{Q}^* f_{x^+}\mathbb{Z}\mathbb{Z}^* {\mathbb{E}}\left[\tilde{N}_{t+1}X_{t+1}^2 \mid \mathcal{F}_t\right]=\mathbb{Q}^* f_x\mathbb{Z}\mathbb{Z}^* X_t^2+\mathbb{Q}^*D_t
$$

$$
\left[\begin{array}{cc}
\Lambda_{11}^{+} & \Lambda_{12}^{+} \\
0 & \Lambda_{22}^{+}
\end{array}\right] \mathbb{Z}^* {\mathbb{E}}\left[\tilde{N}_{t+1}X_{t+1}^2 \mid \mathcal{F}_t\right]=\left[\begin{array}{cc}
\Lambda_{11}^0 & \Lambda_{12}^0 \\
0 & \Lambda_{22}^0
\end{array}\right] \mathbb{Z}^* X_t^2+\mathbb{Q}^*D_t
$$

- Write the second block of this equation as

$$
\Lambda_{22}^{+} \mathbb{E}\left[\tilde{N}_{t+1}\left[\begin{array}{ll}
0 & \mathbb{I}
\end{array}\right] \mathbb{Z}^* X_{t+1}^2 \mid \mathcal{F}_t\right]=\Lambda_{22}^0\left[\begin{array}{ll}
0 & \mathbb{I}
\end{array}\right] \mathbb{Z}^* X_t^2+\left[\begin{array}{ll}
0 & \mathbb{I}
\end{array}\right] \mathbb{Q}^* D_t\tag{1}
$$

- Suppose there exists a $\tilde{D}_t$ that satisfies

$$
\Lambda_{22}^{+} \mathbb{E}\left[\tilde{N}_{t+1}\left(\left[\begin{array}{ll}
0 & \mathbb{I}
\end{array}\right] \mathbb{Z}^* X_{t+1}^2-\tilde{D}_{t+1}\right) \mid \mathcal{F}_t\right]=\Lambda_{22}^0\left(\left[\begin{array}{ll}
0 & \mathbb{I}
\end{array}\right] \mathbb{Z}^* X_t^2-\tilde{D}_t\right)\tag{2}
$$

- From equation 2, we can solve the varibles in $X_t^2$ that are not predetermined using the condition

$$
\left[\begin{array}{ll}
0 & \mathbb{I}
\end{array}\right] \mathbb{Z}^* X_t^2=\tilde{D}_t
$$

- Equation 2 is equivalent to
  $$
  \Lambda_{22}^{+} \mathbb{E}\left[\tilde{N}_{t+1}\left[\begin{array}{ll}
  0 & \mathbb{I}
  \end{array}\right] \mathbb{Z}^* X_{t+1}^2 \mid \mathcal{F}_t\right]-\Lambda_{22}^{+} \mathbb{E}\left[\tilde{N}_{t+1} \tilde{D}_{t+1} \mid \mathcal{F}_t\right]=\Lambda_{22}^0\left[\begin{array}{ll}
  0 & \mathbb{I}
  \end{array}\right] \mathbb{Z}^* X_t^2-\Lambda_{22}^0\tilde{D}_t\tag{3}
  $$

- Take equation 1 into equation 2, we can get
  $$
  \left[\begin{array}{ll}
  0 & \mathbb{I}
  \end{array}\right] \mathbb{Q}^* D_t-\Lambda_{22}^{+} \mathbb{E}\left[\tilde{N}_{t+1} \tilde{D}_{t+1} \mid \mathcal{F}_t\right]=-\Lambda_{22}^0\tilde{D}_t\tag{4}
  $$

- Rearrange the terms we get,

$$
\tilde{D}_t=\left(\Lambda_{22}^0\right)^{-1} \Lambda_{22}^{+} \mathbb{E}\left[\tilde{N}_{t+1} \tilde{D}_{t+1} \mid \mathcal{F}_t\right]-\left(\Lambda_{22}^0\right)^{-1}\left[\begin{array}{ll}
0 & \mathbb{I}
\end{array}\right] \mathbb{Q}^* D_t
$$

- Write $D_t=D\left[\begin{array}{c}
  1 \\
  X_{2, t}^1 \\
  X_{2, t}^1 \otimes X_{2, t}^1
  \end{array}\right]$ and $\tilde{D}_t=\tilde{D}\left[\begin{array}{c}
  1 \\
  X_{2, t}^1 \\
  X_{2, t}^1 \otimes X_{2, t}^1
  \end{array}\right]$，

$$
\tilde{D}\left[\begin{array}{c}
1 \\
X_{2, t}^1 \\
X_{2, t}^1 X_{2, t}^1
\end{array}\right]=\left(\Lambda_{22}^0\right)^{-1} \Lambda_{22}^{+} \mathbb{E}\left[\tilde{N}_{t+1} \tilde{D}\left[\begin{array}{c}
1 \\
X_{2, t+1}^1 \\
X_{2, t+1}^1 X_{2, t+1}^1
\end{array}\right] \mid \mathcal{F}_t\right]-\left(\Lambda_{22}^0\right)^{-1}\left[\begin{array}{ll}
0 & \mathbb{I}
\end{array}\right] \mathbb{Q}^* D\left[\begin{array}{c}
1 \\
X_{2, t}^1 \\
X_{2, t}^1 X_{2, t}^1
\end{array}\right]
$$

- Further simplified to

$$
\tilde{D}\left[\begin{array}{c}
1 \\
X_{2, t}^1 \\
X_{2, t}^1 \otimes X_{2, t}^1
\end{array}\right]=\left(\Lambda_{22}^0\right)^{-1} \Lambda_{22}^{+} \tilde{D} M\left[\begin{array}{c}
1 \\
X_{2, t}^1 \\
X_{2, t}^1 X_{2, t}^1
\end{array}\right]-\left(\Lambda_{22}^0\right)^{-1}\left[\begin{array}{ll}
0 & \mathbb{I}
\end{array}\right] \mathbb{Q}^* D\left[\begin{array}{c}
1 \\
X_{2, t}^1 \\
X_{2, t}^1 \otimes X_{2, t}^1
\end{array}\right]
$$

- where we define

$$
\mathbb{E}\left[M_{t+1}^0\left[\begin{array}{c}
1 \\
X_{2, t+1}^1 \\
X_{2, t+1}^1 \otimes X_{2, t+1}^1
\end{array}\right] \mid \mathcal{F}_t\right]=M\left[\begin{array}{c}
1 \\
X_{2, t}^1 \\
X_{2, t}^1 \otimes X_{2, t}^1
\end{array}\right]
$$

- Matching the coefficients, we have
  $$
  \tilde{D}=\left(\Lambda_{22}^0\right)^{-1} \Lambda_{22}^{+} \tilde{D} M-\left(\Lambda_{22}^0\right)^{-1}\left[\begin{array}{ll}
  0 & \mathbb{I}
  \end{array}\right] \mathbb{Q}^* D
  $$

- Since $\operatorname{vec}(A X B)=\left(B^T \otimes A\right) \operatorname{vec}(X)$, we have

$$
\operatorname{vec}(\tilde{D})=\left(A_2^T \otimes A_1\right) \operatorname{vec}(\tilde{D})+\operatorname{vec}\left(A_3\right)
$$

- Where

$$
A_1=\left(\Lambda_{22}^0\right)^{-1} \Lambda_{22}^{+}, A_2=M, A_3=-\left(\Lambda_{22}^0\right)^{-1}\left[\begin{array}{ll}
0 & \mathbb{I}
\end{array}\right] \mathbb{Q}^* D
$$

- The solution for $\tilde{D}$ is

$$
\operatorname{vec}(\tilde{D})=\left(I-A_2^T \otimes A_1\right)^{-1} \operatorname{vec}\left(A_3\right)
$$

- Then we have
  $$
  X_{1, t}^2=Z_{21}^{-1} Z_{22} X_{2, t}^2+Z_{21}^{-1} \tilde{D}\left[\begin{array}{c}
  1 \\
  X_{2, t}^1 \\
  X_{2, t}^1 \otimes X_{2, t}^1
  \end{array}\right]
  $$
  



### Solve for Jump Variable Coefficients $C$

- Rearrange the law of motion for all equlibrium conditions as
  $$
  \begin{aligned}
  &X_{1, t+1}^1-D_1=\mathbb{N}\left(X_{2, t+1}^1-D_2\right) \\
  &X_{2, t+1}^1-D_2=\tilde{\psi}_x\left(X_{2, t}^1-D_2\right)+\tilde{\psi}_w W_{t+1}
  \end{aligned}
  $$
  where $C=D_1-\mathbb{N} D_2$, $\tilde{\psi}_q=D_2-\tilde{\psi}_x D_2$, and define $D=\begin{bmatrix}D_1\\D_2\end{bmatrix}$

- Again, take the equilibrum conditions for both state variables and jump variables 
  $$
  -f_{x^{+}}\tilde{{\mathbb{E}}}\left[X_{t+1}^1 \mid \mathcal{F}_t\right]=(f_x+{f_w}{\tilde{H}_2} )X_t^1+{f_w} {\tilde{H}_0}+{f_w}\mathbb{E}[W_{t+1}\mid \mathcal{F}_t]
  $$

- We can first add $D$ and then subtract $D$ on both sides to match the forms in the rearanged law of motion
  $$
  -f_{x^{+}} \tilde{\mathbb{E}}\left[X_{t+1}^1-D \mid \mathcal{F}_t\right]-f_{x^+}D=(f_x+{f_w}{\tilde{H}_2} )(X_t^1-D)+(f_x+{f_w}{\tilde{H}_2} )D+{f_w} {\tilde{H}_0}+{f_w}\mathbb{E}[W_{t+1}\mid \mathcal{F}_t]
  $$

- Apply the change of measure $\tilde{N}_{t+1}$, we can get
  $$
  \begin{aligned}
  &-f_{x^{+}} \tilde{{\mathbb{E}}}\left[\begin{bmatrix}\mathbb{N}\\I\end{bmatrix}(X_{2, t+1}^1-D_2)\mid \mathcal{F}_t\right]-f_{x^{+}}D\\&=(f_x+{f_w}{\tilde{H}_2} )\begin{bmatrix}\mathbb{N}\\I\end{bmatrix} (X_{2,t}^1-D_2)+(f_x+{f_w}{\tilde{H}_2} )D+{f_w} {\tilde{H}_0}+{f_w}\mathbb{E}[W_{t+1}\mid \mathcal{F}_t]
  \end{aligned}
  $$
  
- Force the additionally introduced constant terms equal to 0, we get
  $$
  0=(f_x+{f_w}{\tilde{H}_2} )D+f_{x^{+}}D+f_{w}\tilde{H}_0
  $$

























Again, take the equilibrum conditions for both state variables and jump variables 
$$
-f_{x^{+}}\tilde{{\mathbb{E}}}\left[X_{t+1}^1 \mid \mathcal{F}_t\right]=(f_x+{f_w}{\tilde{H}_2} )X_t^1+{f_w} {\tilde{H}_0}+{f_w}\mathbb{E}[X_t\mid \mathcal{F}_t]
$$



- Then we focus on the first block of above equations
  $$
  -f_{1,x^{+}} \tilde{\mathbb{E}}\left[\begin{bmatrix}\mathbb{N}\\I\end{bmatrix}(X_{2, t+1}^1-D_2)\mid \mathcal{F}_t\right]-f_{1,x^+}D_1=f_{1,x}\begin{bmatrix}\mathbb{N}\\I\end{bmatrix} (X_{2,t}^1-D_2)+f_{1,x}D_1+f_{1,w} {\tilde{\mathbb{E}}\left[W_{t+1} \mid \mathcal{F}_t\right]}
  $$

- Apply the change of measure $\tilde{N}_{t+1}$, we can get
  $$
  \begin{aligned}
  &-f_{1,x^{+}} {\mathbb{E}}\left[\begin{bmatrix}\mathbb{N}\\I\end{bmatrix}(X_{2, t+1}^1-D_2)\mid \mathcal{F}_t\right]-(f_{1, x^{+}}\left[\begin{array}{c}
  \mathbb{N} \\
  I
  \end{array}\right]\tilde{\psi}_w) (\tilde{H}_0+\tilde{H}_1X_{2,t}^1)-f_{1,x^{+}}D_1\\&=f_{1,x}\begin{bmatrix}\mathbb{N}\\I\end{bmatrix} (X_{2,t}^1-D_2)+f_{1,x}D_1+f_{1,w} {{\mathbb{E}}\left[W_{t+1} \mid \mathcal{F}_t\right]}+f_{1,w} (\tilde{H}_0+\tilde{H}_1X_{2,t}^1)
  \end{aligned}
  $$

- Force the additionally introduced constant terms equal to 0, we get
  $$
  -(f_{1, x^{+}}\left[\begin{array}{c}
  \mathbb{N} \\
  I
  \end{array}\right]{\psi}_w) \tilde{H}_0-f_{1,x^{+}}D_1=f_{1,x}D_1+f_{1,w}\tilde{H}_0
  $$

  - In principle, we will also have
    $$
    -f_{1,x^{+}} {\mathbb{E}}\left[\begin{bmatrix}\mathbb{N}\\I\end{bmatrix}(X_{2, t+1}^1-D_2)\mid \mathcal{F}_t\right]-(f_{1, x^{+}}\left[\begin{array}{c}
    \mathbb{N} \\
    I
    \end{array}\right]{\psi}_w) \tilde{H}_1X_{2,t}^1=f_{1,x}\begin{bmatrix}\mathbb{N}\\I\end{bmatrix} (X_{2,t}^1-D_2)+f_{1,w}\tilde{H}_1X_{2,t}^1
    $$

  - which implies
    $$
    \mathbb{E}\left[X_{2, t+1}^1\mid \mathcal{F}_t\right]=-(f_{1,x^{+}}\begin{bmatrix}\mathbb{N}\\I\end{bmatrix})^{-1}(f_{1, x^{+}}\left[\begin{array}{c}
    \mathbb{N} \\
    I
    \end{array}\right]{\psi}_w\tilde{H}_1+f_{1,x}\begin{bmatrix}\mathbb{N}\\I\end{bmatrix} +f_{1,w}\tilde{H}_1)X_{2,t}^1
    $$

    - i.e. $\psi_x=-(f_{1,x^{+}}\begin{bmatrix}\mathbb{N}\\I\end{bmatrix})^{-1}(f_{1, x^{+}}\left[\begin{array}{c}
      \mathbb{N} \\
      I
      \end{array}\right]{\psi}_w\tilde{H}_1+f_{1,x}\begin{bmatrix}\mathbb{N}\\I\end{bmatrix} +f_{1,w}\tilde{H}_1)$​






$$
\begin{aligned}
X_{2,t+1}^1&=\psi_{x} X_{2,t}^1+\psi_{w} W_{t+1}+\psi_{q}
\end{aligned}
$$

$$
\begin{aligned}
X_{2,t+1}^1\otimes X_{2,t+1}^1&=(\psi_{x} X_{2,t}^1+\psi_{w} W_{t+1}+\psi_{q})\otimes(\psi_{x} X_{2,t}^1+\psi_{w} W_{t+1}+\psi_{q})\\
&=\psi_{x}\otimes\psi_{x}(X_{2,t}^1\otimes X_{2,t}^1)+\psi_x\otimes\psi_w(X_{2,t}^1\otimes W_{t+1})+\psi_x\otimes\psi_q X_{2,t}^1\\
&+\psi_w\otimes\psi_x(W_{t+1}\otimes X_{2,t}^1)+\psi_w\otimes\psi_w(W_{t+1}\otimes W_{t+1})+\psi_w\otimes\psi_q W_{t+1}\\
&+\psi_q\otimes\psi_x X_{2,t}^1+\psi_q\otimes \psi_wW_{t+1}+\psi_q\otimes\psi_q\\
&=\psi_{x}\otimes\psi_{x}(X_{2,t}^1\otimes X_{2,t}^1)+(\psi_x\otimes\psi_w+\text{KronComm}(\psi_w\otimes\psi_x))(X_{2,t}^1\otimes W_{t+1})\\
&+\psi_x\otimes\psi_q X_{2,t}^1+\psi_w\otimes\psi_w(W_{t+1}\otimes W_{t+1})+(\psi_w\otimes\psi_q+\psi_q\otimes\psi_w) W_{t+1}+\psi_q\otimes\psi_q
\end{aligned}
$$


$$
E(W_{t+1}\otimes W_{t+1})
$$

$$
\mathbb{E}\left[M_{t+1}^0\left[\begin{array}{c}
1 \\
X_{2, t+1}^1 \\
X_{2, t+1}^1 \otimes X_{2, t+1}^1
\end{array}\right] \mid \mathcal{F}_t\right]=M\left[\begin{array}{c}
1 \\
X_{2, t}^1 \\
X_{2, t}^1 \otimes X_{2, t}^1
\end{array}\right]
$$

$$
\begin{bmatrix}
\underbrace{M_{11}}_{1\times1}&\underbrace{M_{12}}_{1\times n_Z}&\underbrace{M_{13}}_{1\times n_Z^2}\\
\underbrace{M_{21}}_{ n_Z\times1}&\underbrace{M_{22}}_{n_Z\times n_Z}&\underbrace{M_{23}}_{n_Z\times n_Z^2}\\
\underbrace{M_{31}}_{n_Z^2\times1}&\underbrace{M_{32}}_{n_Z^2\times n_Z}&\underbrace{M_{33}}_{n_Z^2\times n_Z^2}
\end{bmatrix}=\begin{bmatrix}
1&0&0\\
\psi_{w}E(W_{t+1})&\psi_{x}&0\\
\psi_w\otimes\psi_wE(W_{t+1}\otimes W_{t+1})+(\psi_w\otimes\psi_q+\psi_q\otimes\psi_w)E(W_{t+1})+\psi_q\otimes\psi_q
&\psi_x\otimes\psi_q+(\psi_x\otimes\psi_w+\text{KronComm}(\psi_w\otimes\psi_x))(I\otimes E(W_{t+1}))&\psi_{x}\otimes\psi_{x}
\end{bmatrix}
$$

 

