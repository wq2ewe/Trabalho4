# Trabalho4
**Estimativa de máxima de verossimilhança**
Para estimar os parâmetros do modelo, adaptamos um algoritmo proposto por Anderson(1973).A log-verossimilhança para o modelo espacial linear t-Student é dado por 

$L(\theta)=log(K_{n}(\eta))-\frac{1}{2}log|\Sigma|-\frac{1}{2\eta}(1+\eta\eta)log(1+c(\eta)\delta)$,

com $log(K{n}(\eta))=\frac{n}{2}log(\frac{c(\eta)}{\pi})+log\Gamma(\frac{1+\eta\eta}{2\eta})-log\Gamma(\frac{1}{2\eta}),\delta=(Y-X\beta)^T|\Sigma|^{-1}(Y-X\beta) e c(\eta)=\eta/(1-2\eta),0<\eta<\frac{1}{2}. Conforme observado por Zellner (1976), a função log-verossimilhança(4.4) é uma função descrescente de \eta, e então não pode ser estimado por máximo verossimilhança. Veja também De Bastiani et al.(2015).$
As funções escores para o modelo espacial linear t-Student são fornecidas por $U_\Theta(\Theta)=(U_\beta^T,U_\phi^T)^T, em que$

   $U_\beta=\partial{L}(\Theta)/\partial\beta=w(\delta)X^T|\Sigma|^{-1}e and U_\phi=\partial{L}(\Theta)/\partial\phi,$

com o j-ésimo elemento de $U_\phi, dado por U_\phi j =\partial{L}(\theta)/\partial\phi j = -\frac{1}{2}tr(|\Sigma|^{-1}(\partial|\Sigma|/\partial\phi j))+\frac(\delta)e ^T|\Sigma|^{-1}(\partial|\Sigma|/\partial\phi j)|\Sigma|^{-1} e,para j=$
