**Estimativa de máxima verossimilhança**
Para estimar os parâmetros do modelo, adaptamos um algoritmo proposto por Anderson (1973). A log-verossimilhança para o modelo espacial linear t-Student é dado por

$\mathcal{L}(\theta)=Log(K_{n}(\eta))-\frac{1}{2}log|\Sigma|-\frac{1}{2\eta}(1+n\eta)log(1+c(\eta)\delta)$,

com [[[]]]

Conforme observado por Zellner (1976), a função log-verossimilhança (4.4) é uma função decrescente de \eta, e então não pode ser estimado por máximo verossimilhança. Veja também De Bastiani et al. (2015).
  As funções escores para o modelo espacial linear t-Student são fornecidas por 
  $U_\theta(\theta)=(U^{T}_{\beta},U^T_ϕ)^T$, em que

  [[[]]]]
  [[[]]]]

  $\hat{\beta}=(\boldsymbol{X}^T\Sigma^{-1}\boldsymbol{X})^{-1}\boldsymbol{X}^T\Sigma^{-1}\boldsymbol{Y}$,

  e de $U_ϕ=0$ tem-se que,
  
  $i$) $ϕ_1tr(\Sigma^{-1}\Sigma^{-1})+ϕ_2tr(\Sigma^{-1}\boldsymbol{R}\Sigma^{-1})=w(\delta)\epsilon^T\Sigma^{-1}\Sigma^{-1}\epsilon$,
  
  $ii$) $ϕ_1tr(\Sigma^{-1}\boldsymbol{R}\Sigma^{-1})+ϕ_2tr(\Sigma^{-1}\boldsymbol{R}\Sigma^{-1}\boldsymbol{R})=w(\delta)\epsilon^T\Sigma^{-1}\boldsymbol{R}\Sigma^{-1}\epsilon$.

  As equações $i)$ e $ii)$ podem ser escritas como $\boldsymbol{A}ϕ=b$, veja Anderson 

  
